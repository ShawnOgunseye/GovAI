# How to Govern AI: Foundations and Practical Guide to AI Governance
## Book Specification and Chapter Outlines

**Version 2. Supersedes BOOK_SPECIFICATION.md, TOC.md, TOC_v2.md, and TOC_v3.md.**
**Current as of August 2026.**

**Purpose.** This document is the authoritative structural and editorial specification for the manuscript. It exists so that any writer, human or otherwise, can produce or continue chapters consistent with the whole. Read it in full before drafting any chapter.

**Note on this document's own format.** This is a planning artifact and uses lists and structure freely. The manuscript itself does not. See Style Rules.

---

# PART A: BOOK IDENTITY

## Title and License

*How to Govern AI: Foundations and Practical Guide to AI Governance*

**All rights reserved, © 2026 Shawn Ogunseye.** Changed 23 September 2026 from CC BY-NC 4.0. Free to read at aigov.ogunseye.com. The Appendix C templates remain CC BY-NC 4.0 so readers can adapt them.

This book succeeds and replaces *Governing AI: Leading Responsible Innovation*, the author's earlier work, currently live at aigov.ogunseye.com at version 1.5.2 under CC BY-NC-ND 4.0 with DOI 10.5281/zenodo.18407349. On release, 2.0 takes over that domain. The earlier work remains permanently citable through its DOI and should be archived under a subpath rather than removed. Front matter should state that this book supersedes the earlier one, name it, and give its DOI, so readers arriving from an old citation understand what happened.

The license permits adaptation, which shapes production in three ways. Templates in Appendix C must be written to be adapted and must be original rather than derived from published examples. Every figure must be independent expression rather than a close redrawing, since readers are licensed to adapt further. And the NonCommercial term should be verified against the Pressbooks institutional arrangement before publication, since some open textbook programs prefer CC BY.

## Audience

Two audiences, addressed simultaneously without compromise to either.

The primary audience is graduate and upper-level undergraduate students in business, information systems, law, and public policy taking a first course in AI governance. They have general professional literacy but not necessarily technical or legal training. They should be able to read the book front to back.

The secondary audience is working practitioners moving into AI governance from adjacent functions such as privacy, compliance, risk, audit, product, or data science. They need the book usable as reference after first reading.

Assume the reader is intelligent, motivated, and unfamiliar. Do not assume prior knowledge of machine learning, regulation, or governance practice. Do not condescend.

## Positioning

This is a textbook, not a manifesto, not a survey of literature, and not a compliance manual. It teaches a practice.

It is aligned with the IAPP AIGP body of knowledge but not constrained by it. Where the body of knowledge is thin and the practice is not, follow the practice. Where it covers material that does not serve the argument, omit it. Never structure a chapter around a certification domain.

## The Central Argument

State this nowhere explicitly. Let the structure carry it.

AI governance is not a collection of principles to be endorsed. It is a practice with a method: identify who is affected and what they need, translate obligations and needs into specific and verifiable requirements, trace those requirements through design and implementation to evidence, and evaluate whether the resulting system and the governance around it actually work.

The book demonstrates this by applying the same discipline consistently across every chapter and every lifecycle stage. A reader who finishes should be able to walk into an unfamiliar AI system and know what to ask, in what order, and what artifacts should exist.

The methodological through-line is demonstrated through consistent application, never by naming a parent discipline.

## Word Budget

Target 90,000 to 95,000 words of body text plus approximately 9,000 words of appendices. Per-chapter targets appear below and sum to roughly 93,000.

---

# PART B: EDITORIAL RULES

## Prohibited Vocabulary

The following and any close variant must not appear anywhere in the manuscript, including front matter, appendices, figure captions, and review questions.

- business analysis, business analyst, BA
- BABOK, IIBA, PMI-PBA, CBAP
- business analysis planning and monitoring, strategy analysis, requirements life cycle management, requirements analysis and design definition, solution evaluation (these are proper names of knowledge areas and read as citations even lowercased)
- MoSCoW
- Any branded technique framework carrying a discipline's imprint, including GAIN and similar acronym frameworks

Where a prohibited framework supplied useful content, present the content directly without the brand.

## Permitted Vocabulary

Permitted because common across regulatory, safety, and systems engineering practice: requirements, traceability, traceability matrix, stakeholder analysis, impact assessment, root cause analysis, RACI, prioritization, acceptance criteria, verification, validation.

Use "elicitation" sparingly. Prefer "gathering information," "structured interviews," or "stakeholder consultation." One or two uses across the book is acceptable.

Prefer "must-have, should-have, could-have, and out of scope" over any acronym.

## Naming Rule: AI System Lifecycle

Use "AI system lifecycle," never "AI lifecycle." The longer form matches the EU AI Act, NIST AI RMF, and ISO/IEC 22989, and holds the socio-technical framing established in Chapter 1. The short form recenters the model and contradicts the argument. Applies to headings, body prose, figure captions, and review questions.

**Decided 2026-09-12.** The rule admits one exception: naming the short form as the term the book is correcting, so the reader can recognize it elsewhere. "Most writing on this subject refers to the AI lifecycle, as though there were one" and "the three lifecycles run inside what is usually called the AI lifecycle" (Chapter 3) are reported usage, attributed to other writing and immediately corrected in the same sentence, not the book adopting the short form as its own term. That is the only sanctioned pattern: the short form may appear when explicitly marked as what others call it, in a sentence that goes on to supply or imply the book's own term. It may not appear afterward in the same chapter as a live synonym. Applying this required no change to Chapter 3.

## Coverage Rule: Three System Classes

**This is the rule most at risk of silent violation, because the predictive paradigm is the default and reasserts itself unless actively corrected.**

Three system classes run through the entire book: predictive systems, generative systems, and agentic systems. Every chapter in Part II must address all three. No lifecycle chapter ships with predictive-only examples.

Part III concentrates the controls that content generation and autonomous action require, because those controls cohere and do not sit at a single lifecycle stage. Part III does not mark where generative and agentic systems enter the book. They enter in Chapter 1 and are present continuously.

When drafting any Part II chapter, verify explicitly: what does this stage look like for a predictive system, for a generative system, and for an agentic system? If two of the three answers are absent, the chapter is not finished.

## Coverage Rule: Build and Buy Paths

Most readers will select rather than build. Chapter 4 establishes that the lifecycle stages are the same across paths while the work differs, and every subsequent Part II chapter carries a short passage on what the stage looks like when the organization bought rather than built. A chapter that assumes the reader trained the model has excluded a third of the running cases and most of the audience.

## Prose Style

Model the prose on academic writing in the Parsons register: flowing, connected paragraphs carrying an argument forward. Professional, accessible, no ornament.

Hard rules:

1. **No em dashes.** Use commas, semicolons, or restructure. Not a colon: see rule 1a. In practice the em-dash fix is a comma, a semicolon, or a restructure.
1a. **Colons do not join clauses.** Permitted only for a ratio, a time, a citation, or a title-subtitle pair. A clause-joining colon is an unwanted tic, confirmed directly by the author 2026-09-13 (CH432, Pass 17), not a style option this specification's rule 1 should be read as reopening. Standing project rule, adopted 2026-09-04, carried forward into this specification 2026-09-13. Also encoded in `w/forBook/badw-book.md` section 5; book-wide remediation status is tracked in `rules/badw-book-log.md`.
2. **No bulleted lists as a substitute for explanation.** Lists are permitted only for genuine enumerations where order or discreteness is the point. If a list could be a paragraph, make it a paragraph.
3. **No bold term followed by a definition fragment.** This is a list wearing a costume.
4. **No what/why/how subheading patterns.**
5. **No section consisting of a header and one paragraph.** Develop it or fold it in.

Banned constructions, eliminated on sight: "the question is not X but Y"; "this creates challenges" and "this presents challenges" as transitions; "several X emerge"; "beyond X, Y"; "it is important to note that," "importantly," "notably," "as such," "accordingly"; "consider X as an example" (give the example); stacked hedges.

Prefer active voice with named actors. "Organizations should establish oversight" hides who does what.

## Depth Rule

Every concept the book names must be explained: what it is, why it matters for governance, how it works mechanically at a level the reader can act on, what it trades off, and when to use it over alternatives. A one-sentence gloss is not an explanation. If a chapter names a technique and moves on, the technique should have been developed or cut.

Each chapter outline includes an **Explain, do not name** list identifying items most at risk of reduction to a gloss. Not exhaustive.

## Technique Depth Rule

The book applies information-gathering technique. It does not teach it from scratch.

Commodity technique, meaning how to structure an interview, how to facilitate, silent generation and dot voting, is available in a hundred other books and belongs in none of these chapters. Teaching it implies the reader has no prior competence and spends budget on material that is not this book's contribution.

