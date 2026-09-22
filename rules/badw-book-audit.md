# badw-book audit record

Created 2026-09-21, agent: cl. Required by `badw-book.md` section 18; named in
`README.md` as the fourth file of this folder. It did not exist before this date,
which is itself a finding: every pass logged in `badw-book-log.md` from 2026-09-12
onward ran without the audit record section 18 requires. This file opens with
Chapter 3 and is to be extended one entry per chapter worked on.

**Scope gate.** 5/5 properties present. The work teaches a practitioner to perform,
decide, and assess; its chapters are read alone as often as in sequence; it defines
constructs the reader applies to cases; it carries figures, worked cases, and
end-of-chapter questions; and it is revised as law, standards, and practice change.
`badw-book.md` is the correct suite. The parent `w/` suite is not present in this
repository and does not govern this work.

---

## Standing finding, all chapters

**A18-001. The audit record was absent for passes 1 through 56.** Section 18 requires
the record for every chapter worked on. Fifty-six-plus passes are logged in
`badw-book-log.md` with per-finding dispositions, but no audit record was created, so
the section 7 uniformity signals were never dispositioned in the place the rules
require. Section 7 states that a coefficient of variation below about 0.45 is a
mandatory review signal to be "resolved or justified in the audit." Three files
currently sit below that line with no recorded justification.

**Disposition.** OPEN. This file closes the requirement for Chapter 3 only.
Chapters 1, 2, and 4 through 18 and Appendices A through D remain without an audit
entry. Measurements for all of them are recorded under "Portfolio measurements"
below so that the outstanding work is bounded and visible rather than merely noted.

**A18-002. Nominalisation is over the section 7 threshold book-wide.** Section 7 sets
roughly five percent of words ending -tion, -ment, -ance, -ity, -ness. The book runs
5.7 percent overall, with fifteen of twenty-three files above the line. Chapter 13 at
7.6 percent and Chapter 12 at 7.3 percent are prose and should come down. Appendices
B, C, and D are structurally list-heavy and the excess is inherent to the form.

**Disposition.** OPEN for Chapters 12 and 13. JUSTIFIED for Appendices B, C, and D:
a glossary, a quick reference, and a template set are noun-phrase artifacts by
construction, and rewriting them to verbs would damage their function as lookup
documents. Recorded here rather than left as an unexplained warning.

**A18-003. Three files sit below the sentence-length CV signal.** Chapter 13 at 0.44,
Appendix B at 0.38, Appendix D at 0.31.

**Disposition.** JUSTIFIED for Appendices B and D. A regulatory quick reference and a
glossary are entry-per-item forms; uniform entry length is the form working, not a
template controlling the prose. OPEN for Chapter 13, which is continuous prose at
0.44 and marginal. To be inspected for a controlling template when Chapter 13 is next
worked.

---

## Chapter 3. Scoping, Inventory, and Risk Classification

**Version worked.** `chapters/03-scoping-inventory-classification.qmd`, 8,137 words,
as at 2026-09-21.

**Rule files loaded.** `rules/README.md` and `rules/badw-book.md`, both as at
2026-09-12; `rules/badw-book-log.md` as at 2026-09-15;
`control/BOOK_SPECIFICATION_v2.md` Prohibited and Permitted Vocabulary, section as at
2026-09-12; `control/SOURCES_AND_ATTRIBUTION.md` as at 2026-08-29.

**Central claim.** An organization cannot govern what it has not recorded, and the
record is produced by three judgments the chapter teaches: which lifecycle layer a
question belongs to, where the governance boundary falls, and what the system's risk
classification is, held separate from what any regulation independently requires.

**What the reader can do afterwards.** The six objectives at the chapter opening.
Each is a performable act, not a comprehension check.

**The seven-line spine.**

1. Three lifecycles run at different speeds with different owners, and a question
   asked at the wrong layer is answered wrongly.
2. The governance boundary is a materiality judgment, not a technical input-output
   test, and it is a property of the deployment rather than of the software.
3. Two linked record types are needed, because one model serves many systems and one
   system calls many models.
4. Three fields carry most of the weight and are the ones most often filled badly.
5. What the inventory does not contain is not a random sample, so discovery must be
   designed rather than requested.
6. Risk classification is four factors that behave differently across the three
   system classes.
7. The internal tier is an operating decision; legal applicability is decided by each
   regulation's own trigger, tested independently.

**Paragraph-role map.** Recorded at section granularity. 3.1 establishes and figures;
3.2 establishes, defines, and works three dependency cases; 3.3 defines and
enumerates with failure consequences; 3.4 defines, argues the non-random property,
and pays off in the Case in Focus; 3.5 supplies vocabulary; 3.6 establishes four
factors and varies them across classes; 3.7 separates two questions and figures the
separation; 3.8 consolidates to consequence and hands off to Chapter 4.

**Promise ledger.**

| Promise | Paid off |
|---|---|
| Six objectives at chapter opening | 3.1 through 3.7 respectively; all six discharged in-chapter |
| "Chapter 12 returns to this system" (3.4 case) | Chapter 12, agentic scope and permission |
| "Chapter 16 examines the due diligence that preceded the purchase" (3.4 case) | Chapter 16, vendor assessment |
| System-to-model link (3.3) | Chapter 10 root cause analysis uses it to confirm model version; Chapter 15 turns it into evidence |
| Classify once, map to many (3.7) | Chapter 18 section 18.3 regulation-agnostic mapping |

**Source ledger.** The chapter makes no legal, standards, or case claim requiring
external sourcing. The OECD classification framework in 3.5 is described, not
reproduced, per `SOURCES_AND_ATTRIBUTION.md` Tier 1. The Calloway case is marked
hypothetical in its own first line. No check date applies because no external claim
is asserted.

**Gate commands run, 2026-09-21.** Measurement script over the chapter with code
blocks, tables, figure lines, and headings stripped.

```
sentences        452   (445 before the template pointers; 449 at first insertion,
                       452 after the three were rewritten to fix the faults in A18-005)
mean length      18.0 words
CV               0.592  (signal if <0.45)  PASS
The/This start   24%    (signal if >25%)   PASS, 1 point under
nominalisation   4.4%   (signal if >5%)    PASS
em dashes        0                          PASS
en dashes        0                          PASS
sentences >45w   2
```

Prohibited vocabulary scan against `BOOK_SPECIFICATION_v2.md`: zero occurrences.
Section 6 fluff list, fourteen phrases: zero occurrences.

