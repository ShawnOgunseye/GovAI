# Retired: fig-16-02-supply-chain.svg and fig-16-03-inherited-terms.svg

Retired 2026-09-13, agent cl, Pass 30 (CH), per CH523 (final pass) and rolling
finding 1.

Both figures were superseded when Chapter 16's prose was revised to reject
the claims they draw:

- fig-16-02 drew a compulsory five-layer supply chain (base model, fine-tune,
  adapter, integration, deployment) with a monotonic visibility gradient and
  near-flat obligation bars. The current chapter text (section 16.6) states
  explicitly that a real supply chain "can also include data and labeling
  providers, independent evaluators, a model hosting or cloud provider, a
  retrieval or grounding source, an orchestration layer, and one or more
  subprocessors, and these can branch and repeat rather than forming a
  single line," and that visibility "has to be assessed layer by layer
  rather than assumed to decrease steadily with distance from deployment."
  Table 16.1 replaced this figure in the chapter.

- fig-16-03 drew a two-tier (standard/self-serve vs. enterprise) comparison
  asserting that standard tiers "frequently permit" training on customer
  inputs by default and enterprise tiers "typically exclude" it, and that
  refusal and safety calibration is "fixed by developer, not
  customer-specific" at every tier. Current provider documentation checked
  2026-09-13 (OpenAI enterprise privacy, Anthropic's commercial-data policy,
  Google Cloud's zero-data-retention documentation) contradicts the
  categorical market-default claim, and section 16.7 of the current chapter
  states refusal behavior is "a mix of an inherited policy floor and its own
  configuration" that "needs to be tested as the assembled system actually
  behaves rather than assumed from the base model's reputation alone."
  Table 16.2 replaced this figure in the chapter.

Neither SVG is referenced anywhere in the current chapter text. Both are
kept here, unreferenced, rather than deleted, in case the historical
required-elements record is needed. Do not restore either to `figures/` or
to any build inventory without redrawing it against the chapter's current
claims and re-running the full figure approval process in
`badw-book.md` section 11.
