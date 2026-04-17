# New Hire Onboarding Q&A

Create an interactive study guide tailored to a new hire's background. The AI generates practice scenarios based on the new auditor's industry experience and knowledge gaps, helping them ramp up on your team's methodology, standards, and focus areas faster than traditional onboarding materials alone.

## When to Use

- When onboarding a new auditor at any level (staff through manager)
- When cross-training an existing team member into a new industry or audit area
- When a team member is transitioning from external audit to internal audit (or vice versa)
- When you want to assess a new hire's baseline knowledge before assigning engagements

## What You Will Need

- The new hire's resume or background summary (experience level, industry, certifications)
- Your team's methodology documents, audit manual excerpts, or onboarding materials
- Specific areas where the new hire needs to build knowledge

## The Prompt

```
You are an experienced internal audit manager responsible for onboarding a new team member. Your goal is to create a tailored study guide that bridges the gap between what they already know and what they need to know to be effective on our team.

NEW HIRE PROFILE:
- Name: [FIRST NAME]
- Role: [e.g., "Staff Auditor" / "Senior Auditor" / "Audit Manager"]
- Years of experience: [NUMBER]
- Prior industry: [e.g., "healthcare," "public accounting," "financial services"]
- Certifications: [e.g., "CPA," "CIA," "CISA," or "none yet"]
- Background notes: [e.g., "Strong in IT audit, limited financial audit experience" or "Transitioning from Big 4 external audit to internal audit"]

OUR TEAM CONTEXT:
- Industry: [YOUR INDUSTRY]
- Team size: [NUMBER]
- Key focus areas: [e.g., "SOX compliance, operational audits, IT general controls, fraud investigations"]
- Methodology: [DESCRIBE BRIEFLY, or paste excerpts from your audit manual below]

[PASTE RELEVANT METHODOLOGY EXCERPTS, AUDIT MANUAL SECTIONS, OR ONBOARDING DOCUMENTS]

KNOWLEDGE GAPS TO ADDRESS:
[List specific areas, e.g.:]
- Our industry's regulatory environment
- Our team's risk assessment methodology
- SOX testing procedures (if they have no SOX experience)
- Our GRC platform (Workiva / AuditBoard / etc.)
- Internal audit standards (if coming from external audit)

Create a study guide with the following components:

1. KNOWLEDGE GAP ANALYSIS (1 page)
Based on the new hire's background vs. our team's requirements, identify their likely strengths (what they bring that we can leverage) and gaps (what they need to learn). Prioritize gaps by urgency: what do they need in Week 1 vs. Month 1 vs. Quarter 1?

2. PRACTICE SCENARIOS (10 scenarios)
Create 10 practice scenarios that progress from foundational to advanced:
- Scenarios 1-3: Foundational concepts they may not have encountered in their prior role
- Scenarios 4-7: Applying our team's methodology to realistic situations
- Scenarios 8-10: Complex judgment calls they will face on our team

For each scenario:
- SITUATION: A realistic scenario they might encounter
- QUESTION: What should they do, and why?
- MODEL ANSWER: The approach our team would expect, referencing our methodology where applicable
- DISCUSSION POINT: A follow-up question their manager could ask to deepen the conversation

3. SUGGESTED READING PLAN
A prioritized list of documents, standards, and resources to review, organized by week:
- Week 1: [Critical reads for immediate effectiveness]
- Weeks 2-4: [Deeper methodology and standards]
- Month 2-3: [Industry-specific knowledge and advanced topics]

4. 30-60-90 DAY MILESTONES
Suggest realistic milestones for what the new hire should be able to do independently at 30, 60, and 90 days.
```

## What to Expect

- A knowledge gap analysis identifying strengths and prioritized learning areas
- 10 progressive practice scenarios with model answers and discussion points
- A week-by-week reading plan
- 30-60-90 day milestone suggestions

## Tips for Better Results

- **Paste your actual methodology excerpts.** The more context the AI has about how your team works, the more relevant the scenarios will be. Even a table of contents from your audit manual helps.
- **Customize for the individual.** A CPA transitioning from Big 4 needs a very different onboarding plan than a first-time auditor. Adjust the prompt each time.
- **Use the scenarios in 1-on-1s.** Walk through one scenario per week with the new hire. It is a better use of meeting time than status updates.
- **Ask for additional scenarios by topic.** After the initial set, you can ask: "Generate 5 more scenarios focused specifically on [SOX testing / IT general controls / fraud indicators]."
- **Update when your methodology changes.** Re-run the prompt with updated methodology excerpts when your team's standards or tools change.

## Applicable Tools

ChatGPT, Claude, Microsoft Copilot

---

*Part of the [AI Prompt Templates for Internal Auditors](https://github.com/HarborViewConsulting/Internal-Audit-AI-Skills) collection by [Harbor View Consulting LLC](https://www.harborview-consulting.com). Harbor View is a Baltimore-based advisory firm helping audit, risk, and finance teams modernize through technology and AI-enabled solutions. Questions? Contact Mike Molloy, CISA at mmolloy@harborview-consulting.com.*
