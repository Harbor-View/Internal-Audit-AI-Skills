# Report Review: Clone the Reviewer

Teach the AI your senior reviewer's style by showing it examples of their past edits and comments, then have it apply that same standard to new drafts. Catches recurring logic gaps, tone issues, and structural problems before the draft reaches the reviewer, reducing review cycles.

## When to Use

- Before submitting a draft audit report to your Head of Internal Audit or Director for review
- When onboarding new staff who need to learn what "good" looks like for your team
- When your primary reviewer is unavailable and you want to self-check against their standards

## What You Will Need

- 3-4 past audit reports with tracked changes and comments from the reviewer (the more examples, the better the AI learns the style)
- The new draft report to be reviewed

## The Prompt

```
You are going to learn the review style of a senior internal audit leader, then apply that style to review a new draft report.

STEP 1: LEARN THE REVIEW STYLE

I am going to show you [NUMBER] audit reports that were reviewed by our [TITLE, e.g., "Head of Internal Audit"]. Each includes the reviewer's tracked changes, comments, and feedback. Study these carefully to learn:

- What types of issues they consistently flag (logic gaps, unsupported conclusions, vague language, missing root causes, weak recommendations, tone problems, formatting inconsistencies)
- How they phrase their comments (direct, questioning, coaching)
- What level of specificity they expect in findings, root causes, and recommendations
- What they consider acceptable vs. unacceptable in management responses
- Any recurring feedback themes across reports

EXAMPLE REPORT 1:
[Paste the report with tracked changes and comments]

EXAMPLE REPORT 2:
[Paste the report with tracked changes and comments]

EXAMPLE REPORT 3:
[Paste the report with tracked changes and comments]

STEP 2: SUMMARIZE THE REVIEW STYLE

Before reviewing the new report, provide a summary of the patterns you identified in the reviewer's style. Include:
- Top 5 recurring issues they flag
- Their apparent priorities (what they care about most)
- Common phrases or comment styles they use
- Standards they enforce that might not be obvious

STEP 3: REVIEW THE NEW DRAFT

Now review this new draft report applying the same standards:

[Paste the new draft report]

For your review:
1. Mark each comment with the section and paragraph it applies to
2. Phrase your feedback in the reviewer's voice and style
3. Categorize each comment as: CRITICAL (must fix before submission), IMPORTANT (should fix), or SUGGESTION (nice to have)
4. After your line-by-line review, provide an overall assessment: Is this draft ready for the reviewer, or does it need another round of revision?
5. List the top 3 issues the reviewer would flag first
```

## What to Expect

- A summary of the reviewer's patterns and priorities
- Line-by-line comments on the new draft, phrased in the reviewer's style
- Comments categorized by severity (Critical / Important / Suggestion)
- An overall readiness assessment
- The top issues the reviewer would likely flag first

## Tips for Better Results

- **Use reports with rich tracked changes.** The more edits and comments in your examples, the better the AI learns the reviewer's standards. A clean final report teaches nothing.
- **Include reports across different topics.** Show a financial audit, an IT audit, and an operational audit if available. This helps the AI distinguish style preferences from topic-specific feedback.
- **Use a tool with a large context window.** Multiple full reports with tracked changes consume significant tokens. Claude (1M context) handles this well.
- **Update your examples periodically.** As your reviewer's expectations evolve, swap in recent examples to keep the AI's model current.
- **Share the style summary with your team.** The Step 2 output is useful as a standalone "review standards" document for onboarding new staff.

## Applicable Tools

Claude (large context window preferred for multiple reports), ChatGPT, Microsoft Copilot

---

*Part of the [AI Prompt Templates for Internal Auditors](https://github.com/HarborViewConsulting/Internal-Audit-AI-Skills) collection by [Harbor View Consulting LLC](https://www.harborview-consulting.com). Harbor View is a Baltimore-based advisory firm helping audit, risk, and finance teams modernize through technology and AI-enabled solutions. Questions? Contact Mike Molloy, CISA at mmolloy@harborview-consulting.com.*
