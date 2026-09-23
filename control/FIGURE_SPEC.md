# Figure Specification

**Established 29 August 2026 from the two pilot figures for Chapter 1.**
`COWORK_BRIEF.md` treats this file as existing and authoritative on figures. It did not exist in the repository. This version is written from the figure rules in `BOOK_SPECIFICATION_v2.md` Part B, tested against two figures drawn, rendered, viewed, and grayscale-checked. Revise it from what further pilots show.

---

## 1. Why the prior visual language was replaced

The sixteen figures in v1.5.2 use linear gradients, drop shadows, and six saturated hues at similar lightness. Three problems follow.

They fail the grayscale test. Hues that read as distinct in colour collapse to near-identical greys in print, so a reader of the paper edition cannot tell two categories apart. Colour was carrying meaning that only exists on a screen.

They are decorated rather than drawn. Gradients and shadows add visual weight without adding information, and they compete with the content for the reader's attention in a book whose prose rules forbid ornament everywhere else.

They cannot show what the specification requires. Entry and exit conditions, trust boundaries, and handoffs need line weight, dash pattern, and explicit labelled zones. A style built on filled gradient boxes has no vocabulary for any of them.

The v1.5.2 figures are not being retrofitted. They belong to a book that is being replaced.

---

## 2. Canvas types

Three canvases, one per figure kind. Every figure declares which it is.

**Comparison canvas.** Rows are the things compared, columns are the dimensions of comparison. Used where the reader needs to hold several parallel cases in view. Figures 1.1 and 1.2 are both of this type. Width 900, height set by row count.

**Process canvas.** Left-to-right or top-to-bottom flow with labelled stages. **Must carry an explicit entry condition and an explicit exit condition**, drawn as labelled bands rather than implied by the first and last box. This is the rule most often broken, and a process figure without them is not finished.

**Architecture canvas.** Components and the connections between them. **Must show trust boundaries** as a distinct line treatment, and must label what crosses each one.

A figure showing roles is a comparison canvas with handoffs drawn as arrows between rows, and the handoffs are mandatory.

---

## 3. The palette, and why it is built on value

Categories are distinguished by **lightness**, never by hue alone. This is what makes the grayscale test pass by construction rather than by luck, and it is also what makes the figures legible to readers with colour vision deficiency.

| Token | Hex | Grey value | Use |
|---|---|---|---|
| ink | `#1a2230` | darkest | Titles, rules, primary text, highest category |
| slate | `#46536b` | dark | Secondary text, borders, arrows, second category |
| mid | `#8794a8` | mid | Third category, de-emphasised fills |
| light | `#c9d1dc` | light | Fourth category, filled outcome boxes |
| pale | `#eef1f5` | lightest fill | Fifth category, panel backgrounds |
| paper | `#ffffff` | white | Canvas, and the fill for boxes that mean "a control" |
| alert | `#8a3324` | dark, warm | **One use only:** marking an absence or an impossibility |

Five ordered greys is the maximum. A figure needing a sixth category needs to be two figures.

`alert` is the single exception to the value rule and is rationed deliberately. In Figure 1.1 it marks the one place where no review position exists. If it appears in a figure to mean "important" or "bad", it has been misused.

Text on `ink`, `slate`, or `mid` fills is `#ffffff`. Text on `light` or `pale` is `ink`.

## 4. Type

One family, one scale. `"Source Sans Pro", "Helvetica Neue", Helvetica, Arial, sans-serif`, declared in a `<style>` block at the top of the SVG so it is set once.

| Class | Size | Weight | Use |
|---|---|---|---|
| `.ttl` | 17 | 700 | Figure title, inside the canvas |
| `.cls` / `.lvl` | 14 | 700 | Row label |
| `.bx` | 12.5 | 400 | Box primary text |
| `.col` | 11 | 700 | Column header, letter-spaced `.06em`, in `slate` |
| `.sm` | 11 | 400 | Box secondary text, in `slate` |
| `.em` | 11 | italic | Notes and cascade annotations |

No size below 10.5. At the printed width of a letter-page figure, smaller type is not readable.

## 5. Construction rules

Flat fills only. No `linearGradient`, no `feDropShadow`, no `filter`.

Stroke weights carry meaning and there are three. `1` is a divider between rows. `1.2` to `1.6` is an ordinary box or connector. `1.8` to `2` is a boundary, a control, or a cascade arrow, and is reserved for elements the reader must not miss.

Dashes carry meaning and there are two patterns. `5 3` marks a control that exists but is weakened, such as review by sampling. `4 3` or `3 3` marks something outside the main structure, such as a category that sits off a cascade.

Arrowheads are filled triangles, drawn as a `polygon`, eight units long. Do not use markers; they behave inconsistently across the three renderers this book passes through.

