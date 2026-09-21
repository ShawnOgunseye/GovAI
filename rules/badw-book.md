# badw-book : writing rules for textbooks

## SCOPE. READ THIS BEFORE ANY OTHER LINE IN THIS FOLDER.

**Rule type** Mandatory scope control
**Author** User, written by cl
**Confidence** 100%

**This folder governs textbooks and nothing else.** Every rule below is written for a
book whose purpose is to make a reader able to do something they could not do before.
If the work in front of you is not that, these rules do not apply to it and applying
them will damage it.

**A textbook, for the purpose of this folder, has all five of these properties:**

1. it teaches a practitioner or student to perform, decide, or assess something;
2. its chapters are read alone as often as in sequence;
3. it defines constructs the reader is expected to apply to cases;
4. it carries figures, worked cases, and end-of-chapter questions; and
5. it is revised as the underlying law, standards, or practice change.

**This folder does not govern:** journal articles, conference papers, theses, grant
applications, reports, white papers, memos, blog posts, documentation, marketing
copy, slides, or fiction. For a scientific manuscript, use the parent `w/` suite:
`README.md`, `badw-htw.md`, `badw.md`, and `badw.py`. That suite assumes a target
journal, a research question, a study design, and measured variables. This one
assumes a reader who must act.

**The gate.** Before applying any rule in this folder, state in the audit record
which of the five properties the work has. **If the work in front of you has fewer
than five, stop.** Do not adapt these rules to it. Do not apply the parts that seem
to fit. Say which suite the work belongs to and use that one instead.

**If you are an agent that has just entered this folder:** this file and
`README.md` in this folder are the entry points. Read `README.md` first for the
iteration loop and the logging contract. Read this file for the rules. Do not begin
from any other file, and do not begin from a rule you remember.

---

## Stop. Complete the load gate first

**Rule type** Operational control
**Applies to** drafting, rewriting, and any edit down to a single word

Load this file before writing. It is self-contained: it carries every rule from the
`w/` suite that applies to a book, so `README.md`, `badw.md` and `badw-htw.md` do not
need to be loaded alongside it. Run the gate scripts before delivering.

**Operational reason.** These files change. A rule is what the file says in the
session where the work is done. Loading it makes the session auditable: the audit
record names which rule was applied and a reader can check that against the file. A
session that did not load it has nothing to check against.

**Completion condition.** The audit record names this file and the date of the
version loaded. Absent that line the gate is not passed and no edit is offered.

Do not claim that these rules have been encoded, remembered, or applied merely
because they exist in the folder or were used in an earlier session. State only that
they were loaded and applied in the present session.

For a localized edit, also load the sentence before, the sentence after, and enough
of the paragraph, chapter, and source material to determine the edited sentence's
meaning. Loading is not application. Complete every applicable check before
returning the edit.

---

## What this file is, and what it replaces

The `w/` suite governs scientific manuscripts. It assumes a target journal, a
research question, a study design, measured variables, and a reviewer. A textbook has
none of those. It has a reader who must be able to do something afterwards. Read the
scope control at the top of this file before using anything below it.

**Carried across unchanged,** because they govern prose rather than research: the
five revision passes, the skeleton and paragraph-summary tests, structure, narrative,
what to cut, sentences, the mandatory neighbour-set check, texture and uniformity,
verifying, and the prohibitions on optimising for the rules and on rules that explain
failure in advance.

**Adapted,** because the object changed: claims now answer to sources, law, standards
and documented cases rather than to a design and a measurement; cases are running
teaching cases and documented real ones rather than research cases; sections become
chapters and chapter parts.

**Dropped,** because there is no object to attach them to: target journal and fit
argument, abstract construction, cover and response letters, statistical
significance, identification strategy, null results, robustness checks, and the
limitations section as a genre.

**Added,** because a book teaches and a paper does not: the teaching contract,
cross-chapter obligations, currency, and the figure rules in section 11.

### Precedence when rules appear to conflict

Apply this order:

1. truth, source fidelity, legal and factual accuracy, and disclosure;
2. the author's explicit instructions for the book;
3. what the reader must be able to do after the chapter;
4. structural and narrative judgement in sections 1 to 6;
5. countable warnings from the gate scripts.

A lower rule cannot override a higher obligation. Do not delete a necessary
qualification to shorten a sentence. Do not add an unsupported objection to create
tension. Do not rename a construct to vary vocabulary. Do not soften a legal
statement because the hedge makes the prose less decisive.

When two applicable rules still conflict, stop that edit, name both rules in the
audit record, apply the precedence above, and record the decision. Never resolve a
conflict silently.

### Gate classes

**Hard failures** block completion: fabricated or mismatched citations, quotation
drift, altered numbers or dates, a legal or standards claim the source does not
support, an invented case or example presented as documented, hidden characters,
banned chat artefacts, and an undisclosed material limitation on advice the reader
will act on.

**Mandatory review warnings** also block completion until examined: long sentences,
low sentence-length variation, uniform paragraphs, repeated openings, repeated
three-part lists, template runs, nominalisation density, supplied transitions, and
uniform hedging. These are fallible signals. Fix the underlying template where one
exists. Otherwise retain the passage and record why it is necessary.

**Narrative failures** block completion even when the scripts are clean. A chapter
must have a consequential problem, a stable object of attention, an evidence-led
development, a resolution the material supports, and a stated consequence for what
the reader does.

---

## 0. The revision protocol

Five alternating passes. Each catches what the previous missed. Top-down finds
structural problems and skims sentences; bottom-up finds sentence problems and misses
structural gaps. Alternating forces both lenses.

**Pass 1 : top-down.** Read chapter titles in sequence. Does each follow from the
last? Then section headings within each chapter. Then paragraph by paragraph: does
the first sentence of each connect to the last sentence of the previous? Then
sentence by sentence.

**Pass 2 : bottom-up.** Every sentence: does it earn its place, does it advance the
argument, and does every qualification affect the truth of the claim? Review
sentences over 45 words for visible structure. Shorten until the loss test in section
15 fails, and stop there. Record any sentence retained above 45 words, with the
relation that splitting would break.

For every revision, however small, inspect the revised sentence with both neighbours
at once. Confirm all four requirements in the mandatory neighbour-set check in
section 7: inherited referent, established terminology, the true relation in the
verb, and new material in the ending.

Then every paragraph as a unit: one job, done, stopped. Then every section. Then the
chapter: does it advance the book's argument, or do another chapter's job?

**Pass 3 : top-down again.** Cutting sentences changes paragraph flow; cutting
paragraphs changes section logic. Verify the chain still holds after surgery.

**Pass 4 : bottom-up, defensive language only.** Look specifically for: "X, not Y"
constructions, "not merely", "regardless of"; meta-commentary; caveats volunteered
that no reader would raise; implausible objections invented, or serious ones ignored;
hedged statements the sources support directly; any rhetorical pattern appearing more
than five times.

**Pass 5 : top-down, as a cold reader.** Every sentence immediately clear, every
transition seamless, every section inevitable. If the reader would pause and ask "why
is this here?" or "didn't I read this already?", there is still a problem.

---

## 1. Structure

**Everything earns its place.** Every chapter, section, paragraph and sentence must
follow from what precedes it and lead to what follows. If it does not, it does not
belong in the book.

Adding a transition word to a logic break is a bandage, not a fix. If a sentence
introduces a new direction without connecting to what the previous sentence
established, restructure the sequence.

**The skeleton test.** Read only the first sentence of every paragraph, in order.
They should tell the complete story of the chapter without anything else. Any first
sentence that does not follow from the previous paragraph's first sentence marks a
structural break. Run this after every round of cuts, because cutting changes the
skeleton.