**A18-005. A check was reported at a depth it had not been run to.** On 2026-09-21
this entry recorded Chapter 3 as passing after section 7's mechanical measurements
were run. Section 0's five-pass revision protocol had not been run, and the mandatory
neighbour-set check in section 7 had not been applied to the three sentences added to
sections 3.2, 3.4, and 3.7 the same day. Section 14 states that a recommendation is
not a state, and section 18 states that no audit statement may claim a check that was
not actually performed. The original statement did.

**Disposition.** FIXED, and recorded rather than overwritten. The protocol was run on
2026-09-21 after the omission was raised by the author. It found three faults in the
added sentences that the mechanical gates had passed: a colon subordinating a list in
3.4, against the standing colon rule in section 5; a repeated rhetorical frame across
all three additions, every one opening "Appendix C template N" with a verb and two
using the same verb, against section 7; and a broken inherited referent in 3.4, where
"the second list" named a structure visible only inside the drafting sentence and not
in anything the reader had read. The third is the material one. It is the fault class
the mechanical gates cannot see, and it is the reason section 7 makes the
neighbour-set check mandatory rather than advisory. All three fixed the same day and
re-measured.

**Standing consequence.** A mechanical pass is not an audit entry. Any future entry
claiming a chapter passes must state which of the five passes were run and confirm
the neighbour-set check on every sentence added or revised in that pass.

**Text state.** sha256 7db7ee992368c36f (first 16), 8,282 words, after the A18-005
and A18-008 fixes. Every gate figure in this entry was measured against this state.
An edit to this chapter invalidates the block above; mechanical counts may be re-run
on the changed region, and the neighbour-set check may not inherit.

**Passes actually run, per section 18a.** Section 0's pass 2 (bottom-up, sentence
level) and pass 4 (defensive language) were run, together with the mandatory
neighbour-set check on every sentence added or revised this date. Pass 1, pass 3, and
pass 5 were NOT RUN. This entry therefore does not certify the chapter's structure,
paragraph flow after surgery, or cold-reader clarity. It certifies the mechanical
gates and the sentence-level work on the edited passages only.

**Separation of duties.** Not satisfied. The same agent (cl) drafted the three added
sentences, found the faults, applied the fixes, and recorded this entry. Section 18a
requires that where one agent does both, the entry names the order and states that
the check was re-run against the original finding wording. It was: each of the three
faults was re-checked against its own original sentence, not against the replacement.
Recorded as a known weakness of this entry rather than presented as compliance.

**Unresolved warnings.** None for this chapter on the checks that were run. The 24 percent "The/This" figure sits
one point below the signal threshold and is recorded because it is close, not because
it fails. Noted for re-measurement if the chapter is revised.

**Sentences retained above 45 words.** Two.

- 110 words: the six-item objectives list, counted as one sentence by the measurement
  script because the list items are not terminated. This is an instrument artifact,
  not a sentence. Section 14's rule that an extraordinary result impugns the
  instrument first applies. No action.
- 52 words: "One model may appear in many system records, and one system record may
  reference several models." with its surrounding clause. Retained. Splitting would
  break the many-to-many relation, which is the definition's operative content and
  loses its symmetry when divided.

**Term dispositions.** "AI system lifecycle" is used in full form throughout, per the
naming rule; the short form appears twice as reported usage immediately corrected,
which the specification sanctions explicitly for Chapter 3. "Shadow AI," "system
record," and "model record" are the chapter's own constructs and recur with their
defined meaning at each instance. No reflexive instance recorded.

**Artifact obligations.** Sections 3.2, 3.4, and 3.6/3.7 establish requirements that
Appendix C did not satisfy. Three templates added 2026-09-21 as templates 10, 11, and
12; see the Appendix C entry below. Appendix C's preamble promises that every field
is cross-referenced to the section establishing it, but nothing verified the reverse
direction, that every section establishing a record has a template. That reverse
check is now recorded as a standing obligation.

**Final statement.** Quotations, citations, numbers, dates, figures, and tables in
Chapter 3 were checked against their sources on 2026-09-21. The chapter asserts no
external legal or standards claim; the two figures were confirmed present and
correctly referenced; the Calloway figures (14,000 employees, two believed, eleven
found, six weeks, eighteen months, four days) are internally consistent across
section 3.4 and the end-of-chapter case and are hypothetical by declaration.

---

## Appendix C. Templates and Checklists

**Entry opened 2026-09-21** for the three templates added this date. A full audit
entry for Appendix C is outstanding.

**A18-004. Chapter 3 established three records Appendix C did not carry.** Section
3.2's boundary judgment had no artifact; the System Inventory Record has no field for
what was excluded or why. Section 3.4's discovery method had no artifact; template 2
records a found system and template 9 references the sweep, but nothing records which
channels were searched, which were not, and therefore what the residual blind spot
is. Sections 3.6 and 3.7's two independent questions were compressed into two
adjacent fields on template 2, which invites the collapse section 3.7 exists to
prevent.

**Disposition.** FIXED. Templates 10 (Scope Decision Record), 11 (Risk Classification
and Regulatory Applicability Record), and 12 (Discovery Sweep Record) added
2026-09-21, each carrying the record-control header and section cross-references the
appendix preamble requires. The count in the preamble was updated from nine to
twelve.

---

## Chapter 4. Defining the Problem and Use Case

**Version worked.** `chapters/04-defining-the-problem.qmd`, as at 2026-09-21. Partial
entry: the artifact obligation below was worked and is closed. The full section 18
record for this chapter is outstanding.

**Gate commands run, 2026-09-21.**

```
sentences        457
CV               0.595  (signal if <0.45)  PASS
The/This start   20%    (signal if >25%)   PASS
nominalisation   4.1%   (signal if >5%)    PASS
em dashes        0                          PASS
```

Prohibited vocabulary scan: zero occurrences. Section 6 fluff list: zero occurrences.

**A18-006. Section 4.8 named four fields its own template did not carry, and the
chapter carried the gap as prose.** The section stated that "several fields a
rigorous version needs, the legal role and jurisdiction of each actor involved, the
duration and frequency of the processing or use, and the specific authority who
accepts residual risk, are not fields this book's own templates fully specify yet,"
and closed with "that is a gap this pass records instead of silently accepting."
Recording the gap in the reader-facing text was the correct interim move and is a
better failure than Chapter 3's, where three sections established records with no
template and nothing said so. It was still an unmet obligation.

**Disposition.** FIXED. Template 5 extended 2026-09-21 with the three named fields,
plus the explicit unaddressed-risk field that section 4.8's seven-item list requires
and the per-provision mapping the same paragraph demands, each cross-referenced to
section 4.8. The chapter sentence was rewritten to name what the template now carries
and the gap disclosure removed, since the disclosure described a state that no longer
holds. Neighbour-set check run on the rewritten sentence: inherited referent from
"These seven," established terminology, verb carries the true relation, ending on new
material. Passed.

