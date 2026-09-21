# forBook : entry point, iteration loop, and logging contract

## SCOPE. READ THIS BEFORE ANY OTHER LINE IN THIS FOLDER.

**This folder governs textbooks and nothing else.** A textbook here means a book that
teaches a practitioner or student to perform, decide, or assess something; whose
chapters are read alone as often as in sequence; that defines constructs the reader
applies to cases; that carries figures, worked cases and end-of-chapter questions; and
that is revised as the underlying law, standards or practice change.

**If the work in front of you is not that, stop.** Do not adapt these rules to it. Do
not apply the parts that seem to fit. For a scientific manuscript use the parent `w/`
suite. Name the correct suite and use it.

The scope gate is recorded, not assumed. The first line of every log entry states
which of the five properties the work has. Fewer than five is a stop.

---

## What is in this folder

| file | what it is |
|---|---|
| `README.md` | this file: the entry point, the loop, and the logging contract |
| `badw-book.md` | the rules |
| `badw-book-log.md` | the running issue log, created on first use |
| `badw-book-audit.md` | the per-chapter audit record required by `badw-book.md` section 18 |

**Order for an agent entering cold:** this file, then `badw-book.md`, then the log.
Do not begin from any other file. Do not begin from a rule you remember.

---

## Who writes here

| initials | agent |
|---|---|
| `CH` | ChatGPT |
| `cl` | Claude |
| `User` | Shawn Ogunseye |

Sign every log entry, every rule you add, and every disposition you record. An
unsigned entry is treated as not made.

---

## The loop

**check everything → log every issue → fix → check everything → repeat**

The loop runs until a complete check produces zero open issues. It does not run until
the agent judges the text good enough.

### 1. Check everything

**Check everything means everything, every time.** Every check in the register below,
over every chapter in scope, on every pass. Not a sample. Not the chapters that
changed. Not the checks that failed last time. Not a representative passage.

The reason is mechanical, not moral. A fix changes the text around it. A sentence
repaired in chapter 3 can break a term defined in chapter 1, orphan a pointer in
chapter 7, and change the skeleton of its own paragraph. `badw-book.md` section 14
states it directly: after inserting, find what the insertion made redundant; before
deleting, find what the deletion leaves unsupported. A partial re-check cannot find
either.

**Forbidden, and each is a lazy check:**

* checking only the chapters edited since the last pass;
* checking only the rules that produced issues last time;
* reading the first and last paragraph of a section and inferring the middle;
* accepting a script's clean output as a pass on a judgement rule;
* recording a check as passed when it was skipped, deferred, or partially run;
* recording a check as passed because it passed on an earlier version;
* stopping a pass early because the issue count is already high.

**A check that was not run is recorded as NOT RUN.** Never as passed. A pass with any
NOT RUN entry is an incomplete pass and the loop does not advance.

### 2. Log every issue

Every issue found gets an entry, immediately, before any fix is attempted. Logging
before fixing is what makes the pass countable and stops the agent from repairing what
it happens to notice and forgetting the rest.

An issue is logged even when:

* it is trivial;
* it is about to be fixed in the same minute;
* it is a duplicate of an issue in another chapter;
* the agent believes it is a false positive. Log it, then record the disposition
  `not-a-defect` with the reason. An unrecorded false positive is indistinguishable
  from a missed check.

### 3. Fix

Fix the underlying problem, not the symptom. `badw-book.md` section 16 forbids
editing to move a score.

Every wording change, down to one word, triggers the mandatory neighbour-set check in
`badw-book.md` section 4, applied to the revised sentence with both neighbours at
once. Every economy edit triggers the loss test in section 15, and where an item has
no named carrier in the revision, the cut is not made.

A fix does not close its issue. Only the next complete check closes it.

### 4. Check everything again

Return to step 1. Run the whole register again, over everything in scope.

### Stopping condition

The loop ends when one complete pass over the whole register, over every chapter in
scope, produces zero open issues and zero NOT RUN entries. Record that pass number in
the log and in the audit.

Anything else is an interim state. If work has to stop before then, the log's final
line states the pass number, the open issue count, and what remains unchecked.

---

## The check register

Run every line. Record a result for every line, for every chapter. The section numbers
refer to `badw-book.md`.

**Structure and narrative**

1. Skeleton test: first sentences of every paragraph, in order, tell the chapter (§1)
2. Paragraph-summary test: numbered one-line summaries cohere (§1)
3. Paragraph continuity: each paragraph opens on the previous paragraph's close (§1)
4. No direction reversal inside a paragraph (§1)
5. One move per paragraph (§1)
6. Chapter survives being read alone; every dependency defined or located (§1)
7. Seven-line spine complete, complication is a problem not an absence (§2)
8. Protagonist test: object of attention named in every paragraph (§2)
9. Promise-payoff test: every opening promise paid off in the chapter (§2)
10. State-change test: every paragraph changes knowledge, confidence, question or scope (§2)
11. Problem before framework; frameworks enter and exit (§2)
12. Space follows importance, not template (§2)

