# Research: IIA Standards on Audit Workpaper Documentation

**Purpose:** Inform the design of an AI prompt template that converts walkthrough transcripts into properly formatted audit workpapers.

**Date:** April 17, 2026

---

## 1. IIA Standards on Documentation/Workpapers

The 2024 Global Internal Audit Standards (GIAS), effective January 9, 2025, reorganize the former IPPF into a principles-based framework. Domain V ("Performing Internal Audit Services") contains the primary documentation requirements across three principles:

- **Principle 13: Plan Engagements Effectively** (Standards 13.1 through 13.6)
- **Principle 14: Conduct Engagement Work** (Standards 14.1 through 14.6)
- **Principle 15: Communicate Engagement Results and Monitor Action Plans** (Standards 15.1, 15.2)

### Key Standards

**Standard 14.1 -- Gathering Information for Analyses and Evaluation.** Internal auditors must gather information that is **relevant, reliable, and sufficient** to support engagement findings and conclusions. "Sufficient" means the information allows a prudent, informed, and competent person to repeat the auditor's steps and reach the same conclusion. "Reliable" means factual and current. "Relevant" means consistent with engagement objectives and within scope.

**Standard 14.6 -- Engagement Documentation.** This standard requires internal auditors to document information and evidence in a manner that: (a) supports engagement results and conclusions, (b) enables reperformance of work by a competent professional, (c) facilitates supervisory review, and (d) satisfies retention requirements established by the CAE consistent with organizational guidelines and regulatory requirements.

**Former Standard 2330 (now subsumed by 14.6)** used four quality attributes: documentation must be **sufficient, reliable, relevant, and useful**. The 2024 standards consolidate this into the three-attribute model (sufficient, reliable, relevant) but "useful" remains an implicit expectation: workpapers that cannot be understood by a reviewer are not fit for purpose.

### What "Sufficient, Reliable, Relevant" Means in Practice

| Attribute | Practical Test |
|-----------|---------------|
| **Sufficient** | Could a competent auditor who was not involved in the engagement reperform the work and reach the same conclusion? Is there enough detail on scope, population, sample, procedures, and results? |
| **Reliable** | Is the evidence factual, current, and sourced from credible origins? Are documents authenticated (not just described from memory)? |
| **Relevant** | Does each piece of evidence tie directly to an engagement objective or audit program step? Is extraneous material excluded? |