Governance-applied technique is different and belongs in the chapter where it does work: what to ask that surfaces a use case with no problem statement, what questions reveal that a fairness metric was chosen by whoever was in the room, how to press a vendor who is declining to answer. Give the actual questions. Do not describe that questions should be asked.

Two exceptions warrant genuine depth, because they are where standard practice fails rather than transfers.

The first is consulting stakeholders who cannot be reached. Standard methods assume a reachable participant. The people most affected by an employment screening system never interact with the deploying organization, do not know they were screened, and cannot be interviewed. Chapter 14 owes a real answer.

The second is inquiry directed at a party with an incentive not to answer. Standard methods assume cooperation. Vendor due diligence is adversarial and the approach requires modification, not application. Chapter 16 carries this.

Appendix A provides a compact reference and a short further reading note for readers lacking the base. A pointer, not a course.

## Figure Integration

Every figure requires four elements in order: setup of one or two sentences telling the reader what to look for; the figure, captioned to identify rather than summarize; a walkthrough paragraph reading the figure aloud from a specific starting point; and an application passage on how it changes in a different context. A figure with only a caption is a defect.

## Figure Completeness Specification

**A figure title does not constrain figure content.** The prior edition shipped figures that omitted stages and components, and the omissions were invisible because nothing recorded what the figure was supposed to contain. Titles alone cannot be audited.

Before any figure is drawn, write a required-elements list for it: every stage, component, actor, boundary, and relationship that must appear, plus anything deliberately excluded and why. The list goes in the manuscript source as a comment adjacent to the figure reference, so it travels with the figure and survives revision.

Three rules follow.

Completeness is checked against the list, not against the drawing. Review the list against the chapter prose first and confirm it is complete, then check the drawing against the list. Reviewing a drawing directly invites confirmation that what is present is correct while missing what is absent, which is the failure mode that produced the prior defects.

Any element the surrounding prose discusses must appear in the figure or the figure must state why it does not. A process diagram that omits a stage the text explains is worse than no diagram, because the reader trusts the picture over the paragraph.

Figures showing a lifecycle, process, or flow must show entry and exit conditions, not only the stages between them. Figures showing an architecture must show trust boundaries. Figures showing roles must show handoffs. These are the elements most often dropped.

**Standing audit.** Each figure is verified twice: once against its required-elements list, and once by a reviewer who has read the chapter but not seen the list, who is asked what they expected to see and did not. Record both checks. A figure that has not passed both is not finished.

## Sourcing and Accuracy

Every factual claim traces to project materials or a credible public source: regulators and standards bodies, primary legal texts and official journals, government publications, the OECD, peer-reviewed research. Vendor marketing and consultancy posts are not sources of fact.

Prefer descriptive over assertive framing where a standard's force is interpretive. Write that ISO 42001 provides a management system framework addressing certain topics, not that it requires a specific practice, unless quoting.

Hypothetical scenarios must be identifiable as hypothetical. Never attach a real organization's name to an invented scenario.

Regulatory content ages fast. Verify every date, instrument number, and threshold against a current source before publication. Maintain the open verification list in Part E.

## Chapter Template

**Opening.** Two or three paragraphs establishing why the chapter matters, as narrative. Do not write "this chapter will cover." Show a problem and make the reader want the answer.

**What you will be able to do.** Four to six capability statements. "Classify an AI system against the risk tiers of applicable regimes," not "understand risk classification."

**Body sections.** Per outline.

**Case in Focus.** At least one per chapter, from the running cases or a documented real case. Context, what happened, which control failed or was absent, what would have changed the outcome. 400 to 700 words. Real cases sourced and not embellished.

**Chapter summary.** Prose. Three to five paragraphs recapitulating the argument, not listing topics.

**Review questions.** Exactly seven, labeled: two comprehension, two applied scenario, one spot-the-risk with multiple embedded defects, one compare-and-decide between defensible options, one using a running case.

**Bridge.** One paragraph connecting to the next chapter through the argument.

**Change log.** Drafting artifact. Strip before publication.

---

# PART C: RUNNING CASES

Three hypothetical cases recur throughout. They are not confined to particular chapters. Every chapter touches at least one, and they develop across the book so a reader following them sees a full arc. All are explicitly hypothetical and identified as such on first appearance in each chapter.

## MedAssist

**System.** A clinical deterioration prediction tool integrated into the electronic health record at Northfield Health, a hypothetical regional network operating one academic medical center and six community hospitals. Scores admitted patients hourly for sepsis risk and alerts nursing staff.

**Development.** Built internally using ten years of the academic medical center's records.

**Carries.** Data representativeness and the gap between training and deployment settings. Delayed and ambiguous ground truth, since a prevented deterioration is invisible. Alert fatigue and automation bias. Human oversight where the human is a nurse with eleven other patients. Sector regulation including HIPAA and medical device pathways.

**Arc.** Introduced in Chapter 3 at inventory and classification. Data problems surface in Chapter 5. Chapter 9 reveals the community hospital performance gap. Chapter 10 handles the resulting incident. Extended in Chapter 11 when Northfield adds a generative clinical documentation assistant, which also carries the model selection material in Chapter 6.

## FairLend

**System.** A consumer credit risk model at Meridian Financial, a hypothetical mid-size bank operating in the United States and European Union. Scores personal loan applications and sets approval and pricing.

**Development.** Built internally, replacing a logistic regression model governed for a decade under an existing model risk management function.

**Carries.** The incompatibility of fairness definitions and the fact that choosing among them is a values decision. Proxy discrimination without protected attributes as inputs. Threshold setting and error-type tradeoffs. Explanation obligations and adverse action notices. What happens when a new governance function meets an entrenched one with real authority. Annex III classification, ECOA, FCRA, GDPR Article 22.

**Arc.** Introduced in Chapter 1 to make harm concrete. Fairness metric selection worked in full in Chapter 7. Explanation and contestation in Chapters 8 and 15. Institutional conflict with model risk management runs through Chapter 13.

## TalentScreen

**System.** A resume screening and candidate ranking tool licensed from a vendor by Calloway Industries, a hypothetical manufacturer with 14,000 employees hiring across the United States and Europe. The vendor also supplies automated scheduling and candidate communication.

**Development.** Purchased. Calloway has no visibility into training data or architecture.

**Carries.** Vendor due diligence and what to do when a vendor declines. Liability that does not transfer with the purchase. Bias audit mechanics. Transparency to applicants who do not know they were screened. Scope creep as the tool is extended to new job families without revalidation. The buy path throughout Part II. Annex III employment classification, Title VII disparate impact, jurisdiction-specific audit and notice requirements.

**Arc.** Introduced in Chapter 2 as the regulatory example with the densest overlapping obligations. Carries the buy path through every Part II chapter. Due diligence worked in full in Chapter 16. Extended in Chapter 12 when the scheduling capability becomes agentic and begins rejecting candidates without human review.

---

# PART D: CHAPTER OUTLINES

## PART I: FOUNDATIONS

---

### Chapter 1: What AI Governance Actually Is
**Target: 5,000 words**

**Purpose.** Establish why AI needs governance distinct from existing IT and risk practice, and make the stakes concrete before any framework appears.

**Capabilities.** Distinguish AI from traditional software in terms that determine governance treatment. Explain why learned behavior creates problems programmed behavior does not. Identify harms across five levels and name a real instance of each. Explain what a principle commits an organization to and what it does not.

**Sections.**

*Defining AI for governance purposes.* Work the NIST and EU AI Act definitions to extract the operative element, which is inference rather than specification. Give a usable scope test, then work three boundary cases including a hybrid rules-plus-model system, so the test is shown to be hard rather than clean.

*How machine learning actually works.* Enough mechanism that a non-technical reader can reason about governance implications. Supervised learning worked concretely through a fraud model. Then three consequences: patterns learned from data carry the data's history, learned behavior resists explanation, and performance decays without anyone changing anything.

*Generative and predictive systems.* Introduce all three system classes here, including agentic, so the reader knows from the first chapter that the book covers them. Hallucination explained mechanically, as a property of a system with no representation of truth.

*Narrow AI and the AGI distraction.* Brief. Deployed systems are narrow, general intelligence does not exist, and discussions redirected toward speculative capability are usually being redirected away from present harm. Do not editorialize further.

*AI as socio-technical systems.* The most important framing in the chapter. A model does not deny a loan; an institution does, using a model, within a process, under incentives. Develop with FairLend.

*Why AI requires specialized governance.* Five characteristics as full prose subsections: complexity and opacity, autonomy and speed, data dependency, probabilistic output, emergent behavior. Each contrasts explicitly against traditional software.

*The harms AI can cause.* Five levels with a real, sourced instance at each: individual, group, organizational, societal, environmental. Detroit facial recognition wrongful arrest for individual harm. Documented healthcare algorithm and recidivism findings for group harm.

*Principles of responsible AI.* Six principles as commitments with operational consequences and internal tension, not aspirations. Fairness gets the most space and sets up Chapter 7.

