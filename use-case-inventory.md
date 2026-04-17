# AI Prompt Templates for Internal Auditors: Use Case Inventory

A curated collection of AI prompt templates designed for Internal Audit professionals. Each template is a standalone workflow that works across general-purpose AI tools (ChatGPT, Claude, Microsoft Copilot, and others). No coding experience required.

**Created by:** Harbor View Consulting LLC
**Companion to:** "Practical AI Use Cases for Internal Auditors" (IIA Baltimore Chapter, April 2026)

---

## How to Use This Repo

Each use case below will become its own prompt template file. Templates include the prompt text, instructions for what to provide as input, what to expect as output, and tips for getting better results. Copy and paste them into your preferred AI tool and adapt them to your organization.

---

## Use Cases

### 1. Risk Assessment Deep Research
**Slide Reference:** 10
**Audit Phase:** Risk Assessment & Planning
**Status:** NEEDS DEEP RESEARCH — Requires deeper understanding of how Internal Auditors actually perform risk assessments (frameworks, scoring methodologies, risk universe construction, linkage to audit plan) before this prompt can be written well.

**What it does:** Generates a structured risk research report for a company or business unit by synthesizing publicly available information. The AI reviews financial filings, analyst commentary, regulatory developments, peer benchmarks, and news coverage, then organizes findings into categories (trend analysis, emerging risks, business model changes) with source citations and confidence ratings.

**Inputs:**
- Company name or business unit
- Industry context and any known focus areas
- Optionally: prior audit findings or risk assessment results for comparison

**Outputs:**
- Structured research report organized by risk category
- Source citations for each finding
- Confidence ratings (High / Medium / Low) per item
- Summary of organizational trends, emerging risks, and business model changes

**Example prompt sketch:**
> I'm an internal auditor preparing a risk assessment for [Company Name], a [industry] company. Research the top financial, regulatory, and operational risks facing this company right now. Organize your findings into three sections: (1) Organizational Trends, (2) Emerging Risks, and (3) Business Model Changes. Cite your sources and provide a confidence rating for each finding.

**Applicable tools:** ChatGPT Deep Research, Claude, Microsoft Copilot

---

### 2. Audit Scoping and LOE Estimation
**Slide Reference:** 11
**Audit Phase:** Planning
**Format:** MULTI-AGENT WORKFLOW — Use this as the showcase example of folder structures with agent.md files and sub-agents under an orchestrator. Sub-agents handle research synthesis, standards alignment, and LOE estimation; the orchestrator produces the final scoping package. Developed as a folder structure in the repo alongside the single-file skills.

**What it does:** Takes risk research output and supporting materials (prior audit findings, walkthrough notes, relevant standards) and produces a draft audit scope and level-of-effort estimate. Replaces gut-feel budgeting with structured estimation grounded in complexity, staffing, and timeline analysis.

**Inputs:**
- Risk research output (from Use Case 1 or equivalent)
- Prior audit findings for the entity
- Walkthrough transcripts or notes (if available)
- Relevant IIA or ISACA guidance references

**Outputs:**
- Draft audit scope tailored to identified risks and prior findings
- Level-of-effort estimate with staffing and timeline assumptions
- Rationale connecting scope decisions back to risk factors

**Example prompt sketch:**
> Based on the following risk research [paste output], prior audit findings [paste], and relevant IIA Standards, draft an audit scope for [Entity]. Include: (1) key risk areas to cover, (2) suggested audit objectives for each, (3) a level-of-effort estimate broken down by phase (planning, fieldwork, reporting), and (4) your rationale for what's in scope and what's excluded.

**Applicable tools:** ChatGPT, Claude, Microsoft Copilot

---

### 3. Smart PBC Request Generator
**Slide Reference:** 12
**Audit Phase:** Planning / Fieldwork

**What it does:** Transforms generic PBC (Prepared by Client) requests into hyper-specific, complete requests that minimize back-and-forth with the client. The AI adds precise date ranges, required data fields, file format expectations, and parameter specifications so evidence arrives complete on the first try.

**Inputs:**
- Draft or generic PBC request language
- Audit period dates
- Process area or control being tested
- Optionally: the system the client uses (e.g., SAP, Oracle, NetSuite)

**Outputs:**
- Revised PBC request with specific fields, date ranges, and format requirements
- Suggested follow-up language if the initial request is incomplete

