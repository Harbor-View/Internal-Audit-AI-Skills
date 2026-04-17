# Walkthrough Transcript to Workpaper

Convert a walkthrough recording transcript into a formatted audit workpaper that meets IIA documentation standards. The AI extracts controls, classifies evidence techniques, drafts a process narrative, and builds a controls summary table, while clearly flagging all professional judgments for auditor review.

## When to Use

- After completing a walkthrough (in-person, Teams, Zoom, or voice memo) where a transcript is available
- When converting informal notes into formal workpaper documentation
- When training new auditors on what a properly documented walkthrough looks like

## What You Will Need

- A walkthrough transcript (auto-generated from a meeting recording or voice memo)
- Optionally: the control matrix, test plan, or audit program step being addressed

## The Prompt

```
You are an experienced internal auditor preparing engagement documentation that must comply with the IIA's 2024 Global Internal Audit Standards (effective January 2025).

DOCUMENTATION STANDARDS TO FOLLOW:
Per Standard 14.1, evidence must be sufficient, reliable, and relevant. Per Standard 14.6, workpapers must support conclusions, enable reperformance by a competent professional, and facilitate supervisory review. Per Standard 13.5, workpapers must include evidence of supervisory review.

The "stand-alone test": A competent auditor who was not present at this walkthrough must be able to read this workpaper and fully understand the process, controls, evidence, and conclusion without asking additional questions.

TRANSCRIPT:
[Paste the walkthrough transcript here]

ADDITIONAL CONTEXT (if available):
- Engagement name: [NAME]
- Entity / business unit: [NAME]
- Audit period: [DATES]
- Audit program step this walkthrough addresses: [REFERENCE, if available]
- Control matrix or test plan: [Paste or describe, if available]

Convert this transcript into a formatted audit workpaper with the following sections:

1. WORKPAPER HEADER
- Workpaper reference: [PLACEHOLDER -- to be assigned per firm indexing]
- Engagement name and entity
- Date of walkthrough (extract from transcript)
- Audit period
- Prepared by: [PLACEHOLDER -- auditor to complete]
- Reviewed by: [PLACEHOLDER -- supervisor to complete]
- Audit program step reference: [PLACEHOLDER -- auditor to link]

2. OBJECTIVE
Draft the audit objective for this walkthrough. State what the procedure is designed to evaluate (design and implementation of controls over [process]). Mark as: [DRAFT -- AUDITOR REVIEW REQUIRED]

3. SCOPE
- Process / cycle covered
- Transaction or item traced (describe the specific transaction walked through)
- Period covered
- Interviewee(s): name, title, role, department (extract from transcript)

4. PROCESS NARRATIVE
Convert the transcript into a numbered, step-by-step process flow from initiation to completion. This is not a transcript summary. Structure it as:
- Step 1: [Actor] [action] [system/document] [key details]
- Step 2: ...
For each step, annotate where a control exists with a reference tag (e.g., [Control A], [Control B]).

5. CONTROLS SUMMARY TABLE
For each control identified, create a row in this table:

| Ref | Control Description | Control Owner | Type (P/D) | Automation (Manual / IT-Dependent / Automated) | Frequency | Assertion(s) | Key/Non-Key | Evidence Technique |
|-----|-------------------|---------------|------------|-----------------------------------------------|-----------|-------------|-------------|-------------------|

Where:
- Type: Preventive (P) or Detective (D)
- Assertion(s): Existence/Occurrence, Completeness, Valuation/Allocation, Rights/Obligations, Presentation/Disclosure (map each control to applicable assertions)
- Key/Non-Key: Mark as [AUDITOR TO CONFIRM -- requires engagement risk assessment context]
- Evidence Technique: Inquiry (default for walkthroughs), Inspection, Observation, or Re-performance

For inquiry evidence: attribute each statement to a named individual with their role (e.g., "Per [Name], [Title], the three-way match is performed by..."). Inquiry alone is not sufficient evidence and must be corroborated.

6. GAPS AND EXCEPTIONS
Flag any process gaps, missing controls, segregation of duties concerns, or inconsistencies identified in the transcript. For each:
- Describe the gap
- Explain why it matters (which assertion or risk is affected)
- Suggest follow-up action

7. OPEN ITEMS / FOLLOW-UP NEEDED
List any items that require additional work:
- Documents promised but not yet received
- Areas needing further testing
- Ambiguous statements that need clarification
- Items the AI could not determine from the transcript

8. CONCLUSION
[DRAFT -- AUDITOR REVIEW REQUIRED]
Draft a conclusion stating whether, based on this walkthrough, the controls over [process] appear to be designed effectively and placed in operation.

IMPORTANT: Clearly state that this walkthrough establishes design and implementation (D&I) only. It does NOT establish operating effectiveness. Operating effectiveness requires separate testing over a sample of transactions across the audit period.

9. LIMITATIONS
State that this workpaper is based on:
- Inquiry with [name(s)] and inspection of a single transaction
- A single point in time, not a period of operation
- Inquiry-based evidence requires corroboration through additional procedures

10. INFORMATION SOURCES
List all individuals interviewed and documents referenced during the walkthrough.

FORMATTING RULES:
- Separate factual observations ("the process owner stated that...") from professional conclusions ("based on this walkthrough, the control appears to be...")
- Mark ALL draft conclusions and AI-generated judgments with [DRAFT -- AUDITOR REVIEW REQUIRED]
- Mark all Key/Non-Key designations with [AUDITOR TO CONFIRM]
- Every control must have an owner, type, and frequency documented
- Every conclusion must reference specific evidence
```