**Explain, do not name.** Supervised against unsupervised against reinforcement learning. Hallucination mechanism. Calibration. Model drift. Emergent behavior with a concrete example.

**Case.** FairLend for socio-technical framing. Case in focus: the Detroit wrongful arrest.

**Figures.** 1.1 System classes and governance implications. 1.2 Harms taxonomy with cascade paths.

**Avoid.** Opening with technology hype or a history of AI. Presenting principles as a list of nice things. Resolving the fairness tension here; open it.

---

### Chapter 2: The Regulatory Landscape
**Target: 7,000 words**

**Purpose.** Give a working map of obligations and, more importantly, teach that the map changes and that programs built on a fixed calendar fail.

**Capabilities.** Identify which regimes apply to a described system. Explain what Article 22 restricts and permits. Explain how conformity is demonstrated under the EU AI Act and why the standards machinery matters. Describe the current US position without overstating its stability.

**Sections.**

*Privacy law and AI.* GDPR lawful bases with the legitimate interests assessment worked concretely. Data minimization against AI's appetite for data as a real and unresolved tension. Purpose limitation and further processing. Data subject rights with AI-specific complications, particularly that erasure from a source system does not remove influence from trained parameters.

*Article 22 in depth.* Three elements developed separately: solely automated, significant effect, and the exceptions with required safeguards. Work the meaningful-human-involvement question with specific indicators on both sides. Use FairLend.

*US privacy.* Sectoral federal law and the state patchwork. FCRA warrants real treatment because adverse action obligations bite directly.

*Anti-discrimination law.* Disparate treatment and disparate impact distinguished carefully, with the burden-shifting framework walked through. Explain how a model with no protected attributes produces disparate impact. Vendor liability. Use TalentScreen.

*Consumer protection and product liability.* Unfairness and deception applied to AI. Model deletion as a remedy, which practitioners underestimate. Evolving product liability.

*Intellectual property.* Training data and fair use as contested rather than settled. Output copyrightability. Trade secret protection.

*The EU AI Act.* Risk tiers, prohibited practices, high-risk obligations developed individually, general purpose model obligations, provider against deployer allocation.

*The Digital Omnibus amendments.* Use Chapter_02_Regulatory_Patch.md. The teaching point is not the new dates. It is that the deadline moved because the standards machinery was not ready, that some obligations moved and others did not, and that both over-committing to the original date and abandoning preparation on news of delay were errors sharing a root.

*Conformity assessment and harmonized standards.* Use the patch. Internal against third-party assessment, notified bodies, presumption of conformity, declaration of conformity, CE marking, registration. This section makes the Act operational rather than abstract.

*US federal policy and preemption.* Use the patch. Present the contest factually without political characterization. State law binds until preempted.

*State law.* Two tracks: algorithmic discrimination in consequential decisions, and frontier model development. They reach different parties.

*Standards.* OECD principles briefly. NIST AI RMF with all four functions developed and their actual outcomes, not a one-line gloss each.

The ISO treatment must be substantially wider than 42001 alone. The SC 42 catalogue passed thirty-five published standards, and 2025 added six that closed the assurance gaps around 42001: ISO/IEC 42005 on AI system impact assessment, 42006 on requirements for bodies auditing and certifying AI management systems, 42007 on conformity assessment schemes, 12792 on transparency taxonomy, TS 6254 on explainability, and TR 20226 on environmental sustainability. 42005 matters most for this book because it addresses impact assessment directly and bears on Chapter 14. 42006 matters because it is what makes certification against 42001 mean something. Verify publication status and dates before asserting them.

*Why ISO 42001 is not the AI Act compliance route.* Teach this explicitly, because the common assumption is wrong and the correction carries a conceptual point the book needs. CEN-CENELEC JTC 21 has stated that ISO/IEC 42001 does not cover all quality management requirements of the AI Act, and prEN 18286, a European quality management system standard drafted for AI Act regulatory purposes, is intended to fulfil the complete set. The reason is not coverage but subject: 42001 manages risk to the organization, while the AI Act's Article 9 framing manages risk to persons external to the provider. Those are different accountability structures and no annex mapping bridges them. This is the socio-technical argument from Chapter 1 reappearing as a concrete standards problem, and it is the sharpest available illustration that governance frameworks are not interchangeable.

*Why the standards machinery caused the delay.* CEN-CENELEC accelerated its process in late 2025, permitting direct publication after a positive Enquiry vote without a separate Formal Vote, to make standards available by late 2026. That acceleration and the Digital Omnibus deferral are the same story told from two sides, and telling both makes the Chapter 18 argument about compliance calendars concrete rather than abstract. Verify current status, since harmonized standards cited in the Official Journal would materially change this section.

**Explain, do not name.** Legitimate interests assessment. DPIA. Presumption of conformity. Notified body. Adverse action notice.

**Case.** TalentScreen for overlapping obligations. Case in focus: an enforcement action requiring model deletion.

**Figures.** 2.1 Regime applicability decision flow. 2.2 NIST AI RMF functions. 2.3 EU AI Act obligation timeline as amended.

**Avoid.** Writing a legal treatise. Presenting the timeline as settled. Characterizing political positions.

---

### Chapter 3: Scoping, Inventory, and Risk Classification
**Target: 4,500 words**

**Purpose.** Where every real program starts and where most are already failing.

**Capabilities.** Distinguish the three lifecycle layers. Apply a boundary judgment to a system with an embedded AI component. Specify the fields two linked inventory records must contain. Design a discovery approach for unsanctioned use. Classify once and map to multiple regimes.

**Sections.**

*Three nested lifecycles.* Place first. The model layer runs train, validate, version, retrain, deprecate. The system layer runs scope, design, integrate, deploy, operate, retire, and contains one or more models together with retrieval, tools, interfaces, and guardrails. The use case layer is the business process served. Different cadences, different owners. One model serves several systems. One system swaps models without changing what it does. A use case outlives both. Establish that Part II governs the system layer, Chapter 6 addresses the model layer, and Chapter 4 addresses the use case layer.

*Where the governance boundary falls.* Chapter 1 supplied a test for whether something is AI. The harder question is where the boundary falls when a largely conventional system has an AI component inside it. Teach it as a boundary judgment, not a binary. The component is in scope intensively. The surrounding system is in scope where it shapes the component's inputs or is shaped by its outputs. Work the disputes: a vendor product with an undisclosed model component, a spreadsheet with a regression, a workflow calling a general purpose API, a fine-tuned model, a purchased model behind an interface.

*Building an inventory.* Every regime assumes you know what you have. Specify two linked record types, because one record cannot serve both purposes. The system record captures identifier, owner, purpose, decision type, populations affected, deployment context, classification, applicable regimes, evidence location, review date. The model record captures identifier, provenance, developer, version, training data summary where known, documented limitations, and inherited developer policies. The link is what matters: without it a defect found in a model cannot propagate to every system deploying it. Explain each field by naming what breaks in its absence.

*Discovering shadow AI.* Unsanctioned use of external models with organizational data is the most common live governance problem and is absent from most treatments. Network and expense visibility, self-attestation with amnesty, platform telemetry. The cultural point matters: discovery designed as enforcement produces concealment.

*Risk classification schemes.* Build a workable internal scheme. Explain the driving factors. Classify all three running cases with reasoning, including at least one genuinely arguable call.

*Classify once, map to many.* One classification exercise feeding a mapping table to obligations under each applicable regime. Show the table.

*Scoping decisions and their consequences.* What follows from classifying too narrowly and too broadly. Both fail, differently.

**Explain, do not name.** The three layers. Boundary judgment. Both record types and the link. Shadow AI. Classification factors. Mapping table structure.

**Case.** All three classified with reasoning shown.

**Figures.** 3.1 Three lifecycle layers with their cadences. 3.2 Classification-to-obligation mapping table.

**Avoid.** Restating the lifecycle; Part II does that. Presenting classification as objective.

---

## PART II: THE AI SYSTEM LIFECYCLE

**Applies to every chapter in this part:** the three-system-class coverage rule and the build-and-buy path rule from Part B. Verify both before considering any chapter finished.

---

### Chapter 4: Defining the Problem and Use Case
**Target: 5,000 words**

**Purpose.** Establish that most governance failures originate before any system exists.

**Capabilities.** Convert a proposed solution into a problem statement with success criteria. Run a root cause analysis to useful depth. Identify affected parties beyond the obvious. Recommend against building. Distinguish what the lifecycle demands on the build path from what it demands on the buy path.

**Sections.**

*Intake.* What an intake process captures and why each item earns its place. Give the actual intake questions. The Chapter 3 system record begins here.

*Problem statements.* The discipline of refusing to accept a solution as a problem. Give a weak framing and a strong one for the same situation and show what the strong framing makes possible, including rejecting the AI solution on its own terms.