**Example prompt sketch:**
> I'm preparing a PBC request for an accounts payable audit covering Q1 2026. Here is my current draft request: "[paste generic request]." Make this request more specific by adding: exact date ranges, required data fields (vendor name, invoice number, amount, approval date, etc.), expected file format, and any supporting documentation the client should include (e.g., system parameter screenshots, sampling methodology).

**Applicable tools:** ChatGPT, Claude, Microsoft Copilot

---

### 4. Walkthrough Transcript to Workpaper
**Slide Reference:** 13
**Audit Phase:** Fieldwork
**Status:** NEEDS DEEP RESEARCH — Requires understanding of IIA Standards guidance on workpaper documentation requirements (what must be included, sufficient/reliable/relevant criteria, supervisory review expectations) before this prompt can be written well.

**What it does:** Converts a walkthrough recording transcript (from Teams, Zoom, or a voice memo) into a formatted audit workpaper. The AI classifies controls by type (Inquiry, Inspection, Observation, Re-performance), extracts test attributes, and drafts formal test steps with results. The auditor reviews and edits rather than drafting from scratch.

**Inputs:**
- Walkthrough transcript (auto-generated from meeting recording or voice memo)
- Optionally: the control matrix or test plan being addressed

**Outputs:**
- Formatted workpaper with control descriptions, test steps, and attributes
- Control classifications (Inquiry, Inspection, Observation, Re-performance)
- Draft test results based on statements made during the walkthrough
- Flagged items where the transcript was ambiguous or incomplete

**Example prompt sketch:**
> Here is a transcript from an audit walkthrough of the three-way match process in accounts payable: [paste transcript]. Convert this into a formatted audit workpaper. For each control discussed: (1) classify the control type (Inquiry, Inspection, Observation, or Re-performance), (2) write formal test steps, (3) list the attributes tested, and (4) draft the test result based on what was stated. Flag anything that's ambiguous or needs follow-up.

**Applicable tools:** ChatGPT, Claude, Microsoft Copilot

---

### 5. Population Testing and Exception Filtering
**Slide Reference:** 14
**Audit Phase:** Fieldwork / Testing

**What it does:** Helps auditors move from sample-based testing to population-level analysis. The AI writes test scripts (SQL, Python, or Excel formulas) that validate every transaction in a dataset against defined criteria, then filters down to only the exceptions that require human judgment. Instead of sampling 25 items and hoping they represent the population, the auditor reviews 100% of true exceptions.

**Inputs:**
- Transaction data export (CSV, Excel)
- Control criteria or test conditions (e.g., "flag invoices where the approver is also the requestor")
- Optionally: tolerance thresholds or materiality limits

**Outputs:**
- Test script (SQL, Python, or Excel formula) that applies the criteria to the full population
- Exception listing with relevant fields for each flagged item
- Summary statistics (total tested, exceptions found, exception rate)

**Example prompt sketch:**
> I have an export of 10,000 AP transactions with the following columns: [list columns]. I need to test for segregation of duties violations where the person who approved the invoice is the same person who submitted the purchase request. Write a [Python script / SQL query / Excel formula] that flags all exceptions. Include a summary showing total transactions tested, number of exceptions, and exception rate.

**Applicable tools:** ChatGPT, Claude, Microsoft Copilot (for script generation); results executed in Python, SQL client, or Excel

---

### 6. Cross-Audit Pattern Recognition
**Slide Reference:** 15
**Audit Phase:** Reporting / Continuous Improvement

**What it does:** Analyzes findings across multiple audits to surface systemic patterns and root causes that may not be visible when reviewing individual reports. The AI identifies connections between disparate findings (e.g., twelve findings across departments that trace back to a single root cause) and drafts remediation recommendations that address the systemic issue.

**Inputs:**
- Audit findings from multiple engagements (copy/paste or structured listing)
- Optionally: finding categories, risk ratings, and responsible departments

**Outputs:**
- Grouped findings by common root cause or theme
- Narrative explaining the systemic pattern
- Draft remediation recommendations targeting the root cause
- Suggested talking points for management discussion

**Example prompt sketch:**
> Here are 30 audit findings from 8 audits completed this year: [paste findings with departments and categories]. Analyze these findings for systemic patterns. Group related findings by common root cause, explain the pattern you see, and draft remediation recommendations that address the underlying issue rather than individual symptoms. Include talking points I can use when presenting this analysis to senior management.

**Applicable tools:** ChatGPT, Claude, Microsoft Copilot

---