**Residual.** Two adjacent sentences of 33 and 38 words in that paragraph. The second
is pre-existing text and was not altered. Recorded, not actioned.

**Text state.** sha256 db17bc540833b279 (first 16), 9,276 words.

**Passes actually run.** The neighbour-set check on the one rewritten sentence, and
the mechanical gates. Sections 4.1 through 4.7 and 4.9 were not read in this pass.
Per section 18a a partial pass is NOT RUN, so this entry certifies the artifact
obligation in 4.8 and nothing else about Chapter 4.

---

## Rule change, 2026-09-21

**A18-007. A writing rule was enforced nowhere because it lived only in the
specification.** `BOOK_SPECIFICATION_v2.md`'s Prose Style section carried a
banned-constructions list, eliminated on sight, that `badw-book.md` did not. Every
pass logged since 2026-09-12 loaded the rules folder and not the specification's prose
rules, so the list was never gated. A scan on 2026-09-21 found eight live instances
across five chapters, all in text earlier passes had read as finished.

**Disposition.** FIXED. The list is now section 6 of `badw-book.md` under "Banned
constructions, eliminated on sight," with the provenance, the reason it moved, and a
note that every entry is mechanisable and belongs in the gate rather than a judgement
pass. Two entries carry added guidance: "importantly" and "notably" are supplied
emphasis, and "as such" and "accordingly" are supplied transitions of a kind section 6
already banned, so the word is usually a symptom and the sentence should be re-tested
without it.

**Guard against over-extension.** The new text states explicitly that this is not a
vocabulary filter and must not be extended with words that merely sound
machine-written. Section 19 already records that vocabulary markers are the weakest
generation of tell. Each entry earns its place by doing the reader's work for them,
supplying emphasis, a transition, or a contrast never in dispute, not by being a word
a model favours.

**Instances fixed 2026-09-21.**

| Chapter | Construction | Fix |
|---|---|---|
| 04 | "the specification question is not only X but Y" | recast as a statement of what the specification must state |
| 09 | "…or causal comparison accordingly" | "…to match" |
| 14 | "named as such rather than folded" | "named that way rather than folded" |
| 14 | "is accordingly not an assessment with a smaller gap" | "is not an assessment with a smaller gap" |
| 18 | "imposes a testing duty as such" | "imposes a testing duty of its own" |

**False positives recorded, not actioned.** Three uses of "as such" survive, in the
preface, Chapter 12, and Chapter 14. All three mean "in that capacity" rather than
functioning as a transition: "identified as such," "a property of agents as such,"
"labeled as such." The ban targets the transitional use. The gate pattern was
narrowed to match the transitional form only, so these do not fire. Recorded because
a future pass running a looser string would flag them and should not.

**Instrument fault recorded.** A first version of the gate matched bold-term openings
and reported 181 instances of "bold term followed by a definition fragment." The
specification bans a list wearing a costume, meaning a run of such lines standing in
for explanation, which a count cannot distinguish from a legitimate bolded lead-in
mid-paragraph. Section 14's rule that an extraordinary result impugns the instrument
first applies. Not reported as findings; the pattern was withdrawn from the gate.

---

## Full mechanical sweep, 2026-09-21

Run across all twenty-six content files after the section 6 rule change. HTML figure
comments and fenced blocks stripped first, since figure specifications use
"Must appear:", "Entry condition:" and "Deliberately excluded:" and are not prose.

**A18-008. Four further defects found and fixed.**

| File | Defect | Rule | Fix |
|---|---|---|---|
| appendix-c | clause-joining colon in template 12 | s.5 | split into two sentences |
| appendix-a | clause-joining colon | s.5 | colon to comma |
| 09-operations | "fundamentally different kind of record" | s.6 value-laden | "a different kind of record" |
| 99-back-cover | two em dashes | s.5 hard rule | commas |

The appendix C colon was mine, written the same day in template 12. The back cover
em dashes were also mine, written when the cover was built, and had never been gated
because the back cover was created after the last full pass.

**Result.** Clean across all twenty-six files on em dashes, en dashes, "regime",
clause-joining colons in prose, the section 6 fluff and value-laden lists, supplied
transitions, and every banned construction now in section 6.

**Permitted uses recorded so a future pass does not flag them.** Nine hits remain in
`90-references.qmd`, all permitted by section 5's own exceptions: en dashes in page
ranges, colons in title-subtitle pairs, and em dashes inside official ISO standard
titles, which are quoted and must not be altered. A gate that reports these as
defects has misread section 5 rather than found a fault.

**Instrument fault recorded.** A first version of the colon check matched 187
instances. Inspection showed nearly all were headings ("Case in focus: the arrest")
and figure-specification comments, both outside section 5's scope. The pattern was
narrowed to prose lines with comments stripped, which reduced it to four real
candidates, two of them genuine. Second instance this date of section 14's rule that
an extraordinary result impugns the instrument first; the first was the 181-instance
bold-term pattern under A18-007.

---

## A18-011. The book suite never loaded `w/core`, and a MUST NOT rule went unchecked

**Raised 2026-09-21 by the author.** `badw-book.md` opens by routing work between
itself and "the parent `w/` suite," and every pass in this project loaded only this
folder. `w/core/README.md` states in its first line that CORE "applies to every
serious writing task in W" and must be loaded **before any profile-specific rules**.
It was never loaded here. `badw-book.md` carries provenance lines from `badw.md`,
`badw-htw.md`, and `flow/w-replacements.md`, but not from `core`, so the omission was
invisible from inside this folder.

**The concrete consequence.** CORE-05A prohibits the `judg(e|es|ed|ing|e?ments?)`
family in authored prose as a vague, machine-shaped abstraction. A scan on 2026-09-21
found **119 occurrences across twenty-two files**. Chapter 7 alone holds 37.

**Compounding fault.** Earlier the same day the author asked directly whether the book
used "words like judgement." The answer given was that the word was the author's own,
consistently spelled, and load-bearing, based on finding no rule in `badw-book.md`.
That answer was drawn from the wrong file and was wrong. Recorded because section 18
forbids an audit statement that claims a check not performed, and the check performed
was against an incomplete rule set.

**Sense separation, per CORE-04 and CORE-14B.** A blind replacement would have damaged
the text. 24 occurrences are "judge model" and "model as judge", the evaluation
literature's own term for a Chapter 7 technique, protected by CORE-04 as established
field vocabulary. **95 are the prohibited abstraction** and are the defect.