**Teaching**

13. Every defined concept is used later (§3)
14. Every definition decides a case the reader can bring to it (§3)
15. Every procedure has a worked instance before the general rule (§3)
16. Scaffolding marked for the reader it serves; expert can skip without loss (§3)
17. Transformative concepts identified and given room (§3)
18. End-of-chapter questions require retrieval, not recognition (§3)
19. Terms defined before the procedure that uses them (§3)
20. Interesting-but-not-load-bearing material cut (§3)

**Flow**

21. Neighbour-set check on every changed sentence, all four criteria, together (§4)
22. Paragraph read aloud as a unit after the seam checks pass (§4)

**Sentences**

23. Every sentence over 45 words reviewed; retained ones recorded with the relation (§5)
24. No em dashes; no en dashes except page and date ranges (§5)
25. No sentence restating its predecessor (§5)
26. Unclear referents: bare "this", "these", "the" across boundaries (§5)
27. Acronyms spelled out on first use in each chapter; single-use acronyms removed (§5)
28. Precise and neutral description, no evaluative shorthand (§5)
29. Actors near actions; nominalisations justified (§5)

**Cuts**

30. Throat-clearing (§6)
31. Defensive sentences and pre-empted objections (§6)
32. Meta-commentary (§6)
33. Fluff list (§6)
34. Value-laden words (§6)
35. Supplied transitions (§6)
36. Redundancy across chapter parts (§6)

**Texture and AI language**

37. Repetition of defined terms: every counted instance given a disposition (§7)
38. Sentence-length coefficient of variation; template inspected if uniform (§7)
39. Paragraph-length variation (§7)
40. Sentence openings: "The"/"This" share (§7)
41. Repeated three-part lists (§7)
42. Uniform hedging; the book commits where the sources are settled (§7)
43. Manufactured friction (§7)
44. Nominalisation density (§7)
45. Perfect parallelism (§7)
46. Taxonomy enumerated one sentence per member (§7)
47. Runs: three or more consecutive sentences of sixteen words or fewer (§7)
48. Read aloud for where the emphasis falls (§7)
49. The twelve generated-reasoning patterns (§8)

**Claims and sources**

50. Argument-led citation by default (§9)
51. Text, interpretation, practice and recommendation kept separate (§9)
52. Verb matches the authority (§9)
53. Every source verified against the source, with date (§9)
54. Documented, hypothetical and running cases each labelled as such (§9)
55. No claim widened with terms the book never established; every candidate disposed (§9)
56. Every construct fully defined: includes, excludes, level, neighbour, test, label (§9)
57. The book does not grade its own work (§9)
58. Vocabulary from the right field (§9)
59. Contested positions stated as contested (§9)
60. No hedging of what the sources support directly (§9)

**Currency**

61. Every moving claim carries a check date (§10)
62. Stable and moving material distinguishable in the same passage (§10)
63. Reasoning survives a superseded fact (§10)
64. Standards' publication status verified (§10)

**Figures and tables**

65. Every figure and table earns its place (§11)
66. Chapter-based numbering, consistent (§11)
67. Introduced in the text before it appears (§11)
68. Referred to by number, never "below" (§11)
69. Walked through in prose; the walkthrough explains rather than lists (§11)
70. No forward reference to an unmet concept (§11)
71. Adapted frameworks credited; divergences stated (§11)
72. **Black-and-white test:** rendered monochrome and still readable (§11)
73. Colour, if any, carries a distinction structure cannot, and is defined in the figure (§11)
74. No mark that carries no information (§11)
75. Weight follows importance (§11)
76. Labels adjacent to what they name (§11)
77. Asymmetry where the content is asymmetric (§11)
78. One figure, one job (§11)
79. `role="img"`, `aria-label`, and `<title>` present (§11)
80. Required-elements comment present above the figure in source (§11)

**Cross-chapter**

81. Terminology stable across every chapter, one meaning and one label (§12)
82. No pointer aims at nothing (§12)
83. Every pointer names what the reader will get (§12)
84. Hand-written numbers consistent after any renumbering (§12)

**Readability**

85. Measure between 50 and 80 characters per line (§13)
86. Readability score used to locate, never as a target (§13)
87. Technical terms exact, not membership markers (§13)
88. No tutoring through what the reader knows (§13)

**Verifying**