Sources: [IIA Global Internal Audit Standards (2024)](https://www.theiia.org/globalassets/site/standards/globalinternalauditstandards_2024january9.pdf); [Baker Tilly -- Domain V: Performing Internal Audit Services](https://www.bakertilly.com/insights/domain-v-performing-internal-audit-services); [Wolters Kluwer -- IIA Global Standards Domain II and Domain V](https://www.wolterskluwer.com/en/expert-insights/domains-ii-v-ethics-professionalism-performing-internal-audit-services)

---

## 2. Workpaper Components

### Required and Recommended Components

A properly constructed audit workpaper should contain the following elements:

| Component | Required? | Description |
|-----------|-----------|-------------|
| **Header / Reference Number** | Required | Unique workpaper ID for cross-referencing; engagement name, entity, period |
| **Objective** | Required | Clear statement of what the procedure is designed to test or accomplish; linkage to audit program step |
| **Scope** | Required | Population description, sample size/selection method, period covered |
| **Procedures Performed** | Required | Step-by-step description of what the auditor actually did (not just planned to do) |
| **Evidence Obtained** | Required | Source documents reviewed, screenshots, data extracts, interview notes; must be identified by source |
| **Results / Exceptions** | Required | Factual findings, deviations, errors identified; quantified where possible |
| **Conclusion** | Required | Auditor's professional judgment on whether the objective was met; linkage to control effectiveness |
| **Preparer and Date** | Required | Who performed the work and when |
| **Reviewer and Date** | Required | Who reviewed the workpaper and when; evidence of supervisory sign-off |
| **Cross-references** | Recommended | Links to related workpapers, findings, risk assessments, or the engagement work program |
| **Follow-up Items** | Recommended | Open questions, items for further testing, management action items |

### Walkthrough vs. Test of Controls vs. Substantive Test Workpapers

**Walkthrough Workpaper:**
- Purpose: Understand process design and confirm that a control has been *implemented* (design and implementation, or "D&I")
- Sample: Typically one transaction traced end-to-end ("cradle to grave")
- Documentation method: Narrative description of the process flow, annotated with control points; may include flowcharts, screenshots, and references to policy documents
- Conclusion: Whether the control is designed effectively and has been placed in operation
- Does NOT prove operating effectiveness

**Test of Controls Workpaper:**
- Purpose: Determine whether a control is *operating effectively* over a period
- Sample: Statistically or judgmentally selected sample (commonly 25-40 items for controls operating throughout the period)
- Documentation method: Structured testing matrix with attributes, expected results, actual results, and exception tracking
- Conclusion: Whether the control operated effectively during the test period; deviation rate

**Substantive Test Workpaper:**
- Purpose: Detect material misstatements in account balances or transaction classes
- Sample: Risk-based, often larger samples or full-population analytics
- Documentation method: Quantitative analysis, reconciliations, confirmations, analytical procedures
- Conclusion: Whether balances are materially correct; quantification of errors found

Sources: [IIA Global Knowledge Brief -- Effective Workpapers](https://www.theiia.org/globalassets/site/content/articles/global-knowledge-brief/2018/may/effective-work-papers_update.pdf); [CPA Hall Talk -- How to Use Audit Walkthroughs](https://cpahalltalk.com/audit-walkthroughs/); [My Audit Spot -- Internal Audit Walkthroughs](https://www.myauditspot.com/tools-and-templates/internal-audit-walkthroughs/)

---

## 3. Control Documentation Standards

### The Five Assertion Categories

When documenting controls, auditors must link each control to the management assertion(s) it addresses:

1. **Existence / Occurrence** -- Assets and liabilities exist; recorded transactions actually occurred
2. **Completeness** -- All transactions and accounts that should be recorded have been recorded
3. **Valuation / Allocation** -- Amounts are recorded at appropriate values
4. **Rights and Obligations** -- The entity holds rights to assets and has obligations for liabilities
5. **Presentation and Disclosure** -- Items are properly classified, described, and disclosed

For internal audit walkthroughs, the relevant assertions may also include operational assertions (e.g., process efficiency, compliance with policy, safeguarding of assets) beyond the financial statement focus.

### Control Classification Documentation

During walkthroughs, auditors should document the following control attributes:

| Attribute | Categories | Why It Matters |
|-----------|-----------|----------------|
| **Control type** | Preventive (stops errors before they occur) vs. Detective (identifies errors after the fact) | Determines reliance strategy and residual risk |
| **Automation level** | Manual, IT-dependent (human using system), Fully automated | Affects testing approach; automated controls may need testing only once if GITCs are effective |
| **Frequency** | Per-transaction, daily, weekly, monthly, quarterly, annually | Determines sample size for TOC; informs timing of audit procedures |
| **Key vs. Non-key** | Key control (directly mitigates a significant risk) vs. Non-key (supporting or redundant) | Key controls require testing; non-key controls may be noted but not tested |
| **Control owner** | Name, title, department | Required for accountability and follow-up |
| **Assertion(s) addressed** | Which of the five assertions the control supports | Links control to risk and objective |

### Documenting the Four Evidence-Gathering Techniques

| Technique | How to Document |
|-----------|----------------|
| **Inquiry** | Record who was interviewed, their role, date, and a summary of responses. Note: inquiry alone is not sufficient evidence; must be corroborated |
| **Inspection** | Identify the specific document inspected (name, date, reference number), what was examined, and what it demonstrated |
| **Observation** | Describe what was observed, when, where, and by whom; note that observation provides evidence only for the point in time observed |
| **Re-performance** | Document the control step re-performed, the inputs used, the expected outcome, the actual outcome, and whether results matched |

Sources: [PCAOB AS 1105 -- Audit Evidence](https://pcaobus.org/oversight/standards/auditing-standards/details/AS1105); [Baker Tilly -- Navigating the Basics of Internal Controls](https://www.bakertilly.com/insights/navigating-the-basics-of-internal-controls); [CPA Journal -- The Five Assertions](https://www.cpajournal.com/2017/11/03/five-assertions-categories-assertions-auditors-must-collect-adequate-evidence-support-financial-statement-items/)

---

## 4. Supervisory Review Requirements

### IIA Standards on Review

**Standard 13.5 (Engagement Supervision)** requires that engagements be properly supervised. The engagement supervisor is responsible for reviewing and approving the engagement work program, workpapers, final communication, and performance assessments. Supervision should occur during planning, fieldwork, and reporting.

Evidence of supervisory review includes:
- Workpapers and engagement communications **reviewed and signed or initialled** by the engagement supervisor
- Documented review notes showing questions raised and resolved
- Confirmation that findings and conclusions are **adequately supported** by the evidence in workpapers

### Implications for Workpaper Design

Because workpapers must facilitate supervisory review, they must:
- **Stand alone**: A reviewer should not need to ask the preparer questions to understand the work performed, the evidence obtained, or the conclusion reached
- **Be logically organized**: Follow the engagement work program sequence or a standard template
- **Clearly distinguish fact from judgment**: Observations and evidence should be separated from the auditor's interpretation and conclusion
- **Flag open items**: Unresolved questions or incomplete procedures should be visibly marked for reviewer attention
- **Include a reviewer sign-off field**: Date and initials/signature block

Sources: [IIA Global Internal Audit Standards (2024)](https://www.theiia.org/globalassets/site/standards/globalinternalauditstandards_2024january9.pdf); [IIA Quality Services FAQ](https://www.theiia.org/en/group-services/quality-assurance/quality-services/faq/)

---

## 5. Common Workpaper Failures

Quality assurance reviews (both internal assessments and external quality assessments) consistently flag the following documentation deficiencies:

### Most Frequent Deficiencies

1. **Sign-off without supporting documentation.** Auditors initial an audit program step as complete but include no workpaper showing the evidence obtained or procedures actually performed. A sign-off alone is never sufficient.

2. **Missing or vague conclusions.** Workpapers present evidence but fail to state whether the audit objective was met. The reviewer cannot determine the auditor's professional judgment from the documentation.

3. **Insufficient linkage between risk, procedure, and evidence.** The workpaper does not clearly connect the assessed risk to the specific procedure performed, or the evidence obtained to the conclusion reached. The "so what?" is missing.

4. **Documents filed without context.** A source document is placed in the workpaper file with no annotation explaining why it was obtained, what it demonstrates, or how it relates to the audit objective.

5. **Lack of population and sample documentation.** The workpaper describes testing but does not define the population, the sampling method, or the basis for the sample size. Reperformance is impossible.

6. **No evidence of supervisory review.** Workpapers lack reviewer sign-off, review notes, or any indication that a second person evaluated the work.

7. **Inadequate documentation of inquiry.** Interview responses are summarized too briefly, without identifying who was interviewed, when, or how the response was corroborated with other evidence.

8. **Missing risk assessment linkage.** Procedures are not traceable to the engagement risk assessment or the approved work program. The auditor cannot demonstrate why specific tests were performed.

9. **Inconsistent or outdated templates.** Workpapers use varying formats across engagements, making quality review difficult and increasing the risk of omitted components.

10. **Failure to document scope limitations or deviations.** When planned procedures could not be performed or were modified, the reasons and impact are not recorded.

Sources: [JGA CPA -- Back to Basics: Audit Documentation Failures](https://www.jgacpa.com/back-to-basics-audit-documentation-failures-have-become-dangerous-low-hanging-fruit); [Journal of Accountancy -- Peer Review Findings in Audits](https://www.journalofaccountancy.com/issues/2023/aug/peer-review-findings-in-audits-of-not-for-profits-what-auditors-need-to-know/); [CPA Hall Talk -- A Lack of Audit Documentation is a Big Danger](https://cpahalltalk.com/audit-documentation/); [Wolters Kluwer -- Maximizing IA Effectiveness Through EQAs](https://www.wolterskluwer.com/en/expert-insights/maximizing-internal-audit-effectiveness-through-external-quality-assessments-eqa)

---

## 6. Implications for the AI Prompt

Given the standards and common failures above, the prompt that converts walkthrough transcripts into audit workpapers must instruct the AI to produce the following. Items are categorized as AI-generated (the AI should populate from the transcript) or human-completion (the AI should create the field but flag it for the auditor to fill in or verify).

### Non-Negotiable Fields (Must Appear in Every Workpaper)

| Field | AI-Generated or Human-Completion | Notes |
|-------|----------------------------------|-------|
| **Workpaper reference number** | Human-completion | AI should create a placeholder; numbering depends on the firm's indexing scheme |
| **Engagement name and entity** | AI-generated | Extract from transcript context |
| **Period/date of walkthrough** | AI-generated | Extract from transcript |
| **Audit objective** | AI-generated (draft) | Derive from the discussion; flag for auditor confirmation that it aligns with the work program |
| **Process/cycle name** | AI-generated | Identify from transcript content |
| **Process narrative** | AI-generated | Core value of the tool: convert transcript into structured, step-by-step narrative |
| **Control points identified** | AI-generated | Extract each control mentioned; document control owner, type (preventive/detective), automation level, frequency, and assertion(s) addressed |
| **Evidence technique used** | AI-generated | Tag each control point with the evidence method: inquiry (default for walkthroughs), inspection, observation, or re-performance |
| **Key vs. non-key control designation** | Human-completion | AI can suggest based on context but auditor must confirm |
| **Risks/assertions addressed** | AI-generated (draft) | Map controls to assertions where possible; flag for auditor review |
| **Interviewee(s) / Process owner(s)** | AI-generated | Extract names, titles, roles from transcript |
| **Conclusion** | Human-completion | AI should draft a conclusion but clearly mark it as "DRAFT -- Auditor review required." The auditor's professional judgment cannot be delegated to AI |
| **Exceptions or gaps noted** | AI-generated | Flag any process gaps, missing controls, segregation-of-duties issues, or inconsistencies identified in the transcript |
| **Open items / follow-up needed** | AI-generated | Items mentioned as unresolved, promised documents not yet received, areas needing further testing |
| **Preparer and date** | Human-completion | AI should insert the preparer field; auditor fills in |
| **Reviewer and date** | Human-completion | Must be blank for supervisor to complete |
| **Cross-references** | Human-completion | AI should create placeholder fields for links to work program steps, related workpapers, and findings |

### What the AI Should Flag for Human Completion (Not Generate)

- **Professional conclusions and opinions** -- The AI can draft a conclusion, but must clearly label it as requiring auditor review and sign-off. Per IIA standards, professional judgment is the auditor's responsibility.
- **Key control designations** -- Whether a control is "key" depends on the engagement risk assessment, which the AI does not have full visibility into.
- **Sample size and testing decisions** -- For any follow-up testing recommended, the auditor must determine appropriate sample sizes.
- **Linkage to the approved work program** -- The AI does not have the work program; it should create cross-reference placeholders.
- **Scope limitations** -- If the transcript suggests incomplete information, the AI should note it but the auditor must assess the impact.
- **Risk ratings** -- Residual risk assessments require professional judgment.

### Structural Requirements for the Prompt

The prompt should instruct the AI to:

1. **Use a consistent template structure** matching the firm's methodology (header, objective, scope, narrative, controls table, conclusion, sign-off block)
2. **Separate inquiry evidence from conclusions** -- Clearly distinguish "the process owner stated that..." from "based on this walkthrough, the control appears to be..."
3. **Create a controls summary table** with columns for: control description, control owner, type (P/D), automation (M/IT/A), frequency, assertion(s), key/non-key designation
4. **Document the process as a numbered flow** -- not just a transcript summary, but a logical sequence of steps from initiation to completion
5. **Identify gaps automatically** -- Where the transcript describes a process without a control at a critical point (e.g., no authorization step, no reconciliation, no segregation of duties), the AI should flag it
6. **Include an "Information Sources" section** listing who was interviewed and what documents were referenced
7. **Add a "Limitations" section** noting that the walkthrough is based on inquiry and a single transaction (if applicable), which establishes design and implementation but not operating effectiveness
8. **Mark all draft conclusions and AI-generated judgments** with a visible tag (e.g., "[DRAFT -- AUDITOR REVIEW REQUIRED]") so the reviewer knows what needs human validation

### Quality Checks the Prompt Should Enforce

- Every control identified must have an owner, type, and frequency documented
- Every conclusion must reference specific evidence
- The narrative must be detailed enough that a reviewer who was not present at the walkthrough can understand the process
- Inquiry-based evidence must be attributed to a named individual with their role
- The workpaper must explicitly state what the walkthrough does and does not prove (design and implementation only, not operating effectiveness)

---

## Summary

The IIA's 2024 Global Internal Audit Standards (particularly Standards 13.5, 14.1, and 14.6) set a clear bar: workpapers must contain sufficient, reliable, and relevant information to support conclusions and enable reperformance. The most common QA failures involve missing conclusions, unsupported sign-offs, and evidence filed without context. An AI prompt that converts transcripts to workpapers must produce structured, attributed, and clearly annotated documentation while flagging professional judgments for human completion. The resulting workpaper should pass the "stand-alone test": a competent auditor who was not present at the walkthrough should be able to read the workpaper and understand the process, the controls, the evidence, and the conclusion without asking any additional questions.