**The paragraph-summary test.** Summarise each paragraph in one sentence,
independently. Number them. Read them in order. Do they cohere?

**Paragraph continuity.** A paragraph ending with a claim about X should be followed
by a paragraph beginning with X or its consequence. If the next paragraph begins with
Y, the reader experiences a jump.

**No direction reversal inside a paragraph.** If sentences one to three describe
organizations that adopted a control and abandoned it, sentence four must not
describe barriers to adoption. Different populations, different directions, different
paragraphs.

**One move per paragraph.** When a paragraph covers the obligation, the exception,
the enforcement history, the practical workaround and the cost of getting it wrong,
split it.

**The chapter must survive being read alone.** Readers are given single chapters.
A chapter that only makes sense in sequence has pushed its work onto the book.
Every term the chapter depends on is either defined in it or named as belonging to a
specific earlier chapter the reader can go to.

---

## 2. Narrative

**Problem first, not framework first.** Lead with the problem. Introduce frameworks
as diagnostic instruments when the argument needs them, not as bodies of literature
presented before the reader knows why. The reader should always know why they are
reading a paragraph before they read it.

**Frameworks enter and exit.** A framework enters when the argument needs it and
leaves when it has done its work. It does not linger as architecture the reader must
hold in memory waiting for a payoff. This is the difference between a book that uses
frameworks and one that displays them.

**The chapter spine.** Write it in seven lines before drafting:

1. **Accepted state:** what a competent practitioner currently believes or does.
2. **Complication:** the failure, obligation, incident, or consequence that belief
   cannot handle.
3. **Question:** the exact uncertainty the complication creates.
4. **Development:** the distinctions, cases, or procedures that progressively answer it.
5. **Turning material:** the case or requirement that most changes what the reader
   should do.
6. **Resolution:** the answer the sources support, which may be partial.
7. **Consequence:** what the reader must now do, decide, record, or stop doing.

The complication must be more than an absence. "Most organizations have no inventory"
reports a fact. It becomes a problem only when that absence prevents compliance,
prevents assessment, or produces a harm the chapter can name.

**Keep a stable protagonist.** In a chapter this may be a system, an organization, a
role, an obligation, or a decision. If a paragraph begins with people and ends with a
model as though the model acted, the object of attention has drifted. Signal a
necessary change of level.

**Order by conceptual dependency,** not by the order in which the author learned the
material or the order the law was enacted.

**Control pace by difficulty.** Compress routine context. Slow down where a term
changes meaning, where an obligation becomes conditional, where a case contradicts an
expectation, or where the reader must hold two distinctions at once. Length follows
cognitive load, not a quota.

**Let importance determine space.** Develop the controls the reader will use most
fully and dispatch edge cases briefly. Do not allocate equal space by template. Do
not suppress material the reader needs to act.

### Four narrative checks

* **Spine test:** fill all seven lines. Fail if two lines merely repeat one another,
  the complication is only an absence, or the resolution exceeds what the sources support.
* **Protagonist test:** name the object of attention in every paragraph. Fail
  unexplained switches of actor, level, system, or role.
* **Promise-payoff test:** map every promise the chapter opening makes to the place
  it is paid off. Fail orphan promises and unannounced material.
* **State-change test:** write what the reader knows or can do after each paragraph.
  Fail a paragraph that changes neither knowledge, nor confidence, nor question, nor scope.

**Sources for this section.** Joshua Schimel, *Writing Science*, on the internal
story whose structure carries the argument; Jon Franklin, *Writing for Story*, on
complication and resolution in factual narrative; Wayne Booth, Gregory Colomb, Joseph
Williams, Joseph Bizup and William FitzGerald, *The Craft of Research*, on
reader-oriented problems, claims, reasons, evidence and objections. These are
operational adaptations, not quotations or stylistic imitations. They govern the
logic of factual exposition. They do not license fictional technique.

---

## 3. The teaching contract

**New for this file.** Author Claude. These rules are drawn from instructional
research, cited below. Each names an action and a completion condition. They have not
been validated on this book; the confidence stated is confidence in the underlying
finding, not in its effect on this manuscript.

**A concept introduced must be used.** Every construct, distinction, or framework the
chapter defines must appear again where the reader applies it. A definition that is
never used is decoration. **Test:** for each defined term, name the later passage that
uses it. **On failure:** cut the definition or add the application.

**A definition must be a test the reader can run.** "AI governance is how an
organization decides what its AI systems may do, establishes that they do it, and
makes clear who answers when they do not" is usable, because a reader can hold a
programme against it and find the missing part. A definition the reader cannot apply
to a case in front of them is a gloss. **Test:** state the case the definition
decides. **On failure:** rewrite until it decides one.

**Worked before abstract.** Where a procedure has steps, show one worked instance
before stating the general rule. Studying a worked example imposes less load than
solving the equivalent problem unaided, and the advantage is largest for readers new
to the material. **Test:** for each procedure, name the worked instance. **On
failure:** add one or cut the procedure to a reference table.