**Disposition.** Rule FIXED, text OPEN. CORE-05A is now section 5 of `badw-book.md`
with both exceptions stated. The 95 substitutions are NOT APPLIED. Each needs a
different replacement according to what the sentence means, and several are
"value judgment", "a judgment about values", "produce judgments", where a wrong choice
changes the claim. CORE-14B requires impact assessment before a fix and CORE-11
requires a neighbour-set check on every changed sentence, so this is a scheduled pass
over twenty-two files, not a substitution run. Not begun.

**Wider consequence, unassessed.** CORE has fifteen rule families. This audit has
examined one. The others, including CORE-02A's two-pass flow audit with its thirteen
cohesion checks, CORE-04A's technical-term ledger, CORE-07's canonical establishment
point, CORE-09A's zero-trust citation gate, and CORE-13A's formatting audit, have
never been run against this book. Whether `badw-book.md` satisfies them by
inheritance, contradicts them, or simply omits them is unknown. Recorded as the
largest open item in this file.

---

## A18-013. CORE-02A flow audit, Chapter 3

**Run 2026-09-21.** First flow audit performed on this book. CORE-02B whole-artifact
read-before-edit was satisfied: the chapter was read complete, first word to last,
without editing, against sha256 7db7ee99 (8,282 words, 99 paragraphs), and every issue
noticed was logged before any fix was applied.

**Result.** Two BLOCK, six ADVISE, one check NOT RUN. All eight actionable findings
fixed the same day. Final state sha256 75e5ec99, 8,312 words.

**What passed.** All eight announced multi-item structures discharge in order under
stable labels, satisfying pass 1 check 6, which is the check prose most often fails.
The paragraph skeleton reads as an argument rather than a topic list (pass 2 check 3).
Every forward reference passes the pointer-deletion test (pass 1 check 13). Each of the
six opening objectives is discharged in-chapter (pass 2 check 8).

**F-01, BLOCK, section 3.6.** The agentic paragraph ran 234 words and introduced nine
assessment dimensions, six of them unannounced, through a repeated "Assess X, gloss,
and Y, gloss" frame. Failed concept-entry warrant (pass 1 check 14), split-rheme
discharge (pass 1 check 6), and paragraph integrity (pass 2 check 2) simultaneously. It
also contradicted the chapter's own scheme, which promises four factors in 3.6 and
states four in the Summary. **Fixed** by splitting into two paragraphs: the first
completes the autonomy-versus-reversibility argument, the second announces six
refinements and attaches each to one of the four factors rather than adding to them.

**F-02, BLOCK, section 3.6.** A 353-word paragraph carried the three tier definitions
plus four cross-cutting rules, so evidence confidence, provisional status, appeal, and
revalidation read as properties of the high tier. **Fixed** by separating tier
definitions from the four rules that govern every tier.

**F-03 through F-08, ADVISE, all fixed.** Duplicate treatment of the three system
classes compressed to its canonical point (CORE-07). Section 3.5 now finishes its own
job instead of announcing 3.6 (pass 2 check 9). Self-validating meta-commentary removed
from 3.3 (CORE-10). The discovery-governance paragraph's ten buried requirements
announced and grouped as four (pass 1 check 6). One CORE-05A `judgment` instance
replaced. The six-week and nine-week Calloway exercises disambiguated by naming the
interval (CORE-08).

**Seam repair.** Fixing F-02 created a new seam failure: the following paragraph opened
on the four factors with no inherited referent from a paragraph landing on revalidation.
Caught by the neighbour-set check and repaired with an explicit inheritance. Recorded
because it is CORE-14B's point exactly, that a fix can relocate a defect.

**Post-fix gates.** CV 0.587, The/This 24%, nominalisation 4.5%, em dashes 0, banned
constructions 0, prose clause-joining colons 0. Two clause-joining colons introduced by
the F-01 fix were caught in the post-fix scan and removed before close.

**F-09, NOT RUN.** CORE-02A requires domain-expert, educated-adjacent-field, and
smart-high-school friction passes. One reader performed this audit. The friction pass is
the one that would independently catch an F-01-class defect, and it was not performed.
This entry does not claim it was.

**Separation of duties.** Not satisfied. The same agent read, logged, fixed, and
recorded. The logging pass did complete before any fix, per CORE-02B, and each fix was
re-checked against the original finding wording rather than the replacement text.

---

## A18-014. CORE-02A flow audit, Chapter 4, three independent readers

**Run 2026-09-21.** First audit on this book to satisfy CORE-02A's multi-reader
requirement. Three agents were spawned, one per perspective, each given the file path
and its own brief. None saw another's report before submitting. Their findings differ
substantially, which is the evidence that the separation held.

**Reader 1, domain expert.** Nine findings, three BLOCK. Found a genuine legal error
that the other two readers could not have caught: Article 27's scope sentence omitted
the Annex III qualifier, so as written it implied any high-risk system deployed by a
public body triggers the obligation. Also found an evidentiary overclaim, one constructed
vignette described as "a strong argument" for a general proposition, and a descriptive
claim the chapter's own thesis refutes, that intake's three outcomes are "equally
available".

**Reader 2, educated adjacent-field.** Eight findings, three BLOCK. Found an
unresolvable referent in section 4.1's third sentence, "already assumes it exists on
someone's desk", which the domain expert read past. Also found "training distribution"
ungrounded at a point where it carries the argument, and identified that 4.3 restates
4.1's figures verbatim as though new.

**Reader 3, smart high-school friction.** Seven findings. Found that `FAIRLEND`,
TalentScreen, and the backtick convention arrive with no introduction anywhere in the
chapter, and that "non-compensable" and "the three kinds of system" assume knowledge the
chapter never supplies. Brief explicitly forbade recommending any reduction in scholarly
level; the reader complied and its report instead names where scaffolding is working.

**Consensus findings, reached independently by all three.** Two. The promised term at
"it has a name worth knowing" that is never supplied, and "which moved in July 2026",
whose referent no reader could resolve. Independent convergence is the strongest signal
this method produces.

**Disposition.** Fourteen findings fixed. Post-fix gates: CV 0.595, The/This 19%,
nominalisation 4.1%, em dashes 0, banned constructions 0, prose clause-joining colons 0.
One clause-joining colon introduced by a fix was caught in the post-fix scan and removed.
One enumeration frame orphaned by a fix ("The first is that…" left without its
announcement) was caught by re-reading the repaired paragraph and restructured.

**Rule change.** Section 18b added to `badw-book.md`, recording that independent readers
are separate agents or fresh model instances, never one agent producing three sections,
and that the friction brief must forbid recommending a lower scholarly level.

**Separation of duties.** Partially satisfied, better than any prior entry. Reading and
logging were performed by three identities none of which applied a fix. Fixing and
recording were performed by a fourth. No reader closed its own finding. The remaining
gap is that the fixer also wrote this entry.