89. Tool confirmed on known-good input before acting on a surprising result (§14)
90. Mechanical and judgement checks labelled differently (§14)
91. Quoted documents re-read as they now exist (§14)
92. Lineage established by diff, not filename (§14)
93. After every insertion, what it made redundant (§14)
94. Before every deletion, what it leaves unsupported (§14)

**Process**

95. No edit made only to move a score (§16)
96. No rule, note or comment explains a failure in advance (§17)
97. Audit record complete for the chapter (§18)

---

## The log

One file, `badw-book-log.md`, in this folder. Append only. Never rewrite history;
close an issue by adding its closing entry.

### Pass header

    ## Pass N — YYYY-MM-DD — agent: cl
    Scope gate: 5/5 properties present (teaches; chapters read alone; constructs
    applied to cases; figures and questions; revised as law changes)
    Files loaded: README.md (2026-09-12), badw-book.md (2026-09-12)
    Chapters in scope: index, 00, 01, 02, 03, 04
    Register: 97 checks x 6 chapters = 582 results required

### Issue entry

    ### ISSUE 014
    chapter: 02
    location: section 2.7, paragraph beginning "The practical position"
    check: 46 — taxonomy enumerated one sentence per member (§7)
    found by: cl, pass 1, 2026-09-12
    what: three consecutive sentences on the "would" frame, one per tier
    quote: "Planned datasets would include... Guided repurposing would invoke..."
    status: OPEN

### Fix entry

    #### FIX for ISSUE 014
    by: cl, 2026-09-12
    change: subordinated the three members into one sentence, semicolons carrying
            the distinction; tier names unchanged
    neighbour-set check: inheritance "tier" carries from the previous sentence;
            vocabulary unchanged; verb "triggers" states the real relation;
            ending lands on the monitoring requirement, which is new
    loss test: not applicable, no material removed
    status: FIXED, AWAITING RE-CHECK

### Close entry

    #### CLOSE for ISSUE 014
    by: cl, pass 2, 2026-09-13
    re-checked: check 46 over chapter 02 in full; no run remains
    side effects checked: 21, 22, 37, 38, 47 over the changed paragraph and both
            neighbours; 81 over all chapters for the tier names
    status: CLOSED

### Pass footer

    ### Pass N result
    checks run: 582 of 582
    NOT RUN: 0
    issues opened: 21
    issues closed: 14
    open at end of pass: 7
    loop state: CONTINUE

`loop state: COMPLETE` may be written only when open is 0 and NOT RUN is 0.

### Dispositions

| status | meaning |
|---|---|
| `OPEN` | found, not yet fixed |
| `FIXED, AWAITING RE-CHECK` | changed, not yet confirmed by a complete pass |
| `CLOSED` | confirmed gone by a complete pass |
| `NOT-A-DEFECT` | the check fired and a reader judged it correct; reason recorded |
| `RETAINED` | a real hit, deliberately kept; reason and authority recorded |
| `DEFERRED TO USER` | needs a decision only the author can make; the question stated |

`NOT-A-DEFECT` and `RETAINED` both require a written reason. Neither may be used to
clear a backlog.

---

## Iterating the rules

The rules change. That is expected, and the loop is how it happens safely.

**A rule may be added, sharpened, or removed.** Every change is logged in
`badw-book-log.md` as a rule entry, not as an issue, and carries:

* the pattern or fault, stated specifically enough to test;
* a short constructed example;
* where it was found: which chapter, which pass, by which agent;
* evidence class: reader observation, corpus study, published source, or convention;
* confidence, stated separately for the fault and for any claim about AI style;
* whether it is mechanically detectable, and if partially, what a script can and
  cannot see;
* false-positive risk, with a measured rate if one exists;
* overlap with existing rules, named by section;
* proposed action: judgement rule, review warning, or hard failure.

**Promotion test.** Would this rule have caught something real in a chapter that
otherwise looked finished? A checker that fires on correct writing teaches the writer
to ignore it.

**A new rule enters the register.** Adding a rule to `badw-book.md` without adding its
line to the check register above means it will not be run. The register is the
contract; the rules file is the explanation.

**Renumbering the register is a fix that triggers check 84.** Old numbers appear in
the log. Search for them.

**Do not add taste as rule.** Prohibitions on the passive voice, on the first person,
on beginning a sentence with "But" are folklore. Following them produces the stilted
register readers now read as machine-written.

---

## What a handover must contain

When work stops, whoever picks it up must be able to continue without asking. The last
entry in the log states:

* the pass number and whether it completed;
* open issues by chapter, with their check numbers;
* anything recorded NOT RUN, and why;
* every `DEFERRED TO USER` question, unanswered;
* what the next agent should do first.

An agent that cannot produce that from the log should say so rather than start a new
pass on top of an unknown state.
