# Cowork Brief
## How to Govern AI, version 2.0

**Read this first. It routes to everything else.**

---

## 1. What this is

An eighteen-chapter textbook on AI governance, roughly 93,000 words plus 9,000 of appendices, with forty-one figures, replacing a seven-chapter version currently live at aigov.ogunseye.com. The author is Shawn Ogunseye, tenure-track faculty at Bentley University. The book serves a graduate course and a practitioner audience simultaneously.

The work remaining is drafting and production. The structure is settled and is not open for redesign. If something in the specification looks wrong, flag it rather than fixing it.

---

## 2. Documents

| File | What it is | Authority |
|---|---|---|
| `BOOK_SPECIFICATION_v2.md` | Identity, editorial rules, running cases, all eighteen chapter outlines, appendices, verification items | **Authoritative on content** |
| `FIGURE_SPEC.md` | Visual language, SVG conventions, completeness audit | **Authoritative on figures** |
| `SOURCES_AND_ATTRIBUTION.md` | Reuse rules, source register, currency sweep brief | **Authoritative on sourcing** |
| `TOC_CURRENT.md` | Chapter and section list | Extract of the specification |
| `Chapter_02_Regulatory_Patch.md` | Corrected EU and US regulatory prose | Apply to Chapter 2 before other work |
| `Chapter_01_Revised.md` through `Chapter_06_Revised.md` | Prior drafts of a six-chapter structure | Adaptable material, none current |
| `MANUSCRIPT_AUDIT.md` | Defect catalogue from the prior edition | Historical, mostly addressed |

Files marked SUPERSEDED are pointers. Ignore them.

---

## 3. Order of operations

Do not draft Chapter 1 first. Sequential drafting lets the running cases drift, and by Chapter 15 the promises made in Chapter 4 are lost.

**Phase 1, before any drafting.**

Run the currency sweep in `SOURCES_AND_ATTRIBUTION.md` Section 6 and produce `CURRENCY_FINDINGS.md`. This changes seven chapters and drafting them first means drafting them twice.

Draw three pilot figures against `FIGURE_SPEC.md`, one per canvas type. Confirm the visual language holds, the grayscale test passes, and the PDF path renders. Revise the figure spec from what the pilot shows. Do not draw thirty-eight more against an untested style.

Confirm the build: whether `rsvg-convert` is available to Quarto for the SVG-to-PDF path, or whether PDF variants must be generated alongside. Retrofitting forty-one figures is expensive.

**Phase 2, anchor chapters: 3, 6, 7, 12, 17.**

These carry the most new material and establish vocabulary the rest reference. Chapter 7 is the longest and most important. Chapter 12 has the thinnest source base and must not be written from first principles.

**Phase 3, adapted chapters: 1, 2, 4, 5, 8, 9, 10, 13, 15, 16.**

Prior drafts exist for several. All of it predates the coverage rules and none of it passes unchecked.

**Phase 4, remaining: 11, 14, 18, appendices.**

**Phase 5, consistency pass.** Running case arcs, cross-references, figure numbering, vocabulary, prose register across the whole.

---

## 4. Per-chapter procedure

1. Read the chapter outline in the specification in full, plus Parts A and B.
2. Check `CURRENCY_FINDINGS.md` for anything affecting this chapter.
3. Draft the prose. Not an outline expanded into bullets; connected paragraphs that carry an argument.
4. Write the required-elements list for each figure before drawing it.
5. Draw the figures. Render and view each one.
6. Run the two-pass figure audit.
7. Write the seven review questions in the specified order.
8. Run the quality gates in Section 5.
9. Record status in `PROGRESS.md`.

---

## 5. Quality gates

Run these before considering any chapter done. They are mechanical and catch most defects.

```bash
# Prohibited vocabulary. Any hit is a defect.
grep -niE "business analys|BABOK|IIBA|PMI-PBA|CBAP|MoSCoW|strategy analysis|solution evaluation|requirements life ?cycle" chapters/CH.qmd

# Em dashes. Not permitted anywhere.
grep -n "—\|–" chapters/CH.qmd

# Banned constructions.
grep -niE "the question is not|creates challenges|presents challenges|several .* emerge|it is important to note|as such,|accordingly,|consider .* as an example" chapters/CH.qmd

# Bold-term-plus-fragment, the disguised list.
grep -nE "^\*\*[A-Z][^*]{2,40}\*\*\.? " chapters/CH.qmd
```

Then the judgment checks, which no grep catches.

**Coverage of three system classes.** Every Part II chapter must address predictive, generative, and agentic systems. Ask explicitly what this stage looks like for each. If two of three answers are missing, the chapter is not finished. This rule fails silently because the predictive paradigm is the default and reasserts itself.

**Coverage of build and buy paths.** Most readers select rather than build. A chapter assuming the reader trained the model has excluded a third of the running cases and most of the audience.