*Root cause analysis.* Work the missed-appointment example to five levels and show that most branches do not terminate in AI. The strongest argument in the book that governance creates value rather than friction.

*Identifying who is affected.* Users, subjects, third parties, society. Subjects usually do not know they are subjects. Influence and interest as dimensions and what follows from each quadrant.

*Evaluating appropriateness.* Data sufficiency, objective specifiability including the proxy problem where a measurable target diverges from the actual goal, benefit proportionality, value alignment.

*Build, buy, or stop.* Frame stopping as a legitimate and underused outcome. Then establish the path distinction that governs the rest of Part II: the stages are the same and the work differs. On the build path, data governance means governing your training data; on the buy path, interrogating someone else's. On the build path, testing means designing the evaluation; on the buy path, evaluating the evidence supplied and deciding what to test yourself. Every subsequent chapter carries this distinction.

**Explain, do not name.** Problem statement structure. Five whys to real depth. Influence and interest analysis. Proxy objective failure. The path distinction.

**Case.** TalentScreen origin. Calloway never wrote a problem statement, and what followed.

**Figures.** 4.1 Intake and routing flow. 4.2 Stakeholder influence and interest grid.

---

### Chapter 5: Data Governance for AI
**Target: 6,000 words**

**Purpose.** Data is where most AI harm originates. Treat it accordingly, and across all three system classes rather than training data alone.

**Capabilities.** Assess data quality across named dimensions. Document provenance. Evaluate representativeness against a deployment population. Identify three bias mechanisms in a described dataset. Govern a retrieval corpus and a fine-tuning set.

**Sections.**

*What data means at each path and system class.* Open here, because a chapter that assumes training data excludes most readers. On the build path there is training data. On the buy path there is usually none, and the governable data is the fine-tuning set if any, the retrieval corpus, and what enters context at runtime. For agentic systems add the data the agent reads and writes during execution. Establish the full surface before governing any part of it.

*Why data problems compound in machine learning.* A report with bad data produces a bad report. A model with bad data learns the badness as a rule and applies it systematically.

*Quality dimensions.* Accuracy, completeness, consistency, timeliness, validity, each with what its failure produces in a trained model specifically.

*Provenance and lineage.* Source, collection circumstances, transformations, permissions, and how each affects what the model learns. Cleaning that removes outliers removes legitimate rare cases.

*Representativeness.* The gap between training population and deployment population. Work MedAssist in full: academic center training, community hospital deployment, different equipment, patient mix, and documentation practice.

*Bias mechanisms.* Three mechanisms taught separately because they require different remedies. Historical bias, where data records past discrimination. Measurement bias, where the recorded variable means something different across groups, worked through the healthcare cost proxy. Selection bias, where cases are systematically absent.

*Retrieval corpus governance.* What enters the corpus, who may see what, and the failure where retrieval surfaces material the requesting user is not entitled to. Corpus freshness and stale authority. Cross-reference Chapter 11 for the runtime dimension.

*Fine-tuning data.* Smaller sets, higher leverage. Why a few thousand examples can change behavior more than governance anticipates, and what review that warrants.

*Privacy-enhancing technologies.* Full treatment of four. Anonymization and why re-identification defeats it, with documented instances. Differential privacy including the epsilon tradeoff, real deployments, and what it does not protect against. Federated learning including gradient leakage and inference attacks on updates. Synthetic data including memorization risk and the requirement to test privacy as well as utility. Each with a when-to-use judgment.

*Documentation.* Datasheet structure with categories developed.

**Explain, do not name.** Differential privacy epsilon. Gradient inversion. Membership inference. Measurement bias distinguished from historical bias. Permission inheritance in retrieval.

**Case.** MedAssist for training data and representativeness. Northfield's documentation assistant for retrieval corpus governance.

**Figures.** 5.1 Data surface by path and system class. 5.2 Data lineage. 5.3 Bias mechanisms and their remedies.

---

### Chapter 6: Model Selection and Development
**Target: 5,500 words**

**Purpose.** The model layer. Most readers select rather than build, and selection forecloses control options and imports another organization's judgments.

**Capabilities.** Compare candidate models along dimensions that determine available controls. Explain what an organization inherits when building on a model it did not train. Read a system card adversarially. Distinguish where obligation attaches across build, fine-tune, and purchase. Specify what a model bill of materials records.

**Sections.**

*Build, fine-tune, or select.* Open here rather than with architecture. Most readers are selecting. Where obligation attaches at each path and what visibility each affords. A fine-tuner inherits properties they cannot inspect and did not choose.

*Model affordances and the control surface.* The section most treatments omit. You cannot design a control for a capability you do not know exists, and teams unaware of the control surface invent worse controls, most often a human review step that automation bias hollows out. Teach the axes, not a market snapshot, because axes persist while answers turn over annually. Cover constrained and structured output, tool calling with scoped permissions, instruction hierarchy and whether system instructions resist user override, context handling, confidence and abstention signals and whether they are usable, modality, latency and cost as they bear on whether human review is feasible, and deployment options including hosted, private, and on-premises. For each axis, state what control it enables or forecloses. Do not name specific models with specific capabilities in body text; any dated comparison belongs in Appendix B.

*What you inherit from the developer.* Building on a model you did not train means inheriting a governance regime you did not write and cannot amend. Not ordinary vendor risk and without clean precedent in procurement practice. Usage policies constrain what you may build. Safety training decisions determine what your product refuses, and refusals reach your users as your behavior. Deprecation schedules force migration on someone else's timeline. Data retention and training-use terms determine whether regulated data may touch the interface, and terms differ across tiers in ways organizations discover late. Published safety frameworks determine which safeguards ship. System cards determine what you can claim to know. Governance inputs to be assessed, not boilerplate to be accepted. Cross-reference Chapter 16 for the contractual dimension.

*Reading a system card adversarially.* Structure of a card at the model layer, then the reading discipline: what is omitted, what a vague evaluation section signals, which claims disclosed testing supports and which it does not, and what questions a thin card generates before selection. Coordinate with Chapter 15, which teaches the same discipline for cards the organization produces.

*Architecture and its governance consequences.* Accuracy against interpretability as a real tradeoff, with the burden on complexity. Applies to the build path and to architecture layered around a selected model.

*Interpretability and post-hoc explanation.* Intrinsically interpretable models against post-hoc techniques. What SHAP and LIME actually compute, and that a plausible explanation may not be a faithful one.

*Version control and reproducibility.* What must be reproducible and why. A model that cannot be reproduced cannot be investigated. For selected models the analogous discipline is pinning versions and demonstrating which version produced which output.

*Provenance and model bills of materials.* Base model, weights, data, adapters, dependencies. Populates the Chapter 3 model record.

**Explain, do not name.** Each affordance axis and the control it enables. Instruction hierarchy. Inherited developer policy as governance input. Adversarial system card reading. SHAP. LIME. Faithfulness against plausibility. Fine-tuning against adapters against prompting. Model bill of materials.

**Case.** FairLend replacing an interpretable model with an opaque one, and what the bank gave up. MedAssist selecting a general purpose model for the documentation assistant, including which developer policies constrain use with patient data.

**Figures.** 6.1 Affordance axes mapped to available controls. 6.2 Model supply chain layers with obligation attachment points.

**Avoid.** Tables of named models with named capabilities in body text. Claims about a developer's current terms without a sourced citation and stated date.

---

### Chapter 7: Testing, Evaluation, and Red Teaming
**Target: 7,000 words. The longest and most important chapter in Part II.**

**Purpose.** Teach verification for systems whose behavior cannot be fully specified.

**Capabilities.** Select and justify a fairness metric. Explain why fairness definitions conflict. Design an evaluation set for a generative system. Explain benchmark contamination. Structure a red team exercise. Write a requirement for a property that resists direct specification.

**Sections.**

*Performance testing.* Metrics for classification, regression, ranking. Which metric matches which error cost. Held-out data discipline.

*Fairness testing.* The central section. Four metrics defined precisely: demographic parity, equal opportunity, equalized odds, calibration. Then the impossibility result explained so the reader understands why it holds, not merely that it does. Then the consequence: selection is a values decision requiring named accountability. Work FairLend to a decision with reasoning and dissent.

*Robustness and adversarial testing.* Distribution shift, boundary behavior, adversarial inputs, with concrete examples.

*Evaluating generative systems.* A different discipline from classifier testing and taught as such. Eval design, task decomposition, rubric construction, inter-rater reliability where humans grade.

*Benchmark contamination.* Public benchmarks leak into training data. The mechanism and the holdout discipline that survives it.

*Model as judge.* Widely used and widely misunderstood. Position bias, self-preference, verbosity bias, and correlation with human judgment that degrades exactly where it matters.