---

## Rejection register

Findings the author has declined. Per section 18a these are closed and may not be
raised again by a later pass.

*(empty as at 2026-09-21)*

---

## Open items carried forward

| ID | Item | State |
|---|---|---|
| A18-001 | Audit entries absent for Ch. 1, 2, 5-18 and App. A-D | OPEN |
| A18-002 | Nominalisation over threshold, Ch. 12 and 13 | OPEN |
| A18-003 | Sentence-length CV 0.44, Ch. 13 | OPEN |
| A18-005 | Separation of duties unmet on self-audited entries | OPEN, structural |
| A18-009 | Ch. 3 passes 1, 3, 5 not run | OPEN |
| A18-010 | Ch. 4 read only at 4.8 | OPEN |
| CH026, CH031, CH442, CH443 | Chapter 5 figure findings, from the log | OPEN |
| CH035 | Chapter 6, from the log | OPEN |
| — | Reverse check: every section establishing a record has a template | OPEN, standing |
| — | Style sheet does not exist; see below | OPEN |
| A18-011 | 95 CORE-05A "judgment" violations across 22 files | OPEN, text |
| A18-012 | `w/core`'s other 14 rule families never run against this book | OPEN, scope |
| A18-013 | Ch. 3 flow audit complete; multi-reader passes not run | PARTIAL |
| A18-014 | Ch. 4 flow audit complete, 3 independent readers, 14 fixed | CLOSED |
| — | CORE-02A flow audit not run on Ch. 1, 2, 5-18, App. A-D | OPEN |

**Style sheet.** `w/ac/gate3-copy.md` requires a persistent `style-sheet.md`
recording every spelling, hyphenation, capitalisation, number-treatment and dash
decision, applied everywhere once recorded, and treated as a deliverable rather than
a scratchpad. This book has no such file. Its decisions are currently recoverable only
by reading the rules, the specification, and the log together, which is how the
"judgment" spelling and the "regime" ban stayed consistent by attention rather than by
record. Worth creating; not created here.

---

## A18-015 — Forward-reference density, book-wide

**Raised by:** the author, 2026-09-21. "You shouldn't be talking about chapter 18 in
chapter 3... I think we have too many of that."

**Instrument check first (section 14).** The count was taken with a pattern matching
`Chapters? [0-9]+` per file, then each hit classified forward or backward against the
containing chapter's own number. Appendices A–D, the glossary and the index return
the highest raw counts in the book (92 in the glossary alone). Those are locators in
reference apparatus, where a pointer is the entire purpose of the entry. They were
excluded rather than reported as findings, which is the second instrument fault
avoided in this audit and the third overall.

**Measurement, prose chapters only.**

| | Forward | Backward |
|---|---|---|
| Ch 1–2 | 0 | 1 |
| Ch 3–6 | 48 | 27 |
| Ch 7–12 | 20 | 90 |
| Ch 13–18 | 4 | 116 |

**Finding.** The profile is already the right shape. Forward references concentrate
early and reach zero by Chapter 16; backward references accumulate. That is the
convention comparable textbooks follow, and it is not what the author objected to.
The objection is to density in the early chapters, where Chapter 3 alone pointed at
Chapters 4, 6, 9, 10, 12, 13, 16 and 17.

**Prior audit position, and why it was insufficient.** The Chapter 3 flow audit
recorded that "every forward reference passes the pointer-deletion test (pass 1
check 13)." That test asks whether a pointer is *licensed* — whether deleting it
would strand a reader who needs the material. It does not ask whether the pointer is
*warranted*. A pointer can be individually licensed and collectively excessive, and
no check in CORE-02A measures the aggregate. The author identified a real gap in the
instrument, not a disagreement about taste.

**Rule added.** Section 12 of badw-book.md gains three rules: a forward pointer must
license an omission, hand off evidence, or close a chapter; density must taper across
the book; and a pointer states the subject, not the manuscript's structure. The
warrant test is the deletion test inverted — delete the pointer, and if the prose
stands *and* the reader is left with no unanswered question, it was an advertisement.

**Fixed.** Five advertisements cut.

| File | Cut |
|---|---|
| 03 §3.2 | "Chapter 12 develops this." |
| 03 §3.4 | Whole paragraph: "Chapter 12 returns to this system. Chapter 16 examines the due diligence that preceded the purchase." |
| 03 §3.6 | "Chapter 9 shows why that matters." |
| 03 §3.6 | "Chapter 12 develops each of these." |
| 15 §15.4 | "This is where Chapter 12 connects forward to Chapter 9." |

Chapter 3 falls from 17 forward references to 12; Chapter 15 from 2 to 1. The
Chapter 3 §3.4 cut is the clearest case in the book: an entire paragraph consisting
of two pointers and nothing else, standing between a paragraph that had already
landed its conclusion and the next section heading.

**Deliberately not cut.** The "Evidence carried forward" handoffs in Chapters 5 and 6,
the chapter-closing pointers, and deferrals that license an omission — including
Chapter 4's "Chapter 16 addresses that directly," where the reader has just been told
the buy path is the harder one to govern and is entitled to know where that is
handled. Cutting these would strand readers, which is what the pointer-deletion test
correctly protects against.

**Backward references left alone.** A backward reference costs the reader nothing.
The 116 in Chapters 13–18 were sampled and each names a specific obligation the
reader has already met and is now reusing. Reducing them would make the later
chapters restate material rather than build on it.

**Post-fix gates, both files.** Triple blank lines 0, em dashes 0, orphaned
sentence fragments 0, clause-joining colons unchanged.

---

## A18-016 — Chapters 4, 5, 6: full w-suite audit, 2026-09-21

**Method.** Three independent agents per chapter under §18b, separate contexts, no
agent seeing another's findings. Chapter 4 had a prior flow audit, so its agent was
briefed to find what that audit missed rather than re-run it. Every legal and factual
claim an agent reported was independently verified by a fourth agent before any edit
was made. That verification step changed the outcome twice and is the reason it exists.

**Instrument faults recorded and withdrawn (§14).** Two. The banned-word pattern
matched `vital` against five occurrences of `vital-sign`, clinical terminology, not
the intensifier. It also matched `leverage` against the noun meaning negotiating
position, where the ban targets the verb. Both withdrawn rather than reported.

**Verification overturning a reader finding.** The Chapter 5 substance reader
instructed me to cite EU AI Act Article 10(5) as the legal basis for processing
special-category data to detect bias. Verification established that Regulation (EU)
2026/1744, the Digital Omnibus on AI, in force 27 July 2026, **deleted Article 10(5)**
and moved the basis to a new Article 4a which also extends it to deployers. Following
the reader's instruction would have put current-law status on a repealed provision in
three chapters. This is the clearest evidence so far that §18b's independent readers
must not be trusted without a verification pass: a confident, well-sourced, wrong
instruction is the failure mode.