### 7. Report Review: Audit Committee Dry-Run
**Slide Reference:** 16
**Audit Phase:** Reporting
**Note:** The prompt template must include a detailed default persona for a typical Audit Committee Chair (board-level governance experience, fiduciary mindset, focus on risk appetite alignment, regulatory exposure, tone-at-the-top, management remediation follow-through, financial reporting integrity). Users can override with their own committee member profiles, but the default should be substantive enough to produce realistic pushback out of the box.

**What it does:** Simulates how an Audit Committee member would react to your draft report. You provide the report along with background on the committee members, and the AI reviews the report from their perspective, identifying likely questions, areas of pushback, and gaps in the narrative. Helps you anticipate tough questions before the meeting.

**Inputs:**
- Draft audit report
- Audit Committee member profiles or backgrounds (titles, areas of focus, known concerns)
- Optionally: prior committee meeting minutes or feedback

**Outputs:**
- List of likely questions the committee will ask, organized by report section
- Areas where the committee may push back or request more detail
- Suggested responses or additional talking points
- Recommendations for strengthening the report before submission

**Example prompt sketch:**
> Review this audit report as if you are the Audit Committee Chair. The Chair is a former CFO with a focus on financial controls and regulatory compliance. Here is the report: [paste report]. What questions will you ask? Where will you push back? What's missing or unclear? Provide your feedback organized by report section.

**Applicable tools:** ChatGPT, Claude, Microsoft Copilot

---

### 8. Report Review: Clone the Reviewer
**Slide Reference:** 16
**Audit Phase:** Reporting

**What it does:** Learns the review style of a senior leader (Head of IA, Director, Partner) from examples of their past edits and comments, then applies that same standard to a new draft. Catches recurring logic gaps, tone issues, and structural problems before the draft reaches the reviewer, reducing review cycles.

**Inputs:**
- 3-4 past audit reports with tracked changes and comments from the reviewer
- The new draft report to be reviewed

**Outputs:**
- Marked-up review of the new draft applying the learned review standards
- Specific edits and comments matching the reviewer's style and priorities
- Summary of patterns in the reviewer's feedback (common issues they flag)

**Example prompt sketch:**
> I'm going to show you 3 audit reports that were reviewed by our Head of Internal Audit. Each includes tracked changes and comments showing their review standards. Learn their review style, then apply the same standards to a new draft. [Paste Report 1 with edits] [Paste Report 2 with edits] [Paste Report 3 with edits]. Now review this new draft: [paste new report]. Apply the same standards and flag the same types of issues.

**Applicable tools:** ChatGPT, Claude (large context window helpful for multiple reports), Microsoft Copilot

---

### 9. Plain English to SQL/Python Analytics
**Slide Reference:** 17
**Audit Phase:** Continuous Auditing / Monitoring

**What it does:** Translates a plain English description of what you want to monitor into a working SQL query or Python script. Designed for auditors who do not have programming experience but need to build continuous monitoring dashboards. The output can be pasted directly into Power BI, Tableau, or a database query tool.

**Inputs:**
- Plain English description of the monitoring rule or analytic
- Column names and data types from the source data (or a sample of the data)
- Target platform (Power BI, Tableau, Excel, direct SQL)

**Outputs:**
- Working SQL query or Python script implementing the described logic
- Explanation of what each part of the code does
- Instructions for deploying it in the target platform

**Example prompt sketch:**
> I have an AP transactions export with these columns: [list columns and types]. I want to flag any invoices where the person who approved the invoice is also the person who submitted the purchase request. Write a SQL query I can paste into Power BI to create a continuous segregation of duties monitor. Explain what each part of the query does so I can modify it later.

**Applicable tools:** ChatGPT, Claude, Microsoft Copilot

---

### 10. Recruiting Due Diligence
**Slide Reference:** 18
**Audit Phase:** N/A (Team Management)
**Note:** The prompt template must explicitly invoke deep research / web browsing capabilities. The value of this skill depends on the AI actually searching public sources (SEC EDGAR, press releases, LinkedIn, news articles) to validate claims, not just reasoning about plausibility from the resume text alone.

**What it does:** Performs due diligence on a job candidate's resume by cross-referencing stated experience against publicly available information. The AI extracts tenure dates and checks them against verifiable events (SEC filings, IPOs, M&A activity, major organizational changes) during the candidate's stated employment window. Produces confidence scores on resume claims and generates role-specific interview questions.

**Inputs:**
- Candidate resume (text or PDF)
- Job description or role requirements
- Optionally: specific claims to validate