*Testing agentic systems.* Distinct from both. Testing a system that takes actions requires a sandbox with realistic tools and reversible consequences, evaluation of action sequences rather than single outputs, and deliberate probing of what the agent does when its goal conflicts with its constraints.

*Red teaming.* Structured adversarial evaluation. Scope, team composition, technique categories, documentation, and the disposition question of what happens to findings.

*Specifying the unspecifiable.* The chapter's intellectual core and what distinguishes this book. Some properties resist direct specification: "does not fabricate" cannot be verified directly. The method is decomposition into a verifiable proxy with a stated threshold and verification method, plus an explicitly documented residual naming what the proxy does not cover. Work a full example: a sentinel evaluation run before and after a work batch, weighted toward items unanswerable from provided material so correct behavior is refusal, with thresholds, rotation, and holdout. Then state plainly what it does not establish, and why treating a passed sentinel as verification of the work product is a traceability failure rather than a technical one.

State the terminal difference: for conventional software, decomposition can in principle reach zero residual. Over an open-ended input space it cannot. Verification for AI reaches a characterized and accepted residual, not a verified state. Teach that as the standard.

*Release readiness.* Integration of all results into a documented decision with named accountability. On the buy path this means deciding what to test yourself given what the vendor supplied.

**Explain, do not name.** All four fairness metrics. The impossibility result. Contamination. Judge model failure modes. Action sequence evaluation. Sentinel evaluation design. Residual characterization.

**Case.** FairLend fairness decision in full. TalentScreen bias audit on the buy path.

**Figures.** 7.1 Fairness metric comparison with conflict points. 7.2 Evaluation approach by system class. 7.3 Decomposition of an unspecifiable property.

---

### Chapter 8: Deployment and Release
**Target: 4,500 words**

**Purpose.** Separate system readiness from organizational readiness, where deployment usually fails.

**Capabilities.** Evaluate readiness across three dimensions. Detect a mismatch between validated and deployment context. Design a staged rollout. Specify rollback.

**Sections.**

*System readiness.* Technical, performance, and compliance readiness with verification for each.

*Organizational readiness.* Operational, oversight, monitoring, incident readiness. State it directly: the system is usually ready before the organization is, and deploying anyway is the most common failure at this stage.

*Context alignment.* Use case, population, environment, risk proportionality. Scope creep as the dominant mechanism, since a system validated for one purpose is extended to an adjacent one that seems similar.

*The deployment decision.* Four outcomes with documentation and named accountability. Conditions must be specific and tracked or they are not conditions.

*Progressive rollout.* Blast radius, staged expansion, halt criteria defined before launch. For agentic systems, staged expansion of permission scope rather than user population.

*Rollback.* Technical mechanisms, authority, and the requirement that rollback be tested rather than assumed. For agentic systems, rollback must address actions already taken, not only halting further ones.

**Explain, do not name.** Readiness criteria per dimension. Blast radius. Halt criteria. Permission-scope staging.

**Case.** MedAssist deployed from academic center to community hospitals. Context misalignment nobody caught.

**Figures.** 8.1 Readiness across three dimensions. 8.2 Progressive rollout with halt gates.

---

### Chapter 9: Operations and Monitoring
**Target: 5,500 words**

**Purpose.** Most risk materializes during operation, which lasts far longer than development. The chapter must monitor all three system classes, not predictive drift alone.

**Capabilities.** Design monitoring across five dimensions. Handle performance monitoring when ground truth is delayed or unavailable. Monitor a generative system with no ground truth. Monitor agent actions. Detect automation bias. Specify a post-market monitoring plan.

**Sections.**

*Five monitoring dimensions.* Technical, performance, fairness, drift, usage, each with what it detects that the others miss.

*Ground truth problems.* The hard part. Delayed truth in lending, ambiguous truth in moderation, absent truth where the intervention prevents the outcome. Three approaches: sampling with human adjudication, proxy metrics with stated limitations, delayed evaluation. MedAssist is the hardest case, since a prevented deterioration leaves no trace.

*Monitoring generative output.* No ground truth at all, so monitoring shifts to rubric-based sampling, groundedness checks against retrieved sources, refusal and over-refusal rates, and user-reported failures. Explain why aggregate quality metrics conceal the failures that matter, which are rare and severe rather than common and mild.

*Monitoring agent actions.* The unit of monitoring is the action, not the output. What was done, under whose authority, with what effect, and whether it fell inside the granted scope. Detection of scope violations, unexpected tool use, and action volume anomalies. This material sits here rather than in Chapter 12 because it is operational surveillance; Chapter 12 covers the design of permissions and Chapter 15 covers log design.

*Fairness monitoring.* Disparities emerge that testing did not reveal. Disaggregated analysis on a schedule with thresholds set in advance.

*Drift.* Input drift and concept drift distinguished, with detection methods and what each triggers. Note that drift for a selected model can also come from the developer changing the model beneath you.

*Post-market monitoring plans.* A documented artifact under the EU AI Act, not merely an activity. What the plan contains.

*Human oversight in practice.* Meaningful against nominal review. Automation bias with detection signals: approval rates approaching unity, review times too short for evaluation, absence of override. Interventions when detected. Use MedAssist alert fatigue.

**Explain, do not name.** Sampling with adjudication. Groundedness checking. Over-refusal. Action scope violation. Input against concept drift. Automation bias indicators. Post-market monitoring plan contents.

**Case.** MedAssist community hospital performance gap surfaces here. TalentScreen scheduling agent action volume anomaly.

**Figures.** 9.1 Monitoring dimensions and detection targets. 9.2 Monitoring approach by system class. 9.3 Drift detection and response.

---

### Chapter 10: Incident Response and Remediation
**Target: 4,000 words**

**Purpose.** Systems fail. Response quality determines whether failure becomes catastrophe.

**Capabilities.** Classify severity. Execute a response with defined roles. Identify reporting obligations and timelines. Conduct root cause analysis reaching systemic factors.

**Sections.**

*Detection channels.* Monitoring, user reports, affected individuals, media, external researchers. Each finds what the others miss, and the channels you did not build are the ones that will find it first.

*Severity classification.* A workable scheme with criteria and the responses each tier triggers.

*Response procedures.* Notification, assessment, containment, communication, documentation. Decision authority under time pressure. For agentic systems, containment includes halting the agent and assessing actions already taken.

*Regulatory reporting.* Serious incident obligations and timelines. A compliance obligation with clocks, not a courtesy.

*Root cause analysis.* Beyond proximate cause. Ask why testing missed it, why monitoring did not catch it earlier, and why the process permitted it. Those three questions produce process improvement; the proximate cause produces only a patch.

*Post-incident review.* Findings into process change with tracked ownership.

**Explain, do not name.** Severity criteria. Serious incident definition. Systemic against proximate cause. Containment for systems that have already acted.

**Case.** MedAssist incident arising from the Chapter 9 performance gap, worked end to end.

**Figures.** 10.1 Incident response flow with decision points. 10.2 Root cause analysis to systemic factors.

---

## PART III: GOVERNING CONTENT GENERATION AND AUTONOMOUS ACTION

**Framing note for the writer.** This part concentrates controls that these two capabilities require, because those controls cohere and do not sit at a single lifecycle stage. It does not mark where generative and agentic systems enter the book. They enter in Chapter 1 and are present throughout Part II under the coverage rule. Do not write these chapters as though introducing the system classes for the first time.

---

### Chapter 11: Governing Generative Systems
**Target: 5,000 words**

**Purpose.** Generative systems break assumptions predictive governance depends on.

**Capabilities.** Explain why fabrication is structural. Design grounding and verification controls. Identify a prompt injection surface. Assess intellectual property exposure. Specify marking and disclosure. Govern prompts and retrieval as controlled artifacts.

**Sections.**

*What changes.* No ground truth for open-ended output. No enumerable input space. Output is content rather than a decision, so harm propagates differently.

*Fabrication.* Mechanism restated from Chapter 1 and developed. Why fluency and accuracy are uncorrelated and confidence signals nothing. Then the controls: retrieval grounding, citation requirements, claim-level verification, abstention design. State clearly which controls reduce and which only detect.

*Prompt injection and untrusted content.* Any system reading content it did not author has an injection surface. The mechanism, why it is not solved by input filtering, and why it compounds with retrieval and tool access. Architectural responses including privilege separation between instruction and data, output constraints, and treating retrieved content as untrusted by default. Cross-reference Chapter 12, where injection plus tool access becomes action rather than text.

*Intellectual property.* Training data exposure, output similarity, indemnification and what it actually covers, organizational policy.

*Provenance, marking, and disclosure.* Machine-readable marking obligations, watermarking and its limits, disclosure that is meaningful rather than buried.

*Prompts and system instructions as governed artifacts.* Prompts change behavior as much as retraining and are usually changed with no control at all. Version control, review, testing on change, access restriction.

