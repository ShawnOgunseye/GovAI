# Sources and Attribution
## Reuse rules, source register, and currency sweep brief

---

## 1. The rule that governs everything else

**Publicly available does not mean freely reproducible, and attribution is not a license.**

A framework you can read for free may still be copyrighted. ISO standards are sold. The three lines model belongs to the Institute of Internal Auditors. Academic figures belong to publishers. Crediting the source does not create a right to reproduce it.

The licensing question settles it independently. **Version 2.0 is all rights reserved** as of 23 September 2026, having been CC BY-NC 4.0 before that, and the Appendix C templates are still offered under CC BY-NC 4.0. Releasing anything under a Creative Commons license means sublicensing it, and you cannot sublicense someone else's copyright, so every figure in the appendix must be original work. Dropping the book-wide CC license does not relax this: reproducing someone else's figure without permission is an infringement whatever the book is licensed under. So every figure must be original work.

The bar is set by Appendix C, not by the book-wide licence. The book is all rights reserved, but the Appendix C templates are offered under CC BY-NC, so readers are licensed to adapt, remix, and build on everything in that appendix. A figure redrawn so closely from a copyrighted source that it functions as a copy is not merely reproduced once; it is offered to every reader for further adaptation. The test is not whether we redrew it. The test is whether what we produced is our own expression of the underlying idea. Structure, sequence, and concepts are not copyrightable. Particular visual expression is.

**Therefore: describe any framework, cite its clauses, teach its structure, redraw its diagrams in our own visual language. Never lift a diagram, table, or extended passage, and never produce a redrawing that is recognizably the source figure with new colors.**

The safest and best redrawings are the ones that diverge. Where our model differs from the source, the divergence is both editorially valuable and evidence of independent expression. See `FIGURE_SPEC.md` Section 9.

---

## 2. Reuse tiers

### Tier 1: reusable with attribution

- **NIST publications.** US government work, not subject to domestic copyright. AI RMF 1.0, the Generative AI Profile, NCCoE materials, agent standards work.
- **EU legislative text.** EUR-Lex permits reuse with source acknowledgment. The AI Act, GDPR, the Digital Omnibus amending regulation, Official Journal notices.
- **US federal agency guidance.** EEOC, FTC, CFPB, FDA, executive orders, Federal Register notices.
- **OECD materials.** Generally permissive; verify the specific document.
- **State legislative text.** US state statutes.

Even here, prefer paraphrase. Quote only where exact wording is legally operative, such as a statutory definition or a threshold.

### Tier 2: cite and describe, do not reproduce

- **ISO/IEC standards.** All of them. Copyrighted and sold. Cite by number and clause, describe what a clause addresses, never reproduce its text, tables, or figures.
- **CEN-CENELEC standards and drafts,** including prEN 18286. Same treatment.
- **The three lines model.** Owned by the Institute of Internal Auditors. Describe the structure and redraw it in our visual language.
- **IAPP materials,** including the AIGP body of knowledge in the project files. Structural reference for us, not a citable source, and never reproduced.
- **Academic papers and their figures.** Cite normally; redraw anything visual.
- **Model cards, datasheets, and similar published templates.** The concepts are freely teachable. Published examples belong to their authors. Appendix C templates must be written from scratch, since CC BY-NC licenses readers to adapt them.
- **Vendor and consultancy publications.** Not sources of fact in any case. Useful only for locating primary sources.

### Tier 3: verify individually before use

Anything not listed above. National frameworks including Singapore's IMDA materials, standards bodies outside ISO and CEN, and any third-party template. Check terms before reproducing anything, and default to describe-and-redraw if terms are unclear.

---

## 3. The project files are input, not citation

Two files in the project require explicit handling.

`babok_guide_v3_member.pdf` and `pba_companion_full.md` inform the methodological approach and must never appear in the manuscript. Not in citations, not in references, not in an appendix, not in a further-reading note. Their vocabulary is prohibited outright. See the prohibited vocabulary list in BOOK_SPECIFICATION_v2.md Part B, which is not advisory.

`AIGP_Cert_BOK_FINAL_012925.pdf` and the study guides are structural reference for coverage checking. The book is aligned with the body of knowledge but never organized around it, and never cites it as authority.

`ShawnAIBookFull.docx`, `How_to_Govern_AI_v3.md`, and `AIGP_Study_Book_v4_Final.md` are prior drafts by the author. Reuse freely. Everything in them predates the current specification and none of it passes the current rules unchecked.

The Parsons PDFs are prose style models. Read for register, never cited.

---

## 4. Source register

Verify each against the primary source before assertion. Status column records what was confirmed and when.

### Legislation and regulation

