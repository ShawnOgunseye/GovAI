# Retired: fig-15-01-traceability-matrix.svg and fig-15-02-model-card-annotated.svg

Retired 2026-09-13, agent cl, Pass 29 (CH), per CH518 (final pass) and rolling
finding 2.

Both figures were superseded when Chapter 15's prose was revised to correct
the claims they draw:

- fig-15-01 labelled FL-014 "MET" from a 50-case sample review with no
  sampling protocol, tolerance, or comparison against the model's actual
  decision logic, and labelled FL-015 "PARTIALLY MET" from a readability
  score alone. The current chapter (section 15.2, Table 15.1) marks both
  rows "Unverified" and states directly why a readability score cannot
  substitute for comprehension evidence and why a sample review without a
  stated protocol cannot support "met" against Regulation B's actual-
  principal-reasons standard. Table 15.1 replaced this figure in the
  chapter.

- fig-15-02 drew five model-card sections as the card's full structure. The
  current chapter (section 15.3) states the five-category set is a
  non-exhaustive core, names the additional categories the original model
  card framework covers, and adds provenance/version, maintenance/
  ownership, security/misuse/legal restrictions, and deployment
  dependencies/monitoring as further categories a deploying organization
  should add. Table 15.2 replaced this figure in the chapter, mapping each
  section to the specific follow-up question a reviewer should ask.

Neither SVG is referenced anywhere in the current chapter text. Both are
kept here, unreferenced, rather than deleted, in case the historical
required-elements record is needed. Do not restore either to `figures/` or
to any build inventory without redrawing it against the chapter's current
claims and re-running the full figure approval process in
`badw-book.md` section 11.