*Retrieval and context governance.* What enters context at runtime, permission inheritance, and the failure where retrieval surfaces material the requesting user is not entitled to see. Cross-reference Chapter 5 for corpus governance.

**Explain, do not name.** Retrieval grounding mechanism. Abstention design. Prompt injection mechanism and why filtering fails. Privilege separation. Watermark limitations. Prompt versioning. Permission inheritance.

**Case.** MedAssist documentation assistant. Fabricated content entering a medical record is the concrete stake.

**Figures.** 11.1 Generative risk categories with control mapping. 11.2 Retrieval pipeline with governance and injection points.

---

### Chapter 12: Governing Agentic Systems
**Target: 5,000 words**

**Purpose.** When a system acts rather than recommends, the object of governance changes.

**Capabilities.** Explain why agents require different controls. Specify agent registration. Design permission scopes. Assess reversibility. Design runtime intervention.

**Sections.**

*From output to action.* The central shift. Governing a recommender asks whether the output was correct. Governing an agent asks what it did, under whose authority, and whether it can be undone. Whether a review moment survives before a given action is a design choice, not a property of acting rather than recommending; the autonomy an action class can tolerate depends on impact, scope, reversibility, observability, speed, legal duty, and how reliable recovery would be.

*Agent identity and registration.* An agent acting with credentials is an actor requiring identity. Registration record contents, and the requirement that identity be verifiable at the time of action rather than merely recorded at registration. Unregistered agents are simultaneously a governance gap and a security gap. Design registration so that it produces the identity the authority chain in Chapter 15 must record; identity that cannot be attributed to a specific action is not accountability.

*Permissions and scope.* Tool access, data access, spend limits, external communication rights, ability to invoke other agents. Least privilege applied to autonomous actors, and why default-open configurations are the common failure.

*Reversibility and blast radius.* Score actions against reversibility together with impact, scope, velocity, detectability, and legal duty; reversibility alone does not decide how much autonomy an action tolerates. Sending an external communication, moving money, and deleting data are not the same risk class and should not carry the same permission.

*Runtime intervention.* Circuit breakers, halt authority, and the tested ability to stop an agent mid-task. Intervention that exists in policy but has never been exercised does not exist.

*Multi-agent systems.* Agents invoking agents. Emergent behavior from interaction. Accountability when a chain produces an outcome no single agent decided.

**Explain, do not name.** Agent registration contents. Permission scope design. Reversibility classification. Circuit breaker mechanics.

**Case.** TalentScreen scheduling agent begins sending rejections autonomously. Nobody registered it, nobody scoped its permissions, and nobody can say how many candidates it rejected.

**Figures.** 12.1 Recommender against agent control points. 12.2 Action classification by reversibility.

**Sources.** This chapter has the thinnest established source base in the book and must not be written from first principles alone. Singapore's IMDA Model AI Governance Framework for Agentic AI, first issued January 2026 and updated May 2026, is the first dedicated governance framework for agentic systems and is organized around four dimensions: bounding risks upfront, meaningful human accountability, technical controls and processes, and end-user responsibility. It treats logging and monitoring, access controls, guardrails, and human approvals as core components of an agent, and it addresses multi-agent patterns and third-party agents directly. Verify its current version and contents before citing. Check also for NIST agent standards work and any EU guidance applying Articles 14 and 15 to autonomous systems.

**Cross-references.** Action monitoring is in Chapter 9. Action sequence and authority chain log design are in Chapter 15. Injection reaching tool access is in Chapter 11. Do not duplicate. Chapter 12 designs identity, permission, and intervention; Chapter 15 specifies what gets recorded; Chapter 9 watches it. Verify while drafting that the three fit together, since a permission Chapter 12 grants must be loggable under Chapter 15 and monitorable under Chapter 9 or it is unenforceable.

---

## PART IV: THE GOVERNANCE FUNCTION

---

### Chapter 13: Organizing the Governance Function
**Target: 5,000 words**

**Purpose.** Structure determines whether governance has authority or only opinions.

**Capabilities.** Compare three operating models against organizational context. Identify where the operating model choice recurs. Apply the three lines model to AI. Design an acceptable use policy. Navigate conflict with an incumbent function.

**Sections.**

*Operating models.* Centralized, federated, hybrid, each with what it does well, where it fails, and what conditions favor it. A genuine design decision with no default answer.

*The operating model as a recurring variable.* Not a single choice made once on an org chart. It recurs at every decision point: where the inventory lives, who classifies, who approves deployment, who holds model selection authority, who owns the vendor relationship. Organizations are often federated on some and centralized on others without having decided deliberately.

*Federated at the system layer, centralized at the model layer.* The pattern that usually works, falling directly out of the two-record inventory. Local teams own their deployments while model selection, developer terms, and provenance are held centrally, so a defect propagates once rather than being rediscovered independently.

*How federated governance fails.* Predictable failure modes worth teaching directly: classification drifts apart across units, local governance is captured by the business it serves, and nobody holds aggregate visibility, which is fatal because most regulatory reporting is organization-level.

*Roles and responsibilities.* Who owns what. RACI applied to governance decisions with a worked example.

*The three lines model.* Fully explained in AI terms rather than referenced. First line owns and manages, second provides oversight and expertise, third provides independent assurance. Name which functions occupy which line and what happens when lines blur.

*Governance bodies.* Composition, mandate, decision rights, escalation. A committee without decision rights is a discussion group.

*Acceptable use and sanctioned tooling.* The practical response to shadow AI. Prohibition alone produces concealment; the workable approach pairs restriction with a sanctioned path genuinely easier than the workaround.

*Conflict with incumbent functions.* Where a model risk management function already exists with real authority, a new AI governance function arrives as a competitor. Address the boundary directly: the incumbent typically owns validation and monitoring and has no mandate over problem definition, use case appropriateness, or affected-party requirements, which is where failures concentrate.

*Executive and board engagement.* What boards need, what questions they should ask, what reporting supports oversight.

**Explain, do not name.** Three lines with AI-specific occupants. Decision rights. The layer-split pattern. Federated failure modes. Sanctioned tooling.

**Case.** FairLend, where AI governance meets an entrenched model risk function.

**Figures.** Converted to native tables during the CH zero-trust review. Table 13.1 is the decision-rights matrix and Table 13.2 is the operating-model comparison, following this book's practice of using a table rather than a diagram for a comparison or scoring structure. The original `fig-13-01-operating-models.svg` and `fig-13-02-layer-decisions.svg` are retired and must not be built into the published book.

---

### Chapter 14: Risk Assessment and Management
**Target: 5,000 words**

**Purpose.** Structure risk work, solve the one information problem standard practice cannot, and carry assessment through to control selection and acceptance.

**Capabilities.** Structure an impact assessment. Consult stakeholders who cannot be reached. Score and prioritize risks without false precision. Select controls proportionate to assessed risk. Document residual risk acceptance. Identify what changes trigger reassessment.

**Sections.**

*Assessment structure.* Five components: system description, risk identification across categories, mitigation, residual risk, and a documented decision with named accountability. Establish the risk categories used throughout assessment, drawing on the harms taxonomy from Chapter 1 and the classification factors from Chapter 3 rather than introducing a third scheme. Note briefly how assessment differs across the three system classes: predictive assessment centers on error and disparity, generative on content and misuse, agentic on action and scope.

*Consulting absent and unreachable stakeholders.* The section that earns the chapter. Standard methods assume a reachable participant. The people most affected by an employment screening system never interact with the deploying organization, do not know they were screened, and cannot be interviewed. Give real approaches: proxy consultation through advocacy organizations and representative bodies, evidence from complaint and appeal records, published research on comparable systems and populations, structured adversarial review where someone is assigned to argue the affected party's interest, and outcome analysis after deployment as partial substitute for consultation before it. Be honest about what each substitutes for and what it cannot recover. A genuine methodological gap, not a solved problem, and presented as such.

*Risk scoring and prioritization.* Likelihood and severity without false precision. Prioritization forcing explicit tradeoffs. What to say when every stakeholder insists everything is critical.

*Mitigation planning and control selection.* Where assessment becomes action, and the step most often skipped. For each significant risk, what control addresses it, whether the control is technical, procedural, or contractual, who owns it, and how its effectiveness will be verified. Teach the distinction between controls that reduce a risk and controls that only detect it, since organizations routinely credit detection as though it were prevention. Test each proposed control against feasibility, including the cost constraint developed in Chapter 17. A control nobody can afford to operate will lapse while the documentation continues to claim it.

*Residual risk acceptance.* Who accepts, on what basis, documented how. Unaccepted residual risk is an unowned liability. Connect to Chapter 7: where a control verifies something narrower than the requirement it serves, the gap belongs here as characterized residual rather than disappearing.