## What to Expect

- A complete workpaper with all 10 sections populated from the transcript
- A controls summary table with classifications and evidence techniques
- Clear separation of facts vs. professional judgments
- All conclusions and key control designations flagged for auditor review
- Gap identification with suggested follow-up actions
- A limitations section clarifying what the walkthrough does and does not prove

## Tips for Better Results

- **Use a high-quality transcript.** AI meeting transcription tools (Teams, Zoom, Otter.ai) work well. If the transcript has many errors, clean up key names and technical terms before pasting.
- **Narrate intentionally during the walkthrough.** Before using this tool, coach your team to narrate their walkthroughs clearly: "I'm now looking at Invoice 4521. The amount is $12,400, which matches the PO. The receiving report confirms delivery on March 3." Structured narration produces dramatically better workpapers.
- **Paste your control matrix alongside the transcript.** If the AI knows which controls it should be looking for, it can map the narrative to your existing control framework rather than identifying controls from scratch.
- **Review every [DRAFT] and [AUDITOR TO CONFIRM] tag.** These are the items where your professional judgment is required. The AI handles the documentation labor; you provide the audit judgment.
- **Use this as a training tool.** Have new auditors compare the AI-generated workpaper to one they drafted manually. The comparison teaches documentation standards more effectively than reading about them.

## IIA Standards Alignment

This skill supports compliance with:
- **Standard 13.5** -- Engagement supervision (workpapers must facilitate supervisory review)
- **Standard 14.1** -- Gathering information that is sufficient, reliable, and relevant
- **Standard 14.6** -- Engagement documentation that supports conclusions and enables reperformance

## Applicable Tools

ChatGPT, Claude (large context window helpful for long transcripts), Microsoft Copilot

---

*Part of the [AI Prompt Templates for Internal Auditors](https://github.com/HarborViewConsulting/Internal-Audit-AI-Skills) collection by [Harbor View Consulting LLC](https://www.harborview-consulting.com). Harbor View is a Baltimore-based advisory firm helping audit, risk, and finance teams modernize through technology and AI-enabled solutions. Questions? Contact Mike Molloy, CISA at mmolloy@harborview-consulting.com.*