**Chapter 5 — factual errors corrected in §5.6.** All three independently verified
against the Gender Shades paper (PMLR v81) and IBM's own announcement.

| Was | Now |
|---|---|
| "aggregate error rates" | Subgroup rates. The paper's whole argument is that aggregates conceal these. |
| "no higher than 0.8% / between 20.8 and 34.7%" | Per-classifier: 0.0 / 0.3 / 0.8 and 20.8 / 34.5 / 34.7 |
| "two benchmarks more than three-quarters male" | IJB-A 75.4% male; Adience close to balanced. False for Adience. |
| IBM built "a subsequent system on a stated half a million images with balanced demographic composition" | Diversity in Faces, one million images, an *annotation* set not a training set, described comparatively not as balanced, and criticised within six weeks for consent failures. |

The IBM error was the most serious in the chapter. The book held up as a model remedy
a dataset assembled without subject consent, inside a chapter arguing that authority
must be settled before collection. The corrected passage keeps the case and draws the
harder lesson: the remedy for one fairness problem created a second.

**Chapter 4 — the Amazon case was wrong in a way that inverted its function.** The
chapter used Amazon's recruiting tool as its proof that stopping is reachable, stating
the system "was discontinued when it became clear that it had learned to penalise
indicators of being a woman" and that "the technical work was competent." Verified
against four independent syndications of the Reuters wire: the bias was found by 2015,
Amazon **edited the programs and continued**, and the team was disbanded in early 2017
because executives "lost hope" with the technology "returning results almost at
random." Both characterisations unsupported, the second directly contradicted.
Rewritten to carry the honest sequence and the harder second lesson: an organization
that stops a system only once it stops working has not shown it could stop one that
worked.

**Chapter 4 — an unfinished placeholder was live on the public site.** §4.8 read
"whose dates were amended in July 2026. Check the current dates rather than relying on
this sentence." Replaced with the settled dates: Annex III obligations from 2 December
2027, Annex I from 2 August 2028. A textbook telling the reader to go look it up, when
the answer is knowable and stable, signals the author did not check.

**Chapter 4 — Article 27 scope.** The text claimed to supply "the part most summaries
drop" while itself dropping the express Annex III point 2 carve-out for critical
infrastructure. It also stated FAIRLEND falls inside Article 27 *because* Meridian is
a private company, which is backwards: under the general limb private character is what
**excludes** a deployer. FAIRLEND is caught because creditworthiness is Annex III point
5(b), which reaches any deployer. Both corrected.

**Chapter 6 — Article 25 scope defect.** The text restricted all three role-shift
conditions to "a high-risk system." Article 25(1)(c) is precisely the opposite case: a
system **not** classified as high-risk whose changed intended purpose makes it one.
As written it gave a fine-tuner working on a non-high-risk system a false assurance
that the rules could not reach them, which is the situation a fine-tuner is usually in.

**Chapter 6 — fine-tuning mechanism.** "Adds a thin, task-specific layer on top"
describes adapter methods only. Full fine-tuning updates the base weights, producing an
artifact in which original training and adaptation cannot be separated. The chapter's
own §6.8 bill-of-materials field presumed the distinction its §6.1 definition erased.

**Chapter 6 — internal contradiction.** §6.5 established the accuracy/interpretability
tradeoff as contingent and requiring a test; the Summary asserted it as settled
architectural fact. A reader using the Summary as the takeaway would skip the test the
section says is mandatory. Summary rewritten to match the section.

**Other corrections.** Chapter 5's fine-tuning dilution mechanism (a proportional skew
does not dilute with scale; the leverage comes from where fine-tuning sits in the
process) and its claim that broad behaviour "resists the influence of any small
addition," which is the opposite of published findings. Chapter 5's §5.9 named nine
privacy techniques while teaching four, violating the section's own stated rule that
each earns its place only alongside what it does not protect against. Chapter 5's
anonymization definition, wrong in both directions: it stated absolute untraceability
where GDPR Recital 26 asks about means reasonably likely to be used, and omitted the
legally decisive consequence that anonymised data falls outside the regulation
entirely. Chapter 4's "selection on the dependent variable" misnamed what is properly
the selective labels problem. Chapter 5's §5.5 remedy list offered only build-path
options in a chapter establishing that most readers are on the buy path.

**CORE-05A.** 15 `judgment`-family violations across the three chapters at open,
0 at close. All hits now remaining are inside HTML figure comments, which are not
authored prose and which CORE-05A does not reach.

**Post-fix gates.**

| Chapter | CV | The/This | Nominalisation | Em dash | judgment |
|---|---|---|---|---|---|
| 04 | 0.62 | 19% | 5.1% (was 5.3) | 0 | 0 |
| 05 | 0.52 | 17% | 6.5% (was 6.7) | 0 | 0 |
| 06 | 0.51 | 18% | 6.6% (was 6.7) | 0 | 0 |

Triple blank lines 0, orphaned fragments 0, banned constructions 0 across all three.

**Open, not closed.** Chapter 6's §6.2 objective-1 gap (the chapter lists eight axes
but never supplies a comparison method), the missing selection-decision owner, and the
Chapter 5 datasheet handoff that no later chapter consumes are recorded and unfixed.
Each changes what the chapter argues rather than how it reads, and CORE-14B puts those
in front of the author rather than an agent.

---

## A18-017 — Chapter 3 CORE-02A flow audit after revision, 2026-09-21

**Why run it.** Chapter 3 had been revised heavily in one session: a new section
inserted, 3.3 through 3.8 renumbered, three filled record tables added, a figure
added, and 3.7 restructured. New material that has not been re-cohered with its
surroundings is the predictable failure, and it is what the audit found.

**Method.** Three independent readers per §18b, separate contexts: Pass 1 local
cohesion, Pass 2 whole-artifact coherence, and three reader perspectives (student,
practitioner, hostile expert). File hash recorded before reading per CORE-02B:
2d97584feb1ea20f, 74,186 bytes.

**Consensus findings, raised independently by all three readers.**

*The eight grounds were never enumerated.* The definition box ran them as a prose
comma-string and the chapter then referred to "the eight grounds" three times, plus
`Grounds:` cells in a filled record. A reader had to count commas in a seventy-word
sentence to discover both the number and the name. Fixed: the box now names and
glosses all eight.