*Reassessment triggers.* Assessment is not a one-time artifact. Define what changes require it to be redone: material change to the model or its version, extension to a new population or use case, a regulatory change affecting classification, an incident, and elapsed time regardless of change. Without defined triggers, assessments age silently and the organization governs a system that no longer exists.

**Explain, do not name.** Proxy consultation. Structured adversarial review. Reducing controls against detecting controls. Residual acceptance authority. Reassessment triggers.

**Case.** TalentScreen. The applicants Calloway never consulted and could not have interviewed, and the reassessment that never happened when the tool was extended to a second job family.

**Figures.** 14.1 Assessment process flow. 14.2 Risk scoring with prioritization. 14.3 Reassessment trigger matrix.

**Avoid.** Teaching interview or workshop technique. See the technique depth rule in Part B. Applied questions belong in Chapters 4 and 16.

---

### Chapter 15: Documentation and Evidence
**Target: 4,500 words**

**Purpose.** Governance needs both substantive performance and reliable evidence of it. Missing required records can create a separate compliance failure of their own, regardless of whether the underlying practice was sound.

**Capabilities.** Write a requirement specific enough to test. Build a traceability matrix. Read and evaluate a model card. Specify logging sufficient to reconstruct a decision or an action.

**Sections.**

*Writing requirements.* Identifier, statement, source, priority, acceptance criteria, status. The testability standard, with weak and strong versions of the same requirement compared.

*Traceability.* What the matrix connects and the questions it answers. Show an actual matrix with real rows. Connect back to Chapter 7: a control verifying something narrower than its requirement must record that gap, or the organization will mistake the control for the assurance.

*Model cards.* A non-exhaustive five-category core (intended use, training data, performance and evaluation, limitations, maintenance), with the fuller original framework's additional categories named. Then teach reading one adversarially: an omission or a vague section is an unresolved evidence request, not proof of a concealed result. Coordinate with Chapter 6, which applies this to selection.

*Audit trails and logging.* What must be captured to reconstruct a decision months later under challenge. Retention against privacy tension.

For agentic systems this is a materially harder problem and warrants its own treatment. Two things must be reconstructable and they are not the same. The action sequence records the observable state available to the agent, its inputs, retrieved context, and prior tool results, and what it invoked, not any claim about internal reasoning. The authority chain records under what authorization it acted: which principal granted the permission, which registered agent identity was used, whether a supervising agent delegated to a subordinate one, and what scope was in force at the moment of the action rather than at registration. How that authorization evidence is represented (a policy-decision record, a credential, a token) depends on the architecture; do not present one implementation pattern as a universal requirement. A complete chain establishes who was authorized to act; establishing who is accountable is a separate step, mapping the chain back to the human and organizational roles Chapter 13 defines. Multi-agent architectures make this acute, since the chain from a human principal to the acting agent may run several hops and each hop must be recorded or the chain breaks at that point.

This connects Chapter 12 to Chapter 9. Registration in Chapter 12 creates the identity; the authority chain here is what records that identity in use; Chapter 9 monitors actions against granted scope and can only do so if this data exists. Specify the log design so that the monitoring Chapter 9 requires is actually possible.

*Evidence for regulators.* What demonstrable compliance requires and how it differs from believing you comply.

*Automation.* Generating documentation from development artifacts rather than as a separate burden.

*Versioning and deprecation.* Governance artifacts are maintained objects. A template, a taxonomy, and a threshold all age and need owners and review cycles.

**Explain, do not name.** Testability standard. Matrix structure. Adversarial card reading. Reconstruction-sufficient logging for decisions. Action sequence distinguished from authority chain. Scope in force at time of action.

