# Recruiting Due Diligence

Perform deep research on a job candidate's resume by cross-referencing stated experience against publicly available information. The AI searches SEC filings, press releases, news articles, and public records to validate claims, then produces confidence scores and generates role-specific interview questions targeting areas that could not be fully verified.

## When to Use

- Before extending an offer to a senior hire (Manager, Director, CAE)
- When a candidate claims involvement in high-profile events (IPO readiness, M&A integration, major system implementations, regulatory remediation)
- When you want to prepare targeted interview questions based on verifiable facts rather than resume bullet points

## What You Will Need

- The candidate's resume (text or PDF)
- The job description or role requirements
- Optionally: specific claims you want validated

## The Prompt

```
You are conducting deep research due diligence on a job candidate for an internal audit leadership role. Your task is to cross-reference the candidate's resume claims against publicly available information. You must actively search the web for evidence. Do not rely solely on your training data.

CANDIDATE RESUME:
[Paste the full resume text or upload the PDF]

ROLE THEY ARE APPLYING FOR:
[Paste the job description or summarize: e.g., "Senior Internal Audit Manager, financial services, managing a team of 6, reporting to the CAE"]

RESEARCH INSTRUCTIONS:

For each position listed on the resume, conduct the following research:

1. COMPANY VERIFICATION
- Confirm the company existed during the stated employment dates
- Search for the company on SEC EDGAR, LinkedIn, Crunchbase, and news archives
- Note any name changes, mergers, acquisitions, or bankruptcies during the candidate's stated tenure

2. CLAIM VALIDATION
For each significant claim the candidate makes (led an IPO readiness audit, managed SOX compliance for 50 entities, implemented a new ERP system, built an audit function from scratch), search for:
- SEC filings (10-K, proxy statements, 8-K) that confirm the event occurred during the candidate's stated tenure
- Press releases or news articles referencing the event
- LinkedIn profiles of other employees at the company during that period who reference the same projects
- Glassdoor or public information about the company's scale (employee count, revenue) to validate scope claims

3. TIMELINE CROSS-REFERENCE
- Check whether major events the candidate references (IPOs, M&A transactions, regulatory actions, system go-lives) actually occurred during their specific employment window
- Flag any timeline inconsistencies

4. SCALE AND COMPLEXITY ASSESSMENT
- Assess whether the candidate's stated scope (team size, number of entities, revenue under audit) is plausible given the company's publicly known size and complexity
- Flag claims that appear inflated relative to what public information suggests

DELIVERABLES:

A. CLAIM-BY-CLAIM ASSESSMENT
For each role and each significant claim, provide:
- The claim (quoted from resume)
- What you found (with source citations and URLs)
- Confidence rating: HIGH (corroborated by multiple public sources), MEDIUM (partially supported by one source), LOW (unable to verify), or FLAG (contradictory evidence found)

B. RED FLAGS
List any items that warrant further inquiry: timeline gaps, claims that contradict public records, scope descriptions that seem inconsistent with company size, or companies with no verifiable public presence.

C. INTERVIEW QUESTIONS
Generate 7-10 custom interview questions based on your research:
- 3-4 questions targeting areas where you could not fully verify claims (probe for specifics without revealing what you found)
- 3-4 questions that test depth of knowledge in areas they claim expertise (e.g., if they claim SOX experience, ask about specific PCAOB standards or common control deficiencies)
- 2-3 behavioral questions tied to the specific challenges of the role they are applying for

D. SUMMARY ASSESSMENT
Provide an overall assessment: what percentage of major claims could you corroborate? Where should the hiring manager focus the interview?
```

## What to Expect

- A claim-by-claim validation table with confidence ratings and source links
- Red flags and timeline inconsistencies
- 7-10 custom interview questions targeting verification gaps
- An overall summary assessment

## Tips for Better Results

- **This prompt requires deep research / web browsing.** Use ChatGPT Deep Research, Claude with web search, or a tool that actively searches the internet. Without live web access, the AI can only reason about plausibility from the resume text itself.
- **Focus on senior hires.** This level of diligence is most valuable for Director-level and above, where resume inflation carries the highest organizational risk.
- **Do not use this as the sole basis for a hiring decision.** This is a research aid, not a background check. Always follow your organization's formal background check and reference verification processes.
- **Remove the candidate's name before sharing outputs.** Treat AI-generated assessments as confidential working documents subject to your organization's data privacy and employment law requirements.
- **Pair with a reference check.** Use the interview questions generated here during reference calls as well, not just candidate interviews.

## Applicable Tools

ChatGPT Deep Research (strongest for this use case), Claude (with web search), Microsoft Copilot

---

*Part of the [AI Prompt Templates for Internal Auditors](https://github.com/HarborViewConsulting/Internal-Audit-AI-Skills) collection by [Harbor View Consulting LLC](https://www.harborview-consulting.com). Harbor View is a Baltimore-based advisory firm helping audit, risk, and finance teams modernize through technology and AI-enabled solutions. Questions? Contact Mike Molloy, CISA at mmolloy@harborview-consulting.com.*