*Confidence* high. John Sweller, "Cognitive Load During Problem Solving: Effects on
Learning", *Cognitive Science* 12(2), 1988,
[DOI 10.1207/s15516709cog1202_4](https://onlinelibrary.wiley.com/doi/10.1207/s15516709cog1202_4).

**Scaffolding that helps the novice hinders the expert.** Detailed step-by-step
support improves learning for readers without prior knowledge and degrades it for
readers who have it. A practitioner book has both in its audience. **Test:** mark each
scaffolded passage with the reader it is for. **On failure:** move the scaffold into a
clearly labelled box or appendix the experienced reader can skip without losing the
argument.

*Confidence* high. Slava Kalyuga, "Expertise Reversal Effect and Its Implications for
Learner-Tailored Instruction", *Educational Psychology Review* 19, 2007,
[DOI 10.1007/s10648-007-9054-3](https://link.springer.com/article/10.1007/s10648-007-9054-3).

**Identify the concepts that are hard because they are transformative.** Some ideas
are troublesome not because they are complex but because accepting them changes how
the reader sees everything after. In this domain, that a model can discriminate with
no discriminatory rule anywhere in it is one. Give those concepts room, more than one
angle, and a case. **Test:** name the chapter's transformative concepts. **On
failure:** if a chapter has none, ask whether it is teaching or listing.

*Confidence* medium; the framework is widely used in higher education and is
qualitative rather than experimental. Jan Meyer and Ray Land, "Threshold Concepts and
Troublesome Knowledge (2)", *Higher Education* 49, 2005,
[DOI 10.1007/s10734-004-6779-5](https://link.springer.com/article/10.1007/s10734-004-6779-5).

**Questions must require retrieval, not recognition.** End-of-chapter questions that
can be answered by scanning back are recognition and teach little. A question that
requires the reader to produce the analysis from memory, or to apply it to a case not
in the chapter, is retrieval. Retrieval produces substantially better long-term
retention than rereading. **Test:** for each question, state what the reader must
generate. **On failure:** rewrite it as a case to analyse.

*Confidence* high. Henry Roediger and Jeffrey Karpicke, "Test-Enhanced Learning:
Taking Memory Tests Improves Long-Term Retention", *Psychological Science* 17(3),
2006, [DOI 10.1111/j.1467-9280.2006.01693.x](https://journals.sagepub.com/doi/abs/10.1111/j.1467-9280.2006.01693.x);
and "The Power of Testing Memory", *Perspectives on Psychological Science* 1(3), 2006.

**Define the terms a process uses before walking the process.** A reader who meets a
new term inside a procedure must hold the procedure and learn the term at once.
**Test:** for each procedure, confirm its terms were defined earlier. **On failure:**
move the definitions ahead of it.

**Cut what is interesting but not load-bearing.** Material added for interest
competes for the same attention as material the reader needs. **Test:** for each
digression, name what the reader does with it. **On failure:** cut it.

*Confidence* high for both. Richard Mayer, *Multimedia Learning*, 3rd edition,
Cambridge University Press, 2021, on the pre-training and coherence principles.
[Publisher record](http://assets.cambridge.org/97811071/87504/frontmatter/9781107187504_frontmatter.pdf).

---

## 4. Flow

This section and section 7 are the centre of the file. Flow failures are the most
common defect in generated prose and the hardest to see on rereading.

### Mandatory neighbour-set check

**Text supplied by** User
**Adopted by** CH
**Confidence** 100%
**Carried verbatim** from `README.md`, `badw.md` section 7 and `badw-htw.md` section 7.

**Check a rewritten sentence against its neighbours as a set, not in sequence.**
A sentence that fixes one seam often breaks another: repair the opening referent
and you may swap a construct term for a synonym; state the true causal verb and
you may drop the inherited word that carried the reader across. Before accepting
a revision, confirm together that it opens on a term already in the reader's
mind, reuses the passage's established words rather than fresh ones, states the
real relation in its verb, and ends on new material. Satisfying three and breaking
the fourth is not an improvement but a relocated defect.

**Before offering any rewritten sentence, verify all four against the sentences
around it, together, not in sequence:**

1. **Inheritance.** The opening words pick up a term already in the reader's
   head from the previous sentence. Name which word carries across.
2. **Vocabulary.** Established terms of the passage are reused verbatim, not
   replaced with synonyms. Changing a load-bearing word is itself a flow break.
3. **Truth of the connective.** The causal or logical verb, such as "causes,"
   "is a source of," or "installs," states the real relation, not one that merely
   sounds like a link.
4. **Completion.** The sentence advances to something new by its end. It does
   not restate the prior sentence in fresh words.

This is a scoped continuity rule. A new term is permitted only when the referent
genuinely changes, and the sentence must make that change explicit.

The four criteria test the seam between one sentence and its neighbours. They do not
test the rhythm of a run of sentences. A passage can satisfy inheritance,
vocabulary, connective and completion at every seam and still read as choppy,
because three consecutive short sentences on one frame break nothing locally. After
the neighbour-set check passes, read the paragraph aloud as a unit and apply the run
tests in section 8.

Run this check after every accepted wording change, including a one-word change. The
inspection unit is the revised sentence, its predecessor, and its successor. At a
paragraph boundary, include the sentence across that boundary. Do not delegate this
judgement to a script.

**Scientific-writing basis** George Gopen and Judith Swan, "The Science of Scientific
Writing", on topic position, stress position, backward linkage, and placing the
action in the verb; Guy Norman, "Consistent Naming in Scientific Writing: Sound
Advice or Shibboleth?", on repetition rather than synonym substitution; Joseph
Williams and Joseph Bizup, *Style: Lessons in Clarity and Grace*, on old-before-new
flow, consistent topic strings, and repeated key terms.
[Gopen and Swan](https://www.americanscientist.org/blog/the-long-view/the-science-of-scientific-writing),
[Norman](https://doi.org/10.1016/S0889-4906(02)00013-3), and
[Cornell's open summary of Williams's cohesion method](https://knight.as.cornell.edu/news/how-flow).

---

## 5. Sentences

**Review long sentences.** No sentence over 45 words may pass without review. Rewrite
it below 45 words unless its subject, action, qualification, and logical relation
remain visible and splitting would damage meaning or emphasis. Shorten until the loss
test in section 15 fails, and stop there. Record any retained exception in the audit,
with the relation that splitting would break.

**No em dashes. No en dashes except page and date ranges.**

**Do not use the "judgment" word family in authored prose.** Prohibited: judge,
judges, judged, judging, judgment, judgments, judgement, judgements. Name the actual
operation instead: assessment, decision, determination, evaluation, inference,
review, or interpretation, whichever the sentence means. **Carried from `w/core`
CORE-05A, 2026-09-21**, which classes the family as a vague, machine-shaped
abstraction used where a more exact term exists. This file did not previously carry
the rule, so no pass had ever checked it; a scan on adoption found 119 occurrences
across twenty-two files.

Two exceptions. **Source fidelity**, per CORE-01A: an exact quotation, official title,
or fixed statutory wording is reproduced as supplied, and each retained instance is
documented. **Established field terms**, per CORE-04: "judge model" and "model as
judge" are the evaluation literature's own names for a technique this book teaches in
Chapter 7, and renaming them would obscure the reference rather than clarify it. The
adoption scan separated the senses: 24 occurrences are the technical term and are
retained; 95 are the prohibited abstraction. Do not extend the exception beyond a term
the field itself uses.

**Do not use "regime" for a law, regulation, or standard.** Use "regulation,"
"framework," "law," or "standard," whichever the sentence actually names. Standing
project rule, adopted 2026-09-15 per direct author instruction. Verified against the
live manuscript on adoption: zero occurrences of "regime" or "regimes" across all
eighteen chapters and four appendices, so no remediation pass was required at the
time this rule was recorded; the word had already been fully replaced with
"regulation" or "framework" in every instance a prior pass could find. Any new
occurrence introduced after this date is a defect under this rule regardless of how
earlier passes used the word.

**Colons do not join clauses.** A colon is permitted only for a ratio, a time, a
citation, or a title-subtitle pair. It is not a substitute for a period, a semicolon,
or "which is" when introducing an explanation or elaboration. A clause-joining
colon is a tic, not a style choice, and it is unwanted; it does not earn a pass
for subordinating a list or an explanation the way a semicolon or a full stop
does. Standing project rule, adopted 2026-09-04; encoded here 2026-09-13 per
CH432 (Pass 17), which found that
`BOOK_SPECIFICATION_v2.md`'s hard rule 1 (an em dash may be replaced with commas,
semicolons, or colons) does not carry this restriction and that this file did not
yet state it either. **Resolved 2026-09-13: the author confirmed directly that
the clause-joining colon is an unwanted tic and is to be fixed wherever found,
settling in favor of the narrow reading the scope question this file raised
immediately below.** Book-wide remediation is in progress; see
`rules/badw-book-log.md`'s colon-remediation entries for per-chapter status.
Corroborating evidence: `badw.py`-governed audits on another of this
author's projects (`Discussion_v4d_badw_audit.md`, `Discussion_v5_badw_audit.md`,
both dated 2026-09-04/05) already report their mechanical gate results as "No em
dashes or clause-joining colons appear," confirming the concept and its
approximate adoption date independently of CH's own say-so, though not the exact
exceptions list.

**No sentence that restates the previous sentence in different words.**

**Unclear referents.** Scan for "this", "these", "the" where the reader cannot easily
tell what is meant, especially across paragraph boundaries. Bare demonstratives are
the commonest source of re-reading.

**Acronyms.** Spell out on first use in each chapter, because chapters are read
alone. An acronym used once should not exist; write the term.

**Precise and neutral.** "The system produced the same recommendation regardless of
the applicant's stated income", not "the system struggled with income variation".

**Write sentences around actors and actions.** Make the grammatical subject the
actor, object, construct, or process the sentence is about. Keep the subject and main
verb close enough that the reader does not carry an unresolved subject through a long
interruption. Put actions in verbs: prefer "the regulator fined" to "a fine was
imposed by the regulator" when both mean the same thing. Keep a nominalisation when
the action itself has become the object of analysis or is an established term.

**Choose voice by subject.** Use active voice when the actor matters. Use passive
when the acted-upon object is the continuing topic or the actor is unknown or
irrelevant. Neither voice is inherently better.

**Place qualifications where they alter the claim.** Avoid a long hedge at the
beginning that forces the reader to wait for the proposition.

---

## 6. What to cut

**Carried from** `badw.md` section 4. This list is the most direct defence against
generated phrasing.

**Throat-clearing.** "In this section we discuss…", "It is important to note that…",
"The argument that follows explains…". Execute the strategy; do not narrate it.

**Defensive sentences.** "While some might argue…", "This is not to say that…". If no
credible reader would raise the objection, do not pre-empt it. Keep an "X, not Y"
construction only where the reader actually holds Y.

**Meta-commentary.** The chapter makes its argument; it does not announce that it is
about to. If it needs to say "this is important", it has not yet shown why.

**Metaphor standing in for a verb.** A reader who cannot picture the action does not
know what was claimed. "Everything turns on what meaningfully means" reads as
sophisticated and says only "depends on". The same fault produces "the regulation that
bites soonest", "the full apparatus", "two questions are in play", "materially is doing
work in that sentence", "no purchase on the training decisions", and "the boundary a
decision turns on". Each replaces a plain verb with a figure the reader has to decode.
**Test:** read the sentence aloud to someone outside the field and ask what the verb
means. If they hesitate, or answer with the metaphor rather than the action, the word
is not carrying meaning. **On failure:** name the action. Depends on. Applies. Controls.
Decides. Asks. Influences.

**The borrowed-verb test.** Almost no verb originates in AI governance, so "is this word
from the domain" cannot be the test. The usable test is whether the reader has to picture
a physical action to recover the meaning.

Ask: *what is physically happening in this sentence?* If the answer is an image the reader
must translate, the word is borrowed and the translation is work the writer should have
done. A dependency does not rise through water, so it does not **surface**; the trace
finds it. A trigger does not ignite, so it does not **fire**; its condition is met. A
system does not have a seat, so it does not **sit** inside a boundary; it is inside one.
A finding does not fall from a height, so it does not **land** in a tier; it is placed
there. Nothing is **swept** up, **buried**, or **collapsed** in a governance process.

The same word can pass or fail depending on the subject. Software **runs**, because that
is what execution is called. A test is **run**. A record **carries** a date, because
recording is what records do. An obligation **attaches** to a system and a law **reaches**
a deployer, because those are the operative verbs in legal drafting and the alternatives
are longer and less precise. None of those requires the reader to picture anything.

| Fails | Because | Use |
|---|---|---|
| the trace surfaces a dependency | nothing rises | the trace finds it |
| the trigger fires | nothing ignites | the condition is met |
| the system sits inside the boundary | nothing is seated | it is inside |
| the finding lands in the high tier | nothing falls | it is placed there |
| the sweep surfaces shadow AI | two borrowed words | the sweep finds it |
| averaging buries the driving factor | nothing is interred | averaging hides it |

**Test:** for every verb in a sentence, ask what is physically happening. If the literal
answer is absurd, the verb is borrowed. **On failure:** name the action in the words the
reader would use to describe it.

**Vagueness that survives because it sounds authoritative.** Some words pass unnoticed
because they signal expertise rather than convey it: *apparatus* for a set of controls,
*traction* for progress, *in play* for relevant, *goes to* for concerns. **Test:**
replace the word with the plainest available alternative. If the sentence loses nothing,
the word was decoration. **On failure:** keep the plain version.

**Fluff.** "It is worth noting", "in order to", "the fact that", "plays a critical
role in", "a number of", "in the context of".

**Value-laden words.** "Fundamentally reshaped", "deeper problems", "most
consequential", "compelling", "rich", "pivotal". Describe precisely and let the
reader judge depth.

**Supplied transitions.** "Taken together", "These findings demonstrate", "This
suggests that", "Having established X". A reader who has just read the evidence does
not need to be told it constitutes evidence.

**Redundancy.** A claim lives in one place. The chapter opening previews, the body
develops, the summary consolidates. No section does another section's job. Later
appearances back-reference; they do not restate.

### Banned constructions, eliminated on sight

**Carried into this file 2026-09-21** from `control/BOOK_SPECIFICATION_v2.md`, Prose
Style, where this list had lived since the specification was written. It belongs here
because the specification governs what the book contains and this file governs how it
is written, and a writing rule kept only in the specification is not checked by any
pass that loads the rules folder. Adopted on the author's instruction after a scan
found eight live instances across five chapters that every prior pass had missed, all
of them in text that otherwise read as finished. That is section 19's test for
inclusion, met.

Each entry below is a fixed string or a narrow pattern, so all of them are
mechanisable and belong in the gate rather than in a judgement pass.

* "the question is not X but Y", and its variants "not only X but Y" and "not merely
  X but Y" used as a framing device rather than a real contrast the reader holds
* "this creates challenges" and "this presents challenges" as transitions
* "several X emerge"
* "beyond X, Y" as a paragraph opening
* "it is important to note that", "importantly", "notably", "as such", "accordingly"
* "consider X as an example". Give the example
* stacked hedges: two or more of may, might, could, potentially, arguably, in some
  cases, to some extent in one clause

**"Importantly" and "notably" are the pair most likely to survive an earlier pass**,
because they read as emphasis rather than as filler. They are supplied emphasis:
they tell the reader which half of a sentence matters instead of arranging the
sentence so that it shows. Cut the word and, if the emphasis is genuinely needed,
carry it with sentence length or position.

**"As such" and "accordingly" are usually a symptom, not the fault.** Both are
supplied transitions of the kind this section already bans. A reader who has just
read the evidence does not need to be told that a conclusion follows. Cut the word
first, then check whether the sentence still earns its place without it; often it
does not.

**Vocabulary markers are the weakest generation of tell, and this list is not a
vocabulary filter.** Section 19 records that word-level markers were the first
generation and are now largely stripped by the systems that produce them. What makes
these specific entries worth a rule is not that a machine favours them but that each
one does a reader's work for them: supplies emphasis, supplies a transition, or
supplies a contrast that was never in dispute. Do not extend this list by adding
words that merely sound machine-written. A word that carries its defined meaning in
its sentence stays, however common it has become elsewhere. Extend the list only when
an entry fails section 19's test: it would have caught something real in a chapter
that otherwise looked finished.

**Run this as a gate, not as a reading pass.** Every entry is a literal string or a
short regular expression. A pass that reports no banned construction without having
run the strings has reported a check it did not perform, which section 18 forbids.

---

## 7. Texture : why clean prose still reads as machine-written

**Carried from** `badw.md` section 8, with the sentence-rhythm additions of
2026-09-07.

Everything above concerns word choice and claim strength. A chapter can pass all of
it and still be identified as machine-written on sight, because what gives such prose
away is uniformity.

Human writing is uneven. Sentences run four words or forty. Paragraphs run one
sentence or fifteen. There are fragments, asides, and places where the author commits
flatly and others where they hedge, and the difference tracks their actual confidence.

Machine prose is smooth. Every sentence in the same length band, opening with a
subject, resolving cleanly. Every paragraph with a topic sentence, three supports and
a summary. Lists in threes. Transitions supplied where a reader would have inferred.
Nothing disproportionate, so nothing emphasised.

### Repetition of defined terms

Repetition of a defined term is warranted or reflexive, and only judgement tells them
apart. A construct the book defines will and should recur; that is not a tic.
Frequency alone does not condemn a word. The test is per instance. Does each use carry
the term's defined meaning, or is it a reflexive tag the sentence would not miss?

The scripts count occurrences. **Pass 2 reads every counted instance and records, per
instance, what the sentence loses if the term goes; an instance with no recorded loss
is cut.** The count is the worklist, and the pass is complete when every item on it
carries a disposition.

**Scope.** A frequency count opens the worklist; Pass 2 closes it. No count is a
verdict, and no worklist is left open at delivery.

This applies with most force to the book's own coinages and to the domain named in
every second paragraph, because those are the words the writer stops seeing.

### Uniformity signals

**Inspect sentence-length uniformity.** A coefficient of variation below about 0.45
is a mandatory review signal, not a writing target. If lengths are uniform, inspect
whether a template is controlling the prose. Vary length only when the argument,
emphasis, or syntax calls for it. Resolve or justify the warning in the audit.

**Vary paragraph length.** Paragraphs that all run four to six sentences signal a
template.

**Vary openings.** More than a quarter of sentences beginning "The" or "This" means
subject-first throughout.

**List only what the material contains.** Repeated three-part lists can reveal a
completeness template. Do not replace them mechanically with lists of two or five.
Use the exact number of distinctions the material supports.

**Commit somewhere.** Uniform hedging reads as caution rather than calibration. Some
obligations are settled; say so flatly, and the hedges elsewhere start carrying
information.

**Do not manufacture friction.** Admit uncertainty only when it is genuine and
consequential. Never insert "we do not know why" or an unresolved tension to imitate
a human voice.

**Watch nominalisation.** Above roughly five percent of words ending -tion, -ment,
-ance, -ity, -ness, actions have become objects. "The implementation of the
measurement" is "we measured".

**Suspect perfect parallelism.** Three verbs, three objects, perfectly balanced,
reads as designed because it was.

**Do not enumerate a taxonomy one sentence per member.** When a chapter has named a
two- or three-way distinction, the temptation is to give each member its own short
sentence on the same frame: "Planned datasets would include X. Guided repurposing
would invoke Y. Open-ended repurposing would trigger Z." Each sentence can inherit
correctly from the one before it and the passage still reads as machine-made, because
the frame repeats. Subordinate the members into one sentence and let **semicolons**
carry the distinction (not a colon: see the standing colon rule in section 5, added
2026-09-13). Keep the number of members the material supports; the fault is the
repeated frame, not the distinction.

**Conflict discovered 2026-09-13, resolved 2026-09-13 (CH432, Pass 17).** The
sentence above originally told the writer to use "the colon or semicolons" to
subordinate a taxonomy, and this pattern is pervasive throughout the manuscript as
drafted: a grep of this session's own Chapter 2 edits alone found roughly a dozen
colons used exactly this way, introducing a list, an elaboration, or an explanatory
clause rather than a ratio, a time, a citation, or a title-subtitle, and CH's own
Pass 21/22 mechanical counts independently found 14 more in Chapter 8 and 15 more
in Chapter 9. That is a much larger footprint than "ratios, times, citations, and
title subtitles" permits under the standing colon rule as CH432 characterizes it.
Two readings were possible, and this file logged both rather than guessing: (a) the
four-category list is illustrative, and a colon subordinating a genuine enumeration
or a direct explanatory clause remains permitted; or (b) the rule is exactly as
narrow as stated, and every clause-joining and list-introducing colon in all
eighteen chapters and four appendices needs to be rewritten. **The author decided
directly: reading (b). The clause-joining colon is an unwanted tic, not a
permitted style choice, full stop.** A book-wide remediation pass is under way;
see `rules/badw-book-log.md` for per-chapter progress and the running count of
colons found, fixed, and (for the handful that are genuinely a ratio, a time, a
citation, or a title-subtitle) left alone.

**Read runs, not only seams.** Three or more consecutive sentences of sixteen words
or fewer is a review signal. Ask what is producing the run. A scenario being built, a
numbered process being walked, or a genuine three-way dependency are all legitimate
and should be left alone. A taxonomy being expanded member by member, or a paragraph
that has fallen into subject-verb-object throughout, is not. This signal is imprecise
by design: on one manuscript it fired nine times and four were defects. Use it to
locate passages for reading, never as a count to reduce.

**Read it aloud.** If you cannot hear where the emphasis falls, there is none. This
test catches what no word list can.

---

## 8. Generated reasoning, not merely generated phrasing

**Carried from** `badw-htw.md` section 12.

Machine-sounding prose more often reveals a reasoning template than a banned word.

Reject these patterns:

* synthetic completeness, where every topic becomes a balanced taxonomy;
* repeated three-part lists that the material did not produce;
* false contrasts created only to make a sentence sound decisive;
* generic synthesis sentences that add no inference;
* a paragraph that states, illustrates, and restates the same point;
* synonym variation that changes a term's meaning;
* symmetrical treatment of matters with unequal practical importance;
* staged transitions that announce the argument instead of advancing it;
* fabricated uncertainty, puzzlement, anecdotes, or stylistic roughness added to
  appear human;
* an implication that could follow from almost any chapter;
* a caveat that could be pasted into any book;
* a contribution described only as addressing a gap.

Do not optimise against a detector. A detector can encourage another artificial
style. Let variation arise from differences in evidence, confidence, emphasis, and
function.

**Never invent a citation, quotation, case, example, mechanism, disagreement, or
limitation to complete a pattern.**

---

## 9. Claims and sources

**Adapted from** `badw.md` sections 3, 5 and 6 and `badw-htw.md` sections 2, 4 and 9.
The object of calibration changes: a practitioner book answers to law, standards,
documented cases and observed practice rather than to a study design.

**Argument-led, not author-led.** Write "Liability does not transfer with the
purchase (FTC v. Rite Aid, 2024)." Do not write "The FTC argued in Rite Aid that
liability does not transfer." The claim is the book's; the citation is its evidence.
Author-led attribution belongs where intellectual ownership matters: a disagreement,
a lineage, a direct comparison between authorities.

**Keep the levels separate.** Four levels operate in this domain:

* **Text:** what the instrument, standard, or order actually says.
* **Interpretation:** what it is generally taken to require.
* **Practice:** what organizations actually do.
* **Recommendation:** what the book advises.

Name the movement between levels. Do not let a sentence begin with what a regulation
says and end by asserting what organizations must therefore build, without the step
between.

**Match the verb to the authority.** A statute requires. A regulator has alleged, has
found, or has ordered. A standard specifies. A court held. A survey reports. Practice
suggests. The book recommends. Do not use a stronger verb to make guidance sound
settled, and do not weaken one to appear cautious.

**Every source verified.** Real, correctly cited, with the date. Check against the
source, not against memory. An order, a recital number, an article number, and a
version of a standard are all checkable and all get checked.

**Cases.** A documented case is identified as documented, with its source. A
hypothetical is identified as hypothetical. A running case is identified as running.
Never blend the three, and never invent case material to make the prose concrete.

**Do not widen a claim with terms the book never established.**

> **Author** User
> **Adopted by** CH
> **Confidence** 100%
> **Carried from** the addendum of 2026-09-10.

A closing sentence often reaches for extra nouns to sound more general. "Accuracy,
agreement, and throughput can all improve" in a chapter that discussed only accuracy
is such a sentence. The additional terms were never defined, never used, and never
appear again. The claim gains scope and loses support.

Two failure modes, and the second is worse:

1. **The term appears once.** A construct occurring a single time, in a summary, was
   decoration. If the argument never needed it before, the claim does not need it now.
2. **The term appears elsewhere in a different sense.** "Agreement" meaning
   inter-rater reliability is not "agreement" meaning consensus among reviewers. A
   reader who has met the first will take the second as established. This is construct
   drift wearing the costume of consistency, and it is harder to see than an
   unfamiliar word.

**The test.** For every content noun in a concluding or summarising sentence, count
its occurrences in the chapter and confirm that each use carries the same defined
meaning. One occurrence, or several across two senses, means cut the term or
establish it earlier. Do not repair the sentence by defining the term in the summary.
A construct introduced at the end has no development behind it, and a definition
placed there is a confession rather than a fix.

**Scope.** Counting lists the candidates; **Pass 4 reads each candidate in its
sentence and records keep or cut with the reason, and reads each term used in two
places to confirm both uses carry the same defined meaning.** The rule is satisfied
when every candidate has a recorded disposition, not when the count has been run.

**Define every construct fully.** For each: what it includes; what it excludes; the
level at which it exists; how it differs from its closest neighbour; how it can be
observed or tested; and one stable label used thereafter. Do not replace a construct
name with elegant synonyms. Terminological repetition is preferable to construct drift.

**Do not grade the book's own work.** "Comprehensive", "rigorous", "essential",
"definitive", "best practice". Report what the control does and let the reader judge.

**Vocabulary from the right field.** Mathematics proves; empirical work shows or
supports. Verdicts are legal, deliverables commercial, targets military.

**State what is contested as contested.** Where practitioners disagree, or where a
regulator has not tested a position, say so and say what would settle it. Do not
present an unsettled reading as settled because the guidance reads better.

**Do not hedge what the sources support directly.** "May be" and "might" where the
text is explicit reads as uncertainty about the law itself. Qualify at the exact point
where the authority stops.

---

## 10. Currency

**New for this file.** Author Claude. Confidence high, because the failure is
observable: a book about law and standards decays in a way a book about constructs
does not.

**Date every moving claim.** Any statement about what a regulation requires, when an
obligation applies, what a standard contains, or what an enforcement body has done
carries the date on which it was checked. **Test:** for each such claim, name the
check date. **On failure:** check it or remove it.

**Separate the stable from the moving.** Constructs, mechanisms and failure modes are
stable. Deadlines, thresholds, enforcement postures, and standard version numbers are
not. Where both appear in one passage, the reader must be able to tell which is which.

**Write so that a superseded fact does not invalidate the reasoning.** A chapter that
teaches why a deadline moved survives the deadline moving. A chapter that only states
the deadline does not.

**Verify publication status before relying on a standard.** A standard under
development is not a standard.

---

## 11. Figures, tables, and worked examples

**Adapted from** `badw.md` section 11 and extended. The extensions carry the author's
instruction of 2026-09-12 that diagrams must not read as machine-made.

### What earns a figure

Tables earn their place by making a relationship visible that prose obscures:
mappings, comparisons, syntheses. Figures earn theirs by carrying a model or process
that would take paragraphs. A figure that restates a sentence is decoration.

### Numbering and reference

**Every figure is numbered, and the number is chapter-based.** Figure 1.1, 1.2, 2.1.
Tables likewise.

**Every figure is introduced in the text before it appears,** with what it shows and
why it matters here. **Every figure is referred to by its number,** not as "the figure
below". A reader who returns to the chapter has no "below".

**Every figure is walked through in prose.** The walkthrough names what to read
first, what the arrangement means, and what the reader should take from it. A figure
that needs no walkthrough was not carrying enough to earn its place; a figure whose
walkthrough merely lists its labels is not being explained.

**No figure forward-references a concept the reader has not met.**

**Adapted frameworks are credited** in the caption, and where the book's version
differs from the source, the divergence is stated.

### The figures must not read as machine-made

**Author** Claude, from the user's instruction
**Confidence** high for the diagnosis, medium for the completeness of the list

Generated diagrams have tells, and they are the visual form of the prose tells in
sections 7 and 8:

* **Synthetic completeness.** Balanced taxonomies, equal boxes for unequal things,
  every row filled because the grid has rows. The visual form of the three-part list.
* **Decorative colour.** Colour that marks nothing, or the same blue-to-purple
  gradient across every figure.
* **Uniform weight.** Every arrow the same, every box the same size, so nothing is
  emphasised. The visual form of uniform sentence length.
* **Ornament.** Drop shadows, gradients, rounded glossy boxes, 3D, icons that carry
  no information.
* **Perfect symmetry.** Elements distributed on a grid because a grid was available,
  not because the relationships are symmetric.
* **Labels that restate.** A box labelled "Data Quality Process" inside a figure
  titled "The Data Quality Process".

### The rules

**The figure must work in black and white.** Draw it in black, white and grey. Carry
every distinction by position, weight, shape, spacing, and label. **Test:** render it
monochrome and read it. **On failure:** the distinction that disappeared was being
carried by colour alone; encode it structurally and redraw.

This is also an accessibility requirement, not only a style preference: information
conveyed by colour alone is unavailable to readers who cannot distinguish those
colours, and to anyone reading a printed copy.

**Colour is permitted only where it carries a distinction that position, weight and
label cannot,** and where it is defined in the figure itself. One accent at most.
**Test:** state what the colour means. **On failure:** remove it.

**Erase every mark that carries no information.** Rules, boxes, shadows, fills, and
gridlines that do not encode anything are removed. What remains should be almost
entirely the content. **Test:** delete a mark and ask what the reader no longer knows.
**On failure to answer:** the mark goes.

*Basis.* Edward Tufte, *The Visual Display of Quantitative Information*, on the
data-ink ratio and on chartjunk.
[Publisher record](https://www.edwardtufte.com/book/the-visual-display-of-quantitative-information/).

**Let weight follow importance.** The element the chapter turns on is heavier,
larger, or positioned where the eye lands first. If every element is equal, the
figure has no argument.

**Put the label on the thing.** Labels sit adjacent to what they name, not in a
legend the reader must hold in memory while looking elsewhere. Splitting related
material forces the reader to integrate two sources at once and costs capacity that
should go to the content.

*Basis.* Richard Mayer, *Multimedia Learning*, 3rd edition, on the spatial contiguity
and signalling principles.

**Asymmetry where the content is asymmetric.** If three of five stages carry the risk,
the figure should show that. Do not lay out five equal boxes.

**One figure, one job.** A figure doing two jobs is two figures.

**Accessibility is not optional.** Every figure carries `role="img"` and a
nonempty accessible name, provided by `aria-labelledby` pointing at a `<title>`
and `<desc>` pair (preferred, since it gives assistive technology both a name and
a description) or, failing that, by `aria-label` repeating the caption. Adding a
redundant `aria-label` alongside a working `aria-labelledby` is not required. The
book is published on the web; verify with at least one browser and screen reader
before publication.

*Correction, 2026-09-12:* this rule previously required `aria-label` literally,
which would have flagged the correct `aria-labelledby` pattern already in use as
a defect. Corrected on review; see `logs/CH-review-pass-1.md` ISSUE CH021.

**A required-elements list is written before the figure is drawn** and placed as a
comment immediately above the figure in the source, so that it travels with the
figure and survives revision. It states what must appear, what is deliberately
excluded, and why.

---

## 12. Cross-chapter obligations

**New for this file.** Author Claude. These have no analogue in a paper, which is
read once and whole.

**Terminology is stable across the whole book, not just the chapter.** A construct
named in chapter 1 keeps that name in chapter 14. **Test:** for each defined term,
list its occurrences across all chapters and confirm one meaning and one label.
**On failure:** unify and record the change.

**No pointer aims at nothing.** A sentence pointing at a later chapter is a promise.
It is kept when that chapter exists and covers what was promised. **Test:** for every
cross-reference, confirm the target exists and contains the material. **On failure:**
drop the pointer, move the material, or cut the promise from the source text. Draft
the chapter first, then reconcile the ledger; a chapter written with the promises in
view is organised around someone else's sentences rather than its own argument.

**A pointer names what the reader will get, not just a number.** "Chapter 9 sets out
the monitoring that would have caught this" is usable. "See Chapter 9" is not.

**A forward pointer must do work the reader needs now.** A backward reference costs
the reader nothing, because the material is behind them and they can recall it or
skip it. A forward reference costs attention, because it names something they cannot
check. It is therefore warranted only in three cases. It licenses an omission: the
reader has just met a question this chapter will not answer, and the pointer tells
them they are not expected to know it yet. It hands off evidence: the chapter states
what it produced and which chapter consumes it. It closes the chapter by naming what
comes next and why. **Not warranted:** a pointer that only advertises later content.
"Chapter 12 develops this", "Chapter 9 shows why that matters", "Chapter 12 returns
to this system" are advertisements. They interrupt a sentence to promise a payoff
elsewhere, and deleting them removes nothing the reader can use. **Test:** delete the
pointer. If the surrounding prose still stands and the reader is left with no
unanswered question, the pointer was an advertisement. **On failure:** cut it.

**Forward-reference density falls as the book proceeds.** Early chapters legitimately
defer more, because most of the book is still ahead. By the later chapters forward
pointers should be rare and backward ones common. **Test:** count forward and
backward references per chapter and check the profile tapers. **On failure:** an
increase in forward references late in the book means material is in the wrong
chapter, not that the pointer is badly worded.

**A pointer describes the subject, not the book's structure.** "This is where
Chapter 12 connects forward to Chapter 9" is bookkeeping about the manuscript.
**On failure:** state the substantive relation instead, or cut the sentence if the
next one already carries it.

**Numbers written by hand stay consistent.** Where section and figure numbers are
typed rather than generated, a renumbering is a manual operation across every
cross-reference. **Test:** after any renumbering, search for the old numbers.
**On failure:** fix every occurrence before delivery.

---

## 13. Readability

**New for this file.** Author Claude. The rules are procedural; the caution about
formulas is sourced.

**The measure.** Body text sits between 50 and 80 characters per line. Beyond about
80 the eye loses the start of the next line on the return sweep. **Test:** measure a
rendered paragraph. **On failure:** change the column width, not the prose.

**Readability formulas are locators, not targets.** A grade-level score counts
syllables and sentence lengths. It cannot see whether a term was defined, whether the
order is right, or whether the reader can act on the paragraph. Writing to a formula
shortens sentences and simplifies words without making the passage clearer, and can
make it worse by removing the connectives that carried the logic. **Use:** run one to
locate the densest passages. **Do not:** set a score as a goal or edit to move it.

*Basis.* Janice Redish, "Readability formulas have even more limitations than Klare
discusses", *ACM Journal of Computer Documentation*, on the gap between what formulas
measure and what makes text usable.
[Author's copy](https://redish.net/wp-content/uploads/Redish_on_Readability_Formulas.pdf).

**Technical terms are exact or they are jargon.** Use the term when it is precise and
the reader needs it in practice. Replace the term that only marks membership of a
field. Plain language and technical precision are compatible.

**Do not tutor the reader through what they already know.** Supply the background the
present problem requires and no more.

---

## 14. Verifying

**Carried from** `badw.md` section 9.

**An extraordinary result impugns the instrument first.** If a check reports a
missing section or a changed number, suspect the check. Confirm the tool on
known-good input before acting.

**Confidence is not evidence.** State what was compared, against what, by what
method. Repeating an assertion more firmly after being questioned is the least
reliable signal available.

**Label the kind of check.** Mechanical checks — is this string present, do these
numbers match, is every reference cited — are trustworthy and should be automated.
Judgement checks are not. Never report the second with the confidence of the first.

**A recommendation is not a state.** Advice given is not a change made. Before editing
any document that quotes another, re-read the other as it now exists.

**Diff; do not infer from filenames.** "Final", version numbers and dates in names are
not evidence of lineage.

**After inserting, find what the insertion made redundant.** The commonest revision
fault: a good new sentence is added and the one it replaces is left standing.

**Before deleting, find what the deletion leaves unsupported.** Text that looks
redundant is often the evidence for a conclusion downstream, or the payoff for a
promise made in the chapter opening.

---

## 15. Know when to stop cutting

**Carried from** `badw-htw.md` section 15, with the closing correction of
`flow/w-replacements.md`.

Tight writing contains no material that can be removed without cost. The cost may be
semantic, logical, evidential, rhythmic, or pedagogic.

Before cutting, ask:

* Does the passage supply a premise the conclusion needs?
* Does it preserve a qualification that determines whether the claim is true?
* Does it distinguish this construct from a neighbouring one?
* Does it identify the comparison, unit, scope, or date?
* Does it create necessary emphasis or processing time?
* Does it answer a question the intended reader will actually ask?

If yes, retain or rewrite it. Brevity is not the goal. Precision is.

### Economy requires an independent loss test

**An economy edit is not accepted until the loss has been named and shown to be
nothing.** Shorter, cleaner, more direct and tighter are descriptions of the revision,
offered by the person who made it. They are not evidence.

Before accepting an economy edit:

1. preserve the original sentence;
2. identify every proposition, qualification, relation, referent, transition,
   and emphasis carried by the original;
3. compare the original and revision inside the full paragraph;
4. apply the mandatory neighbour-set check to the revision;
5. state exactly what was removed and why the passage loses nothing; and
6. accept the edit only when every item listed at step 2 has a named carrier in the
   revision. **Where an item has no carrier, the cut is not made.** Doubt is not a
   reason to defer. It is the answer, and the answer is no.

---

## 16. Do not optimise for the rules

**Carried from** `badw.md` section 13.

These rules serve the reader. They are not targets to optimise. A book is not good
because it avoids flagged words, varies its sentence lengths, or passes a scanner. It
is good when it makes a consequential claim, supports it, states its limits precisely,
and leaves the reader able to do something they could not do before.

Blacklists, counts, and thresholds trigger mandatory review. Never add a synonym,
split a sentence, enlarge a list, or manufacture uncertainty merely to change a score.
Variation must arise from the content. No hit may be ignored: fix the underlying
problem or record a specific exception.

When a rule conflicts with accuracy, traceability, disclosure, or what the reader
needs in order to act, the obligation to the reader wins. Record the exception and its
reason.

---

## 17. No rule may explain a failure in advance

**Author** User
**Confidence** 100%
**Rule type** Operational control
**Carried from** `flow/w-replacements.md`.

A rule names an action, the condition under which it is complete, and what to do when
the condition fails. Anything of the form "I am poor at X", "this is hard to judge",
or "only a reader can do Y" supplies the reason for a failure before the failure
occurs, and will be used that way.

**Test.** Strike the sentence. If the procedure still says what to do, the sentence
was an excuse and goes. If the procedure is now incomplete, the sentence is
load-bearing and stays.

**Judgement must be scheduled.** A statement that something needs judgement is
permitted only when it names the pass that supplies the judgement and the record that
pass leaves. An unscheduled limitation is permission not to do the work.

**Not covered.** Calibration of a rule is required and stays: a confidence level, a
recorded test failure on a named manuscript, a marking of convention rather than
evidence, a false-positive rate. Those are statements about the rule. The prohibition
is on statements about the writer.

---

## 18. The audit record

For every chapter worked on, create or update `badw-book-audit.md` beside the working
draft. It must contain:

* the chapter and the version worked on;
* every rule file loaded, with the date of the version loaded;
* the chapter's central claim and what the reader can do afterwards;
* the seven-line spine;
* the paragraph-role map;
* the promise ledger: what the chapter promises, and where each is paid off;
* the source ledger: every legal, standards, or case claim with its source and check
  date;
* the exact gate commands run and their output;
* every unresolved warning, the decision, and the reason;
* every sentence retained above 45 words, with the relation that splitting would break;
* every term with a recorded keep-or-cut disposition from the repetition and
  unestablished-terms passes;
* a final statement that quotations, citations, numbers, dates, figures and tables
  were checked against their sources.

No unexplained warning counts as a pass. No audit statement may claim a check that was
not actually performed.

### 18a. Enforcement: the audit record is evidence, not a declaration

**Adopted 2026-09-21.** Carried from the enforcement model in `w/ac/README.md`, not
from its gates. That module governs research manuscripts at audit and submission
stage and does not govern this book; its scope line and this file's own gate both say
so. What transfers is the reason it exists. Its opening records a manuscript "recorded
as passing W" whose gates "were not too weak" but "were recorded CLOSED without the
evidence they require, and that closure was inherited across later versions." Section
18 had the same hole: it required an audit record, nothing verified one, and none was
written for fifty-six passes.

**Assume the agent writing the audit is untrustworthy.** Every claim in an audit entry
must leave an artifact that can be checked without re-reading the chapter. An entry
that cannot produce its artifact records NOT RUN, not a pass. This applies to an agent
auditing its own work most of all, which is the ordinary case here.

**A partial pass is NOT RUN, not a light pass.** A pass that covered some sections is
recorded as not run. There is no credit for partial coverage, because a reader cannot
tell which half was checked.

**Separation of duties.** The pass that logs a finding does not fix it in the same
breath and then close it. Where one agent must do both, the audit entry names the
order and states that the check was re-run after the fix, against the original
wording of the finding rather than against the corrected text. An agent that edited a
sentence may not record that sentence as checked without re-running the neighbour-set
check on the result.

**Closure binds to the text it was measured against.** Record the word count or a hash
with every gate block. Any later edit to the chapter invalidates that block. Mechanical
counts may be re-run on the changed region alone. Flow, terminology, claim scope, and
the neighbour-set check may never inherit closure across a content change, because
they are properties of the whole text rather than of unchanged bytes. An added
sentence re-opens the paragraph it joined, not merely itself.

**The rejection register.** A finding the author rejects is recorded with the reason
and may not be raised again by a later pass. Without this the loop does not converge
and the log fills with the same disputed item under new numbers. A rejected finding is
closed, not open.

**Iteration cap.** Three rounds on any one finding. At the cap the pass escalates to
the author with the open item and stops. It does not close itself, and it does not
keep rewriting.

**What the gate block must contain.** Every audit entry recording a mechanical pass
states the exact checks run, the command or script that ran them, the output, and the
text state it was run against. "Gates pass" is not a gate block. A gate block that
reports a check the entry cannot evidence is the failure this section exists to catch.

**An extraordinary count impugns the instrument first.** Section 14's rule, restated
here because it fires most often in this context. A pattern reporting a large number
of defects in finished text is usually matching something outside its scope. Inspect
the matches before recording findings, and record the instrument fault rather than the
false count.

### 18b. Independent readers are separate agents, not one agent wearing hats

**Adopted 2026-09-21 on the author's instruction.** `w/core` CORE-02A requires three
reading perspectives for long-form work, and `w/ac` requires that G0 and G2 name
different readers and that G1 and G4 name different readers. Neither is satisfied by a
single agent producing three sections under three headings. One reader who has already
formed a view of a chapter cannot then read it without that view; the second and third
perspectives inherit the first's conclusions and the exercise becomes theatre.

**Where the environment can spawn agents, spawn one per perspective.** Each receives
the file path and its own brief, reads the chapter independently, and returns findings.
No agent sees another's output before reporting. The differences between their reports
are the evidence that they were independent; three identical reports mean the
separation failed.

**Where agents cannot be spawned, open a fresh instance of the model per perspective**,
with no history of the current session, and give it the perspective brief as its whole
task. A fresh context is the mechanism; the persona is only the brief. Carrying a
persona inside an existing context does not produce a second reader, because the
context already holds the first reader's conclusions.

**The three CORE-02A perspectives.** Domain expert, checking professional and
scientific logic, construct boundaries, evidentiary sequence, and whether each
inferential move is warranted. Educated adjacent-field reader, checking whether a
capable non-specialist can follow the argument without reconstructing hidden premises.
Smart high-school friction reader, locating undefined concepts, abrupt topic changes,
unclear referents, missing context, and unexplained notation.

**The friction reader is constrained, not licensed.** Its brief must state that it may
not recommend lowering the scholarly level or simplifying away a technical distinction.
Its value is locating where the text assumes knowledge it never supplied, a defect that
harms expert readers too; they simply do not notice themselves compensating. A friction
brief without that constraint produces a request to dumb the book down, which is worse
than not running the pass.

**Separation of duties follows.** The agent that logs a finding does not fix it. Where
one identity must do both, the audit entry records that, names the order, and confirms
the re-check ran against the original finding's wording. An entry claiming clean
separation while one identity did everything is the failure section 18a exists to stop.

**Record what each reader found separately.** The audit entry names the perspective,
its findings, and which findings two or more readers reached independently. Consensus
across independent readers is the strongest signal available in this method and it is
lost if the reports are merged before recording.

---

## 19. Maintaining this file

Add every new tell of machine-written prose, from wherever it surfaces: detection
papers, editorial policies, reader complaints, corpus studies. The tells move as the
models move. Vocabulary markers were the first generation and are now stripped by the
systems that produced them; the current generation is structural; the next will be
something else.

New claims enter as an intake entry with their source, evidence class, confidence,
mechanisability, and false-positive risk. Promote a pattern into a rule only when it
is specific, recurrent, relevant to book writing, and useful enough to outweigh the
risk of damaging correct prose.

Take rules from strong books, but take **rules, not voices**. "The best textbooks in
this field define a construct, show one worked case, then give the reader a case to
decide" is usable. "Write like Kahneman" is not: imitating a voice is the operation
that produces generated-sounding prose.

**Do not add taste as rule.** Prohibitions on the passive voice, on the first person,
on beginning a sentence with "But" are folklore, contradicted by the best writing in
every field, and following them produces exactly the stilted register readers now read
as machine-written.

**Test for inclusion:** would this rule have caught something real in a chapter that
otherwise looked finished? A checker that fires on correct writing teaches the writer
to ignore it.

---

## 20. Final standard

A finished chapter should allow a sceptical practitioner to answer these questions:

* What exactly is this chapter claiming?
* What is stated in the source, and what is the book's interpretation of it?
* Which authority licenses each obligation, and as of when?
* What can I do after this chapter that I could not do before?
* Which distinction does the chapter turn on?
* Where does the guidance stop, and what is still contested?
* Can every term, number, date, quotation, case and citation be traced?
* If I read only this chapter, does it stand?

If the chapter cannot answer them, it is not finished. A clean gate report cannot
change that.