**Case.** All three, tracing a shared transparency goal through three different domain-specific legal requirements (Regulation B for FairLend, New York City Local Law 144's bias-audit-and-notice duty, not an individual-explanation duty, for TalentScreen) and showing how evidence strength differs on build and buy paths.

**Figures.** 15.1 (traceability matrix) and 15.2 (model card structure) were retired 2026-09-13 in favor of native Tables 15.1 and 15.2; see `figures/archive/RETIRED-15.1-15.2-README.md`. 15.3 Authority chain from principal to acting agent in a multi-agent sequence, labelled as this book's own recommended synthesis (not a claim that a named organization implements this exact process), citing NIST SP 800-207 for the policy-decision/enforcement model and RFC 8693 only for the token-exchange variant, showing a complete path and a path broken at an unrecorded hop, and closing on a step mapping the technical chain to Chapter 13's accountability roles. SVG redraw against this spec is OPEN (CH250/CH251/CH519, Pass 29).

---

### Chapter 16: Third-Party, Vendor, and Supply Chain Governance
**Target: 5,000 words**

**Purpose.** Most organizations buy more AI than they build, and liability does not transfer with the purchase.

**Capabilities.** Structure due diligence. Conduct inquiry with a party who has reason not to answer. Evaluate vendor-supplied evidence rather than accepting it. Draft contract provisions serving governance. Assess a supply chain. Use procurement as leverage.

**Sections.**

*Due diligence as structured inquiry.* Preparation, open questions first, specific second, limitation questions last. Give the actual questions rather than describing that questions should be asked.

*Assessment dimensions.* Provider, system, documentation, compliance. What each reveals and what a weak answer signals.

*Vendor resistance.* The section practitioners need most, and the second exception under the technique depth rule. Standard inquiry assumes cooperation; this is adversarial and requires modification. Distinguish trade secret refusals from refusals of convenience. Specify what you actually need, which is rarely the algorithm and usually disaggregated performance, documented failure modes, and known limitations. State which gaps are disqualifying. Document declined questions, because the record of what a vendor would not answer is itself evidence.

*Evaluating vendor-supplied evidence.* Getting the metrics is not the same as being able to trust them. A vendor bias audit is an artifact with a chosen methodology, a chosen population, and a chosen metric, all selected by a party with an interest. Send the reader back to Chapter 7 to interrogate it: which fairness metric, on which population, against which threshold, and what would the result have been under a different choice.

*Contract provisions.* Information rights, audit rights, change notification and approval, incident cooperation, liability allocation, exit. Give example language.

*The supply chain.* A real supply chain branches and repeats rather than forming one fixed line (base model, fine-tune, adapter, integration, and deployment is one common shape, not the only one). Obligation and visibility are separate attributes, assessed layer by layer rather than assumed to move together or to decrease steadily with distance from deployment.

*Model developer policy as inherited governance.* Chapter 6 established what an organization inherits. This addresses what to do about it. Which terms are negotiable is set by each developer's own current, dated terms, not by a fixed rule this book can state once; check named terms (data retention, training use of customer inputs, support responsiveness) against the actual account's terms rather than assuming a market default by tier. How to assess deprecation risk and what migration readiness requires, since a forced migration is a revalidation event and should be budgeted as one. What to do when a usage policy prohibits a use your organization considers legitimate, and that the contract language, not a uniform rule, decides what a violation triggers. How refusal behavior is a mix of an inherited policy floor and the organization's own configuration, tested as the assembled system actually behaves, and what disclosure that warrants.

*Open-weight models.* License variation, support becoming your problem, provenance variation, and liability that depends on actor, conduct, jurisdiction, and claim rather than landing automatically on the deployer merely because there is no purchase contract. Community viability as a real dependency.

*Procurement as leverage.* Requirements in solicitation documents obtain what post-contract requests cannot, because leverage is often strongest before signature. It is not the only leverage a relationship ever has; renewal, rebids, audit findings, breach, regulatory change, and credible alternatives create real leverage after signature too, and preserving it means building audit, access, and exit rights into the contract itself.

*Ongoing management.* Performance, compliance, relationship, reassessment.

**Explain, do not name.** Specific due diligence questions. Adversarial inquiry. Interrogating a supplied bias audit. Contract clause purposes. Supply chain layers. Negotiable terms that require checking dated current terms rather than assuming a market default. Deprecation as a revalidation event. Open-weight liability as actor- and conduct-dependent.

**Case.** TalentScreen in full. Calloway's due diligence, the vendor's refusal, the decision to proceed, and what followed. A hypothetical extension of MedAssist illustrating the developer-policy assessment due diligence needs before permitting patient data near a hosted model.

**Figures and tables.** 16.1 Due diligence sequence (figure; redraw pending against the current required-elements record, see `badw-book-log.md` CH523/CH295). Supply-chain actors, visibility, and duty (native table, replaced the former Figure 16.2). Contract-tier verification checklist (native table, replaced the former Figure 16.3). Retired SVGs for the two replaced figures are kept, unreferenced, in `figures/archive/`; do not restore either without redrawing it against the chapter's current claims.

---

## PART V: BUILDING GOVERNANCE CAPABILITY

---

### Chapter 17: Implementing AI Governance
**Target: 6,000 words**

**Purpose.** Treat the governance program as something designed, built, deployed, and evaluated, using the same discipline the book applies to AI systems. Do not announce the parallel. Let the vocabulary carry it.

**Capabilities.** Assess current state. Define a target operating model. Produce a gap analysis and sequenced roadmap. Gather requirements from those who must live with the process. Design controls against a real budget. Evaluate whether governance works. Diagnose why a program is being bypassed.

**Sections.**

*Governance as something you build.* Open by treating the program as a designed thing with users, requirements, and failure modes. State without ceremony that a governance program nobody uses has failed regardless of its documentation.

*Current state assessment.* What exists, what functions, what is theater. Distinguish documented process from actual practice; the gap is the finding.

*Target operating model.* What the program should look like given size, sector, regulatory exposure, portfolio, and existing functions. Draw on Chapter 13. No universal answer, and the chapter should refuse to supply one.

*Gap analysis and sequencing.* Current to target. What must come first because other things depend on it. Inventory precedes classification, classification precedes proportionate process.

*Requirements for the governance function.* What distinguishes this chapter. Programs fail most often because nobody asked the development teams, business owners, and reviewers what they need. Apply the same discipline used on AI systems, with the governance process as the subject. Ask developers where the process obstructs. Observe what people do when the process is inconvenient.

*Designing controls, artifacts, and workflows.* Proportionate design. Where automation fits. Making the compliant path the easy path rather than relying on discipline.

*Cost as a design constraint.* Inference cost determines whether a control is viable. Human review of every output is specifiable and unaffordable at volume. Cheaper models shift the accuracy-oversight tradeoff. Rate limits shape architecture. A control designed without a cost model will be abandoned quietly, which is worse than never having specified it, because the documentation will still claim it.

*AI literacy and training.* A regulatory obligation reaching providers and deployers, not only good practice. Role-differentiated content and evidence of completion.

*Rollout and adoption.* Staged introduction, pilot selection, the same progressive-rollout logic used for systems in Chapter 8.

*Evaluating whether governance works.* The question almost no program asks. Process metrics measure activity; outcome metrics measure whether risk is managed. Are issues found before deployment or after? Are classifications accurate on review? Is the process bypassed, and by whom?

*The two-speed problem.* Close here. System cycles run in days, program cycles in quarters. That mismatch is the structural source of most governance pain and explains the bypass behavior described earlier. Responses include embedding controls into tooling, automating what is automatable, tiering by risk, and shifting weight from pre-deployment gates toward runtime controls and monitoring. Connect explicitly to Chapters 9 and 12.

**Explain, do not name.** Current against documented state. Sequencing dependencies. Cost-viability of controls. Outcome against process metrics. The two-speed mismatch.

**Case.** A composite implementation at Calloway covering all three systems, showing sequencing and one wrong call.

**Figures.** 17.1 Current to target with sequenced roadmap. 17.2 Governance cadence against development cadence.

---

### Chapter 18: Governing Under Uncertainty
**Target: 3,500 words**

**Purpose.** Replace prediction with durable method. Do not forecast.

**Capabilities.** Explain why fixed compliance calendars fail. Build a horizon-scanning practice. Design programs that survive regime change. Explain what the field asks of a professional.

**Sections.**

*Why compliance calendars fail.* Use the 2026 deferral concretely. Organizations treating the original date as immovable over-invested; organizations treating the proposed delay as settled stopped work. Both errors share a root: treating a regulatory date as a plan rather than one input to a plan.

*Horizon scanning.* Source selection, cadence, triage, and translation of a regulatory change into an internal change request against existing requirements. Regulatory change management as an operating discipline, not reading the news.

*Regime-agnostic design.* One inventory, one classification, many mappings. When a regime changes, the mapping updates and the classification survives. Connect explicitly to Chapter 3.

*What stays stable.* Beneath changing regimes, obligations converge on a small set: know what you have, assess before deploying, test for disparate effect, document, oversee, monitor, respond. A program built on these survives regime change with modest amendment.

*The profession.* What the field asks: technical literacy without technical expertise, legal literacy without legal training, judgment to distinguish real risk from theater, and standing to say no. Where the discipline is going and what remains unsettled.

*From compliance to advantage.* Brief and unsentimental. Governance preventing the wrong system from being built saves more than governance documenting the right one. Do not overclaim a business case the evidence does not support.

**Explain, do not name.** Horizon scanning cadence. Regulatory change as change request. The convergent obligation set.

**Case.** Brief return to all three. Where each stands and what remains unresolved. Do not tie a bow.

**Figures.** 18.1 Regime-agnostic mapping architecture.

---

# PART E: APPENDICES, FIGURES, AND OPEN ITEMS

## Appendix A: Technique Reference
Alphabetical. Each entry gives a short description, when to use it, and chapter cross-reference. Includes a brief further reading note for readers lacking the base in general information-gathering practice. A pointer, not a course. Approximately 2,500 words. No parent-discipline attribution.

## Appendix B: Regulatory Quick Reference
EU AI Act tiers and obligations with amended timeline. Conformity assessment routes. NIST AI RMF functions and categories. ISO 42001 clause structure. US federal and state landscape. Sector requirements. Any dated model capability comparison belongs here, clearly labeled as a snapshot. Approximately 3,000 words. Date the appendix explicitly.

## Appendix C: Templates and Checklists
AI use case documentation. System inventory record. Model inventory record. Model card. Impact assessment. Vendor assessment. Agent registration and permission scope. Incident response. Governance readiness. Approximately 2,000 words. Usable as given, not illustrative.

Under CC BY-NC these are licensed for readers to adapt, which is the main practical gain from the license change and should be stated in a short appendix preamble. It also means every template must be original work rather than derived from a published example. Write them from the requirements the chapters establish, not from existing templates in circulation.

## Appendix D: Glossary
Approximately 1,500 words. Every term explained in the body appears here. No prohibited vocabulary.

## Figure Inventory
Forty-two figures across eighteen chapters (corrected from "forty-one" by CH426, Pass 17, 2026-09-13: this file's own chapter-by-chapter list sums to 42), listed per chapter above. Every figure requires the four-element integration in Part B. **Historical planning language, superseded 2026-09-13 (CH429 of pass-17b, the control-reconciliation document): all 18 chapters and 4 appendices are now draft complete and this is no longer a placeholder-production phase. `control/PROGRESS.md` is the controlling record of each figure's current build/audit status; treat "currently placeholder references requiring production" below as describing the pre-drafting phase, not the present state.**

## Open Items Requiring Verification Before Publication

1. Colorado AI Act current effective date. Adjusted since enactment.
2. EU AI Act harmonized standards status. Whether CEN-CENELEC standards have been cited in the Official Journal materially affects Chapter 2. Track prEN 18286 specifically, along with the European AI conformity assessment framework standard.
2a. ISO SC 42 publication status for 42005, 42006, 42007, 12792, TS 6254, TR 20226, 27090 on AI cybersecurity, and 29119-11 on testing of AI systems. Confirm each from ISO directly. 42005 bears on Chapter 14, 27090 on Chapter 7 security testing, 29119-11 on Chapter 7 generally.
3. US preemption litigation status and any enacted federal AI legislation.
4. State frontier model laws taking effect January 2027 and subsequent enactments.
5. NIST agent standards work. Referenced in Chapter 12 and requires a primary source before assertion.
5a. Singapore IMDA Model AI Governance Framework for Agentic AI. Confirm current version, publication date, and contents from IMDA directly rather than from secondary commentary before citing in Chapters 2 or 12.
6. All EU AI Act penalty figures and deadlines against the consolidated text as amended.
7. Sources for every real case used in a Case in Focus.
8. Model developer usage policies, enterprise terms, retention and training-use provisions, and published safety frameworks. Cite with access dates. Assume these change between drafting and publication.
9. Any dated model capability comparison placed in Appendix B. Date it explicitly and state that it is a snapshot.

## Drafting Sequence

**Completed historical planning, not a current instruction (CH429 of pass-17b, Pass 17, 2026-09-13).** All 18 chapters and four appendices are now draft complete; nothing below directs current work. It is preserved as a record of the original sequencing decision, not as a live task list. `control/PROGRESS.md`'s "Next" section and the signed CH review ledger (`rules/badw-book-log.md`) are the controlling statement of what remains, which is verification and correction work, not drafting.

Chapters 3, 6, 7, 12, and 17 contain the most new material and carry the most weight. Draft those first.

Chapters 1, 2, 4, 5, 8, 9, 10, 13, 15, and 16 have substantial existing draft material in Chapter_01_Revised.md through Chapter_06_Revised.md that can be adapted, but all of it predates the three-system-class coverage rule and the build-and-buy path rule. Every adapted chapter must be checked against both before it is considered done. Chapter 2 requires Chapter_02_Regulatory_Patch.md applied before any other work.

Chapters 11 and 14 require the most rewriting relative to existing material: Chapter 11 gains prompt injection, and Chapter 14 loses its technique content while gaining mitigation planning and reassessment triggers.