**Outputs:**
- Claim-by-claim validation with confidence ratings (High / Medium / Low)
- Flags for claims that cannot be verified or appear inconsistent
- Custom interview questions targeting areas where verification was inconclusive
- Summary assessment

**Example prompt sketch:**
> Here is a resume for a Senior Internal Auditor candidate: [paste resume]. Cross-reference their stated experience against publicly available information. For each role: (1) verify the company existed during the stated dates, (2) check if major events they reference (IPO readiness, M&A, system implementations) actually occurred during their tenure, and (3) assess whether their stated scope and complexity is plausible. Provide a confidence rating for each claim. Then generate 5 interview questions targeting areas where you couldn't fully verify their claims.

**Applicable tools:** ChatGPT Deep Research, Claude, Microsoft Copilot

---

### 11. Standards and Guidance Flashcard Generator
**Slide Reference:** 19
**Audit Phase:** N/A (Professional Development)
**Note:** The prompt must explicitly constrain the AI to only use content from the provided document. No outside knowledge, no paraphrasing beyond what the source says. Every flashcard must include the page number / section reference from the source document so the user can verify each answer against the original. This is a grounded extraction task, not a creative generation task.

**What it does:** Converts dense guidance documents (new IIA Standards, COSO updates, regulatory changes) into concise flashcards for rapid recall. Each flashcard covers one key change with a practical example showing how it applies to day-to-day audit work. Tailored to the auditor's experience level and industry.

**Inputs:**
- Guidance document or standards update (pasted text or uploaded PDF)
- Auditor's experience level and industry context
- Number of flashcards desired

**Outputs:**
- Set of flashcards, each with a front (question/concept) and back (answer with practical example)
- Organized by topic or section of the source document
- Optionally: formatted for import into a flashcard app (Anki, Quizlet)

**Example prompt sketch:**
> I'm a senior auditor with 5 years of experience in financial services. Here is the latest IIA Standards update: [paste document]. Turn this into 10 flashcards covering the most significant changes. Each flashcard should have a front side with the concept or requirement, and a back side with: (1) a plain-English explanation, (2) a practical example of how this applies to a financial services internal audit team, and (3) what changed from the prior standard.

**Applicable tools:** ChatGPT, Claude, Microsoft Copilot

---

### 12. New Hire Onboarding Q&A
**Slide Reference:** 19
**Audit Phase:** N/A (Team Management / Onboarding)

**What it does:** Creates an interactive Q&A study guide tailored to a new hire's background. The AI generates practice scenarios based on the new auditor's specific industry experience and knowledge gaps, helping them ramp up on the team's methodology, standards, and focus areas faster than traditional onboarding materials alone.

**Inputs:**
- New hire's resume or background summary (experience level, industry, certifications)
- Team methodology documents, audit manual excerpts, or onboarding materials
- Specific areas where the new hire needs to build knowledge

**Outputs:**
- Tailored practice scenarios with questions and model answers
- Knowledge gap analysis based on the new hire's background vs. team requirements
- Suggested reading list or study plan prioritized by relevance
- Progressive difficulty: foundational concepts first, then team-specific applications

**Example prompt sketch:**
> I'm onboarding a new staff auditor who has 2 years of experience in healthcare but is new to financial services. Here are excerpts from our audit methodology: [paste]. Generate 10 practice scenarios that help them build knowledge in financial services audit, starting with foundational concepts and progressing to our team's specific methodologies. For each scenario, include a question, a model answer, and a reference to the relevant section of our methodology.

**Applicable tools:** ChatGPT, Claude, Microsoft Copilot

---

## Prioritization

**Start here (highest standalone value, easiest to demonstrate):**
1. Risk Assessment Deep Research (#1)
2. Smart PBC Request Generator (#3)
3. Standards and Guidance Flashcard Generator (#11)

These three are referenced on Slide 21 ("Tools & Takeaways") as prompts attendees can try immediately. They require minimal setup, no data uploads, and produce useful output on the first try.

**Build next (high value, requires some preparation):**
4. Plain English to SQL/Python Analytics (#9)
5. Cross-Audit Pattern Recognition (#6)
6. Report Review: Audit Committee Dry-Run (#7)

**Build last (most powerful but require real data or multi-step workflows):**
7. Walkthrough Transcript to Workpaper (#4)
8. Population Testing and Exception Filtering (#5)
9. Report Review: Clone the Reviewer (#8)
10. Audit Scoping and LOE Estimation (#2)
11. Recruiting Due Diligence (#10)
12. New Hire Onboarding Q&A (#12)
