# Faculty Development Repository: AI Workflows & Strategies

[← Back to Resource Library](../RESOURCES.md)

Practical, field-tested workflows that help faculty use AI to work smarter in clinical care, administration, teaching, and scholarship. Each entry follows a consistent format so you can scan quickly, try one this week, and contribute your own.

**The rule that governs everything here:** patient data belongs only in institutionally approved, PHI-secure tools; unpublished scholarly work belongs only in no-retention enterprise tools or local models; and you — not the AI — remain accountable for every output you act on.

---

## How to Use This Repository

- **Scan the workflow index** below and pick one that matches a task you already do.
- **Check the tool requirements first** — every workflow specifies the security tier it needs (EHR-integrated / enterprise no-retention / local model / any).
- **Start with the prompt starter**, then adapt it to your context and specialty.
- **Contribute back**: if you adapt a workflow or invent a better one, [send it in](#contribute-a-workflow).

### Workflow Index

| Workflow | Category | Security Tier Required |
|----------|----------|------------------------|
| [Omission Scanning](#omission-scanning-medication--problem-list-reconciliation) | Clinical | EHR-integrated or enterprise PHI-secure AI |
| [Ready-to-Use Teaching Session: AI in Clinical Care](#ready-to-use-teaching-session-ai-in-clinical-care) | Teaching | None — discussion-based module |
| [Pre-Submission Manuscript Review](#pre-submission-manuscript-review) | Scholarly / Administrative | No-retention enterprise AI or local model |

---

## Clinical Workflows

### Omission Scanning: Medication & Problem List Reconciliation

**Category:** Clinical &nbsp;|&nbsp; **Time investment:** 2–3 minutes per patient &nbsp;|&nbsp; **Tools:** Institutionally approved, PHI-secure AI only (EHR-integrated assistant or enterprise tool covered by a BAA)

**The problem it solves.** Errors of omission are harder to see than errors of commission. Medication lists and problem lists drift out of sync across transitions of care, specialist handoffs, and years of visits — a medication lingers after its indication resolved, or a documented problem never received guideline-supported therapy. Manually cross-checking both lists in both directions is tedious, so it rarely happens systematically.

**What the workflow does.** Uses a PHI-secure AI tool to scan the active medication list against the problem list — in both directions — and flag likely omissions for the clinician to verify:

1. **Medications without a matching indication** on the problem list — may signal an undocumented diagnosis (fix the problem list) or a legacy medication that's a deprescribing candidate (fix the med list)
2. **Problems without expected therapy** — potential care gaps, e.g., heart failure with reduced ejection fraction without guideline-directed medical therapy, atrial fibrillation with an elevated CHA₂DS₂-VASc score without anticoagulation, diabetes with established ASCVD without a statin
3. **Duplicate or overlapping therapies** — therapeutic duplication across prescribers
4. **Stale entries** — resolved or outdated problems cluttering the list and degrading its signal value

**Steps:**

1. **Confirm your tool is approved for PHI.** EHR-integrated assistants or enterprise tools under a BAA only. Never a consumer chatbot — no exceptions.
2. **Assemble the inputs.** Current medication list and problem list (EHR-integrated tools may pull chart context directly).
3. **Run the scan** using the prompt starter below.
4. **Verify every flag against the chart** before acting. The AI cannot see the outside cardiologist's note, the documented intolerance, or the goals-of-care conversation. A flag is a question, not a finding.
5. **Act on confirmed items**: update the problem list, reconcile medications, address true care gaps, deprescribe where appropriate.
6. **Document your reasoning** wherever a change affects care.

**Prompt starter:**

> Compare this active medication list with this problem list. Identify: (1) medications with no matching indication on the problem list; (2) problems that typically warrant medication therapy where none appears on the list; (3) duplicate or therapeutically overlapping medications; (4) problems that appear resolved or outdated. For each flag, briefly state your reasoning and what I should verify in the chart before acting. Flag only — do not make treatment recommendations.

**Guardrails:**

- The output is a *screen*, not a decision. Every flag requires chart verification and clinical judgment.
- Many "omissions" are intentional: patient preference, contraindications, prior adverse reactions, comfort-focused goals of care, or an outside prescriber managing the condition.
- Watch for hallucinated indications or invented "guideline recommendations" — verify anything that drives an ordering decision against a primary source.
- Accountability for the final medication list and problem list rests with the clinician, exactly as it would without the tool.

**Why faculty report it's worth it:** a structured two-to-three-minute scan before a visit or during medication reconciliation catches list drift that ad hoc review misses, improves the problem list as a communication tool for the whole care team, and models rigorous, transparent AI use for trainees in real time.

---

## Teaching Workflows

### Ready-to-Use Teaching Session: AI in Clinical Care

**Category:** Teaching &nbsp;|&nbsp; **Time investment:** one small-group session (no preparation of original materials required) &nbsp;|&nbsp; **Tools:** None — discussion-based module

**The problem it solves.** Faculty asked to teach about AI in clinical care often have to build a session from scratch on a topic they're still learning themselves. A vetted, case-based module with a moderator guide removes that barrier.

**What the workflow is.** A case-based teaching module from the Yale Primary Care Pediatrics Curriculum, designed as a guide for small-group discussion on AI in clinical care and also suitable for self-directed reading. Targeted at all levels of learners and clinicians, it comes in separate **learner** and **moderator** versions, so you can lead the discussion from the moderator guide while distributing the learner version.

The module's five learning objectives: developing vocabulary around clinical AI; evaluating use cases (ambient documentation, clinical decision support, summarization); selecting applications that avoid cognitive offloading; applying safeguards such as verification and privacy review; and discussing climate implications — all while emphasizing preservation of diagnostic reasoning and professional accountability.

**How to use it:**

1. Read the moderator version to prepare; no additional materials are needed.
2. Distribute the learner version before or during a small-group session.
3. Lead the case discussion, drawing on the moderator guide's prompts.
4. Alternatively, assign it as self-directed reading for learners or as a primer for fellow faculty.

- [Sample Chapter](https://medicine.yale.edu/pediatrics/pcpc/about/sample/)

*Source: Yale School of Medicine (contributed by Jaideep S. Talwalkar, MD)*

---

## Scholarly & Administrative Workflows

### Pre-Submission Manuscript Review

**Category:** Scholarly / Administrative &nbsp;|&nbsp; **Time investment:** 20–30 minutes per manuscript &nbsp;|&nbsp; **Tools:** Secure AI with contractual no-data-retention (enterprise tier), or a local model for full confidentiality

**The problem it solves.** Copy-edit-level problems — typos, inconsistent terminology, numbers that don't match between abstract and tables — generate avoidable rounds of editorial revision that add weeks to publication timelines. A systematic AI-assisted final pass catches most of them before submission.

**What the workflow does.** Runs the near-final manuscript through targeted review passes for mechanical and consistency errors, using a tool whose terms guarantee your unpublished work isn't retained or used for training:

- Grammar, spelling, and punctuation
- **Terminology and abbreviation consistency** — every abbreviation defined at first use and used consistently thereafter
- **Numerical consistency** — values in the abstract match the results section, tables, and figures
- Internal cross-references (Table 2 exists and says what the text claims)
- Tense and voice consistency across sections
- Word-count and formatting limits for the target journal
- Presence of applicable reporting-guideline elements (CONSORT, STROBE, PRISMA, SQUIRE)

**Steps:**

1. **Choose an appropriate tool.** Unpublished manuscripts are confidential — yours, your co-authors', and often your funder's. Use an enterprise AI tool with contractual no-training/no-retention terms, or run a local model so nothing leaves your machine.
2. **Run targeted passes, one concern at a time.** "Check numerical consistency between the abstract, results, and tables" outperforms "fix everything." Repeat for abbreviations, cross-references, and grammar.
3. **Review every suggested change yourself.** Accept mechanical fixes; scrutinize anything touching scientific meaning. Preserve your authorial voice.
4. **Verify references survived intact.** AI tools may "helpfully" reformat or — worse — fabricate citations. Confirm every reference against your reference manager.
5. **Disclose the use.** Follow ICMJE guidance and the target journal's AI policy: AI-assisted editing is typically noted in the acknowledgments or methods, AI is never listed as an author, and authors remain fully accountable for all content. Proactive disclosure here is also simply modeling the transparency we ask of our learners.
6. **Keep a use record** — tool, version, date, and how it was used — so your disclosure statement is accurate and effortless to write.

**Prompt starter:**

> Review this manuscript draft for internal consistency only — do not rewrite content or alter scientific meaning. Report: (1) abbreviations not defined at first use, or used inconsistently; (2) numerical values that differ between the abstract, body text, tables, or figure captions; (3) cross-references to tables, figures, or sections that don't match their targets; (4) grammar, spelling, or punctuation errors. Present findings as a list with locations; do not produce a revised draft.

**Guardrails:**

- Never paste unpublished data or manuscripts into consumer tools that retain inputs or train on them.
- Check the target journal's AI policy *before* submission — policies vary and are evolving quickly.
- The tool checks consistency; it cannot check truth. Scientific accuracy remains entirely the authors' responsibility.

**Why faculty report it's worth it:** fewer copy-edit-level revision requests, faster editorial turnaround, and a disclosure practice that keeps you ahead of tightening journal requirements rather than scrambling to comply with them.

---

## Contribute a Workflow

This repository grows through member contributions. If you've developed an AI workflow that saves you time in clinical care, administration, teaching, or scholarship — polished or rough — we want it.

**How to submit:** Open a Pull Request adding your workflow to this file, or open an issue in this repository describing it. Submissions are reviewed and incorporated with attribution to you and your institution (or anonymously, if you prefer).

A complete submission is welcome but not required — a two-sentence description of what you do and which tool you use is enough to start the conversation. If you'd like to make incorporation fast, include:

- **Workflow name** and one-line description
- **Category**: clinical, administrative, teaching, or scholarly
- **Tools used** and their security tier (EHR-integrated / enterprise no-retention / local model / any)
- **Steps** as you actually perform them
- **A prompt** that works for you, if applicable
- **Guardrails** — what could go wrong and how you prevent it
- **Time saved**, even as a rough estimate

---

*Source: AI in Medical Education Consortium — Faculty Development thematic group*