*The trace came after the example that needed it.* Section 3.2 worked a full boundary
on a list of seven dependencies, and section 3.3 then explained how to generate such a
list. Section 3.2 apologised for this in a parenthetical rather than fixing it. The
four passes have been moved ahead of the worked example, which now opens "Run the four
passes over Calloway's deployment and seven dependencies surface." Section 3.3 keeps
the two conceptual subsections and is retitled.

**Damage from my own edits, found and fixed.** Three defects traced to this session's
renumbering and insertions, not to the original text.

| Defect | Cause |
|---|---|
| "risk classification, in sections 3.6 through 3.8" | Old numbering carried forward; the range now sweeps in the two sections the chapter works hardest to distinguish from classification |
| "Section 3.4 describes what an inventory later found inside it" | Should be 3.5; renumbering |
| "Calloway's record above" pointing twenty-four lines below it | Filled record inserted after the sentence that referred to it |

**Contradiction between two worked accounts.** Section 3.7 said TalentScreen's
scheduling component went from low to high on reversibility and population. The
section 3.9 case box said TalentScreen went from medium to high on unmeasured human
review, citing "the reason given earlier in this chapter" for a reason not given
earlier. Review question 7 examines the first version. Section 3.7 made authoritative;
3.9 now reports the autonomy measurement as a separate finding about screening rather
than as the reclassification.

**Legal error, verified before correction.** The hostile reader identified the worst
finding in the audit, and independent verification against GDPR Article 3, Article 22,
and EDPB Guidelines 3/2018 confirmed it. Section 3.8 argued that a mapping rule must
encode a regulation's own trigger rather than a paraphrase, and then paraphrased
Article 22 wrongly in the sentence demonstrating the standard. It folded territorial
scope into the Article 22 trigger and stated that scope as a per-data-subject location
check. Article 3(1) applies to processing by a controller established in the Union
regardless of where the data subject is; the location test describes only Article 3(2),
which covers controllers not established in the Union. EDPB Example 4 is direct
authority. A Dublin-established controller processing data about a person in Brazil is
inside the regulation, and the book's rule would have let it out. Rewritten as two
rules: Article 3 decides whether the regulation applies, Article 22 then has its own
trigger, which is a decision based solely on automated processing producing legal or
similarly significant effects.

**Substantive objections answered rather than deflected.** The hostile reader raised
three the chapter could not leave standing.

*The exclusion asymmetry.* The chapter included dependencies on eight broad grounds and
excluded payroll on the narrow input-output test section 3.2 spends its length
rejecting. The exclusion now runs the same eight grounds in the negative and says
explicitly that the shorter argument is the rejected one, which would also have
excluded single sign-on.

*"Materially" had no threshold.* The load-bearing qualifier in the whole test was
undefined. Now: a dependency affects a ground materially when its failure would change
what a reviewer could establish or what an affected person could do. The three
dispositions, including limited depth, are named as the answer to the everything-is-in
problem.

*The maximum rule inflates tiers.* Section 3.7 names "a scheme that classifies
everything as high risk is functionally identical to having no scheme at all" as the
failure condition, then supplied a rule that produces it. Answered with two checks: the
driving factor must independently meet the high-tier inclusion rule, and the governance
a high tier attracts is set by the driving factor rather than applied wholesale.

*The amnesty promises what the employer does not own.* An employer can waive its own
response and cannot waive a duty running to a regulator or a counterparty. Section 3.5
now states the limit before the period opens.

**Post-fix gates.** CV 0.61, The/This 22%, nominalisation 5.3%, em dashes 0,
`judg*` 0, triple blank lines 0, dangling section references 0, enumeration frames all
discharged. Nine sections, correct order, three filled records rendering, no broken
figures.

**Open, recorded, not fixed.** The objectives list and the summary do not cover the new
section 3.3 or section 3.9's "scope broadly and govern proportionately," which Pass 2
identified as the chapter's most actionable rule and the disposition Chapter 4's intake
assumes. The Calloway case numbers carry argumentative weight the hostile reader showed
hypothetical figures cannot bear: the eleven-to-forty-three improvement is attributed
to method while the first pass is retroactively recharacterised, the amnesty's success
criterion is redefined after its result, and 400 person-hours for 43 systems is an
order of magnitude below what the chapter's own worked boundary implies. Those are
authorial decisions about a hypothetical case, not defects an agent should resolve.

---

## A18-018 — Borrowed verbs, book-wide, 2026-09-21

**Raised by:** the author, after reading a teaching note I wrote. "If you follow W, we
won't have such things like 'turn on'." Then, correctly sharpening it: "fires? it is not
in the subject domain so shouldn't be used. any word not in the domain should never be
used. surfaces?"

**My first answer was wrong and is recorded as such.** I measured 292 instances of vague
metaphor, fixed the obvious ones, and then defended `surfaces`, `fires`, `reaches` and
`attaches` as domain vocabulary. Two of those four are not. A trigger does not ignite. A
dependency does not rise through water. I had drawn the line at what sounded
professional to me rather than at what a reader can picture, which is the same fault the
rule is supposed to catch.

**The rule as it now stands.** "Is this word from the domain" cannot be the test, because
almost no verb originates in AI governance. The usable test is whether the reader has to
picture a physical action to recover the meaning. Ask what is physically happening in the
sentence; if the literal answer is absurd, the verb is borrowed and the translation is
work the writer left undone. The same word passes or fails by subject: software **runs**,
a record **carries** a date, an obligation **attaches** to a system, a law **reaches** a
deployer. None of those asks the reader to picture anything. Written into section 6 with
a six-row table of failures and their replacements.

**Measurement.** 693 instances of twelve borrowed verbs book-wide. Of those, `runs` (146)
and `carries` (166) are overwhelmingly literal and were left alone.

**Instrument faults recorded and withdrawn.** Three. `sweep` is a defined term in section
3.5 with its own Appendix C template. `collapse`, as in collapsing two categories into
one, is standard analytic usage. `data surface` is a defined term in Chapter 5, and 11 of
that chapter's 24 `surfac*` hits are the noun, not the verb. Reporting any of these would
have been a finding against the book's own vocabulary.

**Fixed in Chapters 1 through 6.**

| Was | Now |
|---|---|
| the trace surfaces a dependency | the trace finds it |
| an automatic trigger fires | an automatic trigger applies |
| a deployment lands here when | a deployment belongs here when |
| averaging buries the factor that should drive the decision | averaging hides the factor that should decide the outcome |
| record which factor drove it | record which factor decided it |
| everything turns on what meaningfully means | everything depends on what meaningfully means |
| the regulation that bites soonest | the regulation that applies soonest |
| the full apparatus | the full set of high-tier controls |
| two questions are in play | two questions have to be answered |
| materially is doing work in that sentence | materially is the word that decides the outcome |
| no purchase on the training decisions | no way to influence the training decisions |
| the boundary a real decision turns on | the boundary where a real decision is made |