Every figure carries `role="img"`, an `aria-label` repeating the caption, and a `<title>` element as the first child. The book is published on the web and this is not optional.

`viewBox` is `0 0 900 H`. Never set `width` or `height` attributes on the root element; let the container scale it.

## 6. The required-elements list

Written **before** the figure is drawn, placed as an HTML comment in the `.qmd` immediately above the figure reference so that it travels with the figure and survives revision.

```
<!-- FIGURE N.N REQUIRED ELEMENTS
Must appear: [every stage, component, actor, boundary, relationship]
Deliberately excluded: [what, and why]
-->
```

The exclusion line is not optional. A figure that omits something the prose discusses must record that the omission was a decision, otherwise a later reviewer cannot distinguish a choice from an oversight.

## 7. The two audits

**Pass one, against the list.** Check the list against the chapter prose first and confirm the list is complete. Then check the drawing against the list. This order matters: reviewing the drawing directly invites confirming that what is present is correct while missing what is absent, which is the failure mode that produced the defects in the prior edition.

**Pass two, blind.** A reviewer who has read the chapter but not seen the list is asked what they expected to see and did not.

Both are recorded in `PROGRESS.md`. A figure that has not passed both is not finished.

## 8. Mechanical checks

```bash
# no gradients, filters or shadows
grep -lE "linearGradient|radialGradient|feDropShadow|filter=" figures/*.svg

# no hardcoded root dimensions
grep -lE "<svg[^>]*(width|height)=" figures/*.svg

# accessibility attributes present
for f in figures/*.svg; do grep -q 'role="img"' "$f" || echo "MISSING role: $f"; done

# every colour is on the palette
grep -ohE '#[0-9a-fA-F]{6}' figures/*.svg | sort -u
```

**Watch for two failure modes that are invisible in the source.**

A CSS class fill beats a `fill="..."` presentation attribute on the same element. Writing `class="f bx" fill="#ffffff"` for white text on a dark band produces *dark text on a dark band*, which renders as nothing at all. Define a reversed-text class and apply it as a class. This bit two figures on the first pass.

Then, when adding such a class, check the name is not already in use in that file. Adding a second `.rv` rule to a figure that already had one silently changed the fill of every element using it. Both errors were caught only by looking at the render.

**Render and view every figure.** A figure that has not been looked at has not been checked. Text overflowing the canvas is invisible in the source and obvious in the render, and it happened once in these two pilots.

```bash
rsvg-convert -w 1400 figures/F.svg -o /tmp/F.png          # view this
python3 -c "from PIL import Image; Image.open('/tmp/F.png').convert('L').save('/tmp/F_g.png')"
```

The grayscale render is the test. If two categories are not distinguishable in it, the figure fails regardless of how it looks in colour.

## 9. Redrawing from a source

Structure, sequence, and concepts are not copyrightable. Particular visual expression is. This holds whatever the book is licensed under: a redrawing close enough to function as a copy infringes on its own. Where a figure sits in Appendix C, which is offered under CC BY-NC, it is worse, because the copy is then offered onward to every reader for further adaptation.

Redraw from the described structure, in this visual language, never by tracing. **State the divergence in the caption or the walkthrough.** Where this book's model differs from the source, the divergence is both the editorially interesting part and the evidence of independent expression.

## 10. Build path, confirmed

`rsvg-convert` (librsvg) is what Quarto uses to place SVG into PDF. Confirmed working on 29 August 2026: figures reach the PDF as **vector**, not raster, and their text remains selectable in the output.

**No PDF variants of the figures are needed.** One SVG per figure serves HTML, PDF, and EPUB.

Install if absent: `apt-get install librsvg2-bin`, or `brew install librsvg`.

The PDF build additionally requires a working LaTeX. On this container the default `xelatex` path failed on Latin Modern font metrics, and `pdf-engine: pdflatex` is set in `_quarto.yml` as a result. The lean `preamble.tex` exists for the same reason: every package it no longer loads was a way for the build to fail on a machine that did not have it.

---

## Appendix: figures completed

| Figure | Chapter | Canvas | Elements list | Audit 1 | Audit 2 |
|---|---|---|---|---|---|
| 1.1 System classes and intervention points | 1 | Comparison | Yes, in `.qmd` | Passed | **Outstanding** |
| 1.2 Harm levels, cascade, detection | 1 | Comparison | Yes, in `.qmd` | Passed, one text overflow found and fixed | **Outstanding** |

Forty figures remain against the specification's actual 42-figure total (not 41, corrected by CH426, Pass 17, 2026-09-13: BOOK_SPECIFICATION_v2.md's own chapter-by-chapter figure list sums to 42, and this file's prior "41 total"/"thirty-nine remain" notes were themselves stale). Both pass-two audits require a reader who is not the author of the figure.
