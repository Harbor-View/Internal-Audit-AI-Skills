# Cross-Audit Pattern Recognition

Analyze findings across multiple audits to surface systemic patterns and root causes that are not visible when reviewing individual reports. The AI identifies connections between disparate findings and drafts remediation recommendations that address the underlying issue rather than individual symptoms.

## When to Use

- During annual reporting when summarizing the year's audit results for the Audit Committee
- When you suspect related findings across departments share a common root cause
- When preparing a thematic or horizontal review across business units
- When building the case for a systemic remediation initiative

## What You Will Need

- Audit findings from multiple engagements (the more the better)
- For each finding: the title, department or business unit, finding category, risk rating, root cause (if documented), and current remediation status
- Optionally: the time period each audit covered and whether findings are new or repeat

## The Prompt

```
You are a senior internal audit leader preparing an analysis of findings across multiple audits to identify systemic patterns for Audit Committee reporting.

Here are the findings from [NUMBER] audits completed between [START DATE] and [END DATE]:

[PASTE FINDINGS -- for each include:]
- Audit name
- Department / business unit
- Finding title
- Finding description (brief)
- Risk rating (Critical / High / Medium / Low)
- Root cause (if documented)
- Remediation status (Open / In Progress / Closed / Overdue)
- New or repeat finding

Analyze these findings for systemic patterns. Specifically:

1. PATTERN IDENTIFICATION
Group related findings by common root cause or theme, even if they span different departments or audit types. Look for patterns that would not be obvious when reading individual reports in isolation.

2. ROOT CAUSE ANALYSIS
For each pattern identified, describe the likely systemic root cause. Go beyond surface-level explanations ("process gap") to identify structural drivers (e.g., lack of automated reconciliation across systems, no centralized policy ownership, inadequate segregation of duties in the shared services model).

3. TREND ANALYSIS
Identify any trends: are certain categories of findings increasing? Are repeat findings concentrated in specific areas? Are overdue remediations clustering around a particular root cause?

4. REMEDIATION RECOMMENDATIONS
For each systemic pattern, draft a remediation recommendation that addresses the root cause rather than individual symptoms. Include:
- The specific action to take
- Who should own it (role, not person name)
- Estimated complexity (Low / Medium / High)
- Expected impact on future findings if implemented

5. AUDIT COMMITTEE TALKING POINTS
Draft 3-5 talking points I can use when presenting this analysis to the Audit Committee. Focus on:
- What the patterns mean for organizational risk
- Where management attention is most needed
- Any resource or governance implications

6. VISUAL SUMMARY
Provide a simple text-based summary table showing: Pattern Name | # of Related Findings | Departments Affected | Aggregate Risk | Recommended Action

Do not manufacture patterns that are not supported by the data. If findings appear unrelated, say so. The goal is honest analysis, not forcing connections.
```

## What to Expect

- Grouped findings organized by systemic root cause
- A narrative explaining each pattern and why it matters
- Trend analysis highlighting escalation risks
- Remediation recommendations targeting root causes
- Ready-to-use Audit Committee talking points
- A summary table for reporting

## Tips for Better Results

- **Include finding descriptions, not just titles.** Titles alone often lack enough detail for the AI to identify connections.
- **Include historical data if possible.** Findings from the prior year help the AI identify trends and repeat issues.
- **Export from your GRC tool.** If you use AuditBoard, Workiva, or similar, export your findings register to CSV and paste or attach it.
- **Ask for a heatmap narrative.** Add: "Also describe what a heatmap of these findings would look like, organized by department (rows) and risk category (columns)."
- **Iterate on patterns.** If the AI identifies a pattern you disagree with, tell it why and ask it to re-analyze. Your organizational knowledge is essential context.

## Applicable Tools

ChatGPT, Claude, Microsoft Copilot

---

*Part of the [AI Prompt Templates for Internal Auditors](https://github.com/HarborViewConsulting/Internal-Audit-AI-Skills) collection by [Harbor View Consulting LLC](https://www.harborview-consulting.com). Harbor View is a Baltimore-based advisory firm helping audit, risk, and finance teams modernize through technology and AI-enabled solutions. Questions? Contact Mike Molloy, CISA at mmolloy@harborview-consulting.com.*