| Source | Covers | Status |
|---|---|---|
| Regulation (EU) 2024/1689 (AI Act) | Risk tiers, prohibited practices, high-risk obligations, GPAI, penalties | Cited throughout Ch 2 |
| Regulation (EU) 2026/1744 (Digital Omnibus on AI) | Deferrals, new Art. 5 prohibitions, AI Office powers | OJ 24 Jul 2026, in force 27 Jul 2026. Confirmed Aug 2026 |
| GDPR, esp. Arts. 5, 6, 22, 35 | Lawful bases, minimization, automated decisions, DPIAs | Stable |
| US EO, Dec 2025, national AI policy framework | Preemption direction, litigation task force | Confirmed Aug 2026 |
| California SB 53 (frontier track) | Frontier developer safety-framework disclosure, eff. 1 Jan 2026 | Confirmed 2026-09-12 |
| Texas TRAIGA / HB 149 | Government-use disclosure and prohibitions; explicitly NOT an algorithmic-discrimination duty-of-care statute, no impact assessment, does not reach private employment, AG enforcement only; eff. 1 Jan 2026 | Confirmed 2026-09-12. Do not group with Illinois or Colorado as the same track. |
| Illinois HB 3773 (amends Illinois Human Rights Act) | Algorithmic-discrimination track: AI employment discrimination prohibition, notice to employees/applicants; eff. **1 Jan 2026**, not 2027 | Confirmed 2026-09-12, corrected from prior spec |
| New York RAISE Act (frontier track) | Frontier model transparency, eff. 1 Jan 2027 | Confirmed 2026-09-12 |
| California automated-employment-decision law | **None in force.** SB 7 would have created one; vetoed Oct 2025. Do not describe California as regulating automated employment decisions. | Confirmed 2026-09-12 |
| Colorado AI Act (SB 24-205) | Never became operative; repealed 14 May 2026 by SB 26-189 before its own deferred start date. Replaced by the narrower Automated Decision-Making Technology Act (disclosure/individual rights, not duty of care), eff. 1 Jan 2027. | Confirmed 2026-09-12 |
| NYC Local Law 144; Illinois AI video interview act | Bias audits, notice and consent | Verify current |
| Title VII, ADA, ADEA, ECOA, FCRA, FHA | Discrimination and credit obligations | Stable |

### Standards and frameworks

| Source | Covers | Status |
|---|---|---|
| NIST AI RMF 1.0 | Govern, Map, Measure, Manage | Tier 1, reusable |
| NIST Generative AI Profile (AI 600-1) | Generative risk categories | Verify current version |
| NIST agent standards work | Agent identity, authorization, accountability | **Primary source needed. Ch 12** |
| ISO/IEC 42001:2023 | AI management system, certifiable | Tier 2 |
| ISO/IEC 42005 | AI system impact assessment | **Verify publication. Bears on Ch 14** |
| ISO/IEC 42006:2025 | Requirements for AIMS audit and certification bodies | **Verify. Makes 42001 certification meaningful** |
| ISO/IEC 42007 | Conformity assessment schemes | **Verify** |
| ISO/IEC 12792 | Transparency taxonomy | **Verify** |
| ISO/IEC TS 6254 | Explainability | **Verify. Bears on Ch 6** |
| ISO/IEC 27090 | Cybersecurity guidance for AI | **FDIS registered Mar 2026. Verify publication. Ch 7** |
| ISO/IEC 29119-11 | Testing of AI systems | **Verify status. Ch 7** |
| ISO/IEC 22989; 23894 | Terminology; risk management | Tier 2 |
| CEN-CENELEC JTC 21, prEN 18286 | EU quality management system for AI Act purposes | **Track. Critical to Ch 2 argument** |
| IMDA Model AI Governance Framework for Agentic AI | Four dimensions, agent components, multi-agent patterns | v1.5, 20 May 2026. **Confirm from IMDA directly. Ch 12** |
| OECD AI Principles; classification framework | Values; five-dimension classification | Tier 1 |
| Institute of Internal Auditors three lines model | Ch 13 | Tier 2, redraw |

### Documented cases

Every real case used in a Case in Focus needs a source before it ships. Currently referenced: the Detroit facial recognition wrongful arrest, the healthcare cost-proxy algorithm finding, recidivism prediction disparity findings, the Amazon recruiting tool, and an enforcement action requiring model deletion. **None are sourced in the specification. All require sourcing.**

---

## 5. Citation conventions

Per-chapter references, which version 1.5.2 lacked and should have.

Legislation by instrument number, article, and where relevant the amending instrument. Standards by number, year, and clause. Cases by the source that documented them, not by the news coverage of the source. Web sources with access dates, because this field's primary sources move.

Where a claim rests on a fast-moving source, say so in text rather than only in the note. "As of August 2026" is not hedging in this book; it is accuracy, and it protects readers who find the book two years later.

---

## 6. Currency sweep brief

Run this before drafting. It changes Chapters 2, 6, 7, 11, 12, 14, and 16, and drafting them first means drafting them twice.

Produce one findings document: `CURRENCY_FINDINGS.md`, organized by chapter, each entry stating what is current, what the specification currently says, whether they differ, and what changes. Cite everything with access dates.

**Confirm or correct.** Every unconfirmed item in Section 4, starting with Colorado's effective date and the ISO publication statuses.

**Check for movement since May 2026 on.** Harmonized standards cited in the Official Journal, which would materially change Chapter 2. US preemption litigation and any enacted federal legislation. The Great American AI Act's progress. Additional state laws. EU AI Act implementing acts and guidance. GPAI code of practice status.

**Check for gaps we may not know exist.** Jurisdictions the specification barely covers: Canada, China, India, Brazil, Korea, UK. Sector-specific AI regulation in healthcare, financial services, and employment. Agentic-specific guidance beyond IMDA. AI incident reporting regimes and repositories. Assurance and audit market developments, including whether third-party AI audit has matured into anything citable. Evaluation and benchmarking practice, which moves faster than regulation and where Chapter 7 is most exposed.

**Check the live book.** aigov.ogunseye.com, version 1.5.2, January 2026. Identify what is now stale, what version 2.0 keeps, and what the seven-chapter structure covered that the eighteen-chapter specification may have dropped. Chapter 7 of the live book, on ongoing issues and future directions, has no direct successor and should be checked for orphaned material.

**Do not resolve conflicts silently.** Where a finding contradicts the specification, record both and flag it. Some contradictions are the specification being wrong; some are the finding being from a secondary source that misread a primary one. That call belongs to the author.