**Depth.** Every concept named must be explained: what it is, why it matters, how it works mechanically, what it trades off, when to use it over alternatives. A one-sentence gloss is not an explanation. Check the chapter's "Explain, do not name" list.

**Figures.** Both audit passes recorded. Structural minimums met: entry and exit conditions on process figures, trust boundaries on architecture figures, handoffs on role figures.

**Sourcing.** Every factual claim traced. Nothing invented. Hypotheticals identified as hypothetical. No real organization attached to an invented scenario.

---

## 6. Build

Existing pipeline, working, do not replace it.

Quarto 1.8.25, rendering to `/docs`, deployed via GitHub Pages from `github.com/shawnogunseye/GovAI` to `aigov.ogunseye.com`. A publish workflow exists at `.github/workflows/publish.yml`. A `CNAME` file and `.nojekyll` are in the repo root. Version 1.5.2 carries DOI 10.5281/zenodo.18407349 and remains permanently citable there. Version 2.0 needs its own DOI. Whether that is a new Zenodo record or a new version of the existing one is an author decision, noted in `AUTHOR_QUESTIONS.md`.

Source is `.qmd`, one file per chapter, in `chapters/`. Figures are separate SVG files in `figures/`, referenced from the qmd, never inlined. Per-chapter bibliographies via BibTeX and CSL, which version 1.5.2 lacked.

Three outputs from one source: HTML for the site, PDF for Pressbooks and KDP, EPUB. All three must build before any chapter is considered shipped, because format-specific breakage found late is expensive.

**Decided, August 2026; licence revised 23 September 2026.** Version 2.0 is titled *How to Govern AI: Foundations and Practical Guide to AI Governance* and is **all rights reserved**, © 2026 Shawn Ogunseye. It was CC BY-NC 4.0 until 23 September 2026. The Appendix C templates keep CC BY-NC 4.0 as a narrower, deliberate grant. It is the successor to *Governing AI: Leading Responsible Innovation* and **replaces it** at aigov.ogunseye.com on release. The retitle and the license change are both deliberate; a successor may carry a new title.

The earlier work is not erased. Version 1.5.2 remains permanently citable through DOI 10.5281/zenodo.18407349, which is what the Zenodo deposit is for. Replacement means the live site serves 2.0, not that 1.5.2 ceases to exist.

Three production consequences.

**URL continuity.** The current site serves `chapters/01-foundations.html` through `chapters/11-appendix-d.html`, an eleven-file structure. Version 2.0 has eighteen chapters plus four appendices, so filenames change and `07-future.html` has no direct successor. Every existing inbound link, citation, and syllabus reference breaks unless redirects are in place. Produce a redirect map from the old paths to their nearest 2.0 equivalent before release, and archive the rendered 1.5.2 site under `/v1/` so nothing 404s. Chapter 7 of the old book, on ongoing issues and future directions, needs its content checked for anything orphaned by the restructure.

**Licence transition.** Copies distributed under CC BY-NC-ND 4.0 stay under that license permanently; a license cannot be revoked retroactively. This is normal and requires nothing except that the front matter be clear which license governs which work.

**Front matter.** Should state plainly that this book supersedes the earlier one, name it, and give its DOI, so readers arriving from an old citation understand what happened.

---

## 7. Prose register

The specification's Part B is binding and detailed. The short version:

Flowing connected paragraphs. No em dashes. No lists standing in for explanation. No bold term followed by a definition fragment. No section that is a header plus one paragraph. Active voice with named actors. One qualifier per claim, only where the uncertainty is real and explained.

Write as if teaching a capable person who does not yet know the material. Not as reference, not as a framework summary, not as a compliance manual.

The book applies information-gathering technique; it does not teach it from scratch. Give the actual questions to ask in the chapter where they do work. Do not explain how to run a workshop.

---

## 8. Continuity

Maintain `PROGRESS.md` with, per chapter: status, word count, figures complete and audited, quality gates run, open questions, and anything deferred. Update it at the end of every session, not the start of the next one.

Maintain `DECISIONS.md` for anything resolved during production that the specification does not cover, with the reasoning. The next session will not remember why.

Maintain `AUTHOR_QUESTIONS.md` for anything requiring Shawn's judgment. Do not stall on these; note them and continue. Structural changes, title and license, running case arcs, and any contradiction between a finding and the specification are all his call.

---

## 9. Standing instructions

Flag rather than fix. If the specification looks wrong, say so in `AUTHOR_QUESTIONS.md` and proceed as written.

Verify rather than assume. The regulatory and standards landscape moved substantially between the specification's sources and now, and it will move again during production. Every date, instrument number, and threshold gets checked against a primary source.

Redraw rather than reproduce. Every figure is original. Credit sources as the origin of a model and state divergences explicitly. The divergences are where the book has a view.

Be honest about gaps. Where practice has no good answer, such as consulting stakeholders who cannot be reached, say so rather than presenting a partial substitute as a solution. The author would rather publish an acknowledged gap than a false resolution.