**CORE-05A, found while here.** Chapter 7 carried 37 `judg*` hits. 24 are `judge model`,
the technical term for LLM-as-a-judge evaluation, which is protected field vocabulary and
was withdrawn as a fourth instrument fault. The other 13 were real and are fixed. Chapter
2's single hit is `SCHUFA judgment`, a case name, which the rule does not reach.

**Open.** 59 borrowed-verb instances remain in Chapters 7 through 18 and the appendices.
Those chapters have not been audited and are queued for the weekly batches. The rule is
now in section 6, so those runs will catch them.

---

## A18-019 — Three changes from a student critique, 2026-09-22

**Source.** Mirzad Glavic, CS747 session 3, classified Bentley's own Turnitin deployment
against Chapter 3's method and submitted a nine-section handout with an appendix. Three
of his findings required changes to the chapter. All legal claims in his handout were
independently verified before any edit; none was contradicted.

**1. An ambiguous sentence in section 3.7, found by the student.** The text read that a
legal classification such as an Annex III entry places a system in the high tier on its
own, and that no combination of low scores offsets a trigger law sets independently. He
observed that the AI Act's Article 6(3) lets a provider conclude an Annex III system is
not high-risk after all, and asked whether the two conflict. His own answer: it depends
on whether the chapter is describing the law's category or advising on the internal
tier, and the sentence reads either way. He declined to resolve it and raised it instead.

He was right that it reads both ways. Resolved in the direction his own work implies: he
built a tier from institutional documents with no legal input and it held, so the
sentence is about the internal tier. A paragraph now says so, and states that whether the
law classifies a system is a separate question decided by the law's own test under
section 3.8. The two rules answer different questions and do not conflict.

**2. The appeal route is unreachable from outside, conceded.** Section 3.7's cross-cutting
rules give an affected party a route to appeal the classification. He pointed out that the
route runs to someone inside the organization, so it exists only once the organization has
classified the system. Bentley had produced no tier, no reasoning, no reviewer and nothing
to appeal, which left him with no route at all. He was fair about it, noting the chapter is
written for organizations governing their own systems and he is not one.

The chapter now states the limit rather than leaving a reader to find it. Where nothing was
classified there is no tier to appeal; what remains is outside the organization, and the
chapter does not govern it. The closing sentence puts the gap where it belongs: the appeal
route exists only where the governance did.

**3. The autonomy factor had no measurement procedure.** His six-link decision chain showed
that Bentley's instructor review produces no threshold and no record, and that the official
record begins two links later. The chapter already held that an unmeasured review is an
assumption rather than a control, but never said what would make one measurable, which left
the factor unusable in exactly the case it was written for.

Three requirements added: a stated threshold, a record of the decision including the cases
where the reviewer looked and did nothing, and a disagreement rate. Where a deployment
produces none of the three, the honest entry is unmeasured rather than low, and unmeasured
supports the high tier because the organization cannot show the control exists.

**Defect I introduced and caught.** My replacement text for item 3 used "exercising
judgement", a CORE-05A violation in new prose. Found on the post-fix scan and fixed. Third
time in this project that a fix has introduced a defect, which is the scan earning its place.

**Verified, nothing to change.** Chapter 2's compliance dates and Appendix B's timeline were
checked against Regulation (EU) 2026/1744 and are correct and current, including the deferral
of Annex III high-risk obligations to 2 December 2027 and Annex I to 2 August 2028.

**Open, not fixed.** The book uses "in force" to mean both that a text is law and that an
obligation binds, and never separates them. Articles 6, 8 and 9 and Annex III are in the gap
right now: law today, binding from December 2027. One paragraph in section 2.6 would fix it.
Left for the Chapter 2 batch.

**Post-fix gates.** CV 0.61, The/This 21%, nominalisation 5.3%, em dashes 0, judgment 0,
triple blank lines 0, dangling section references 0.

---

## Portfolio measurements, 2026-09-21

Recorded so the outstanding audit work is bounded. A measurement is not an audit
entry; these files still require the full section 18 record.

| File | Sents | CV | The/This | Nomin. | Em |
|---|---|---|---|---|---|
| 00-preface | 66 | 0.55 | 18% | 3.8% | 0 |
| 01-what-ai-governance-is | 409 | 0.60 | 17% | 4.4% | 0 |
| 02-regulatory-landscape | 428 | 0.56 | 18% | 5.6% | 0 |
| 03-scoping-inventory-classification | 445 | 0.59 | 24% | 4.5% | 0 |
| 04-defining-the-problem | 459 | 0.60 | 20% | 4.1% | 0 |
| 05-data-governance-for-ai | 386 | 0.51 | 16% | 5.5% | 0 |
| 06-model-selection-and-development | 280 | 0.49 | 16% | 5.4% | 0 |
| 07-testing-evaluation-and-red-teaming | 348 | 0.48 | 16% | 5.0% | 0 |
| 08-deployment-and-release | 210 | 0.50 | 11% | 6.2% | 0 |
| 09-operations-and-monitoring | 306 | 0.46 | 9% | 5.4% | 0 |
| 10-incident-response-and-remediation | 248 | 0.46 | 18% | 5.6% | 0 |
| 11-governing-generative-systems | 243 | 0.49 | 16% | 5.5% | 0 |
| 12-governing-agentic-systems | 250 | 0.45 | 13% | 7.3% | 0 |
| 13-organizing-the-governance-function | 246 | **0.44** | 19% | **7.6%** | 0 |
| 14-risk-assessment-and-management | 278 | 0.52 | 15% | 6.8% | 0 |
| 15-documentation-and-evidence | 253 | 0.52 | 13% | 6.6% | 0 |
| 16-third-party-vendor-and-supply-chain | 235 | 0.50 | 12% | 6.5% | 0 |
| 17-implementing-ai-governance | 282 | 0.53 | 15% | 5.3% | 0 |
| 18-governing-under-uncertainty | 200 | 0.52 | 12% | 6.2% | 0 |
| appendix-a-technique-reference | 132 | 0.50 | 5% | 5.2% | 0 |
| appendix-b-regulatory-quick-reference | 92 | **0.38** | 21% | 7.5% | 0 |
| appendix-c-templates-and-checklists | 33 | 1.15 | 6% | 7.1% | 0 |
| appendix-d-glossary | 132 | **0.31** | 6% | 7.0% | 0 |
| **Book** | **5,961** | — | **16%** | **5.7%** | **0** |

Bold marks a value past a section 7 signal. Em-dash count is zero in every file,
satisfying section 5's hard rule book-wide. The section 6 fluff list returns zero
occurrences book-wide.
