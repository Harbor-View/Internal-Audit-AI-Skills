# Inputs

Place your input files in this folder before running the workflow. The orchestrator and agents will read from here.

## Expected Files

| File | Required? | Description |
|------|-----------|-------------|
| `risk-research.md` | **Required** | Risk research output (from Skill #01 or your own risk assessment). This is the primary input that drives the scoping process. |
| `prior-findings.md` | Recommended | Audit findings from prior engagements for this entity. Include: finding title, risk rating, root cause, remediation status, and whether the finding is new or repeat. |
| `walkthrough-notes.md` | Optional | Notes or transcripts from preliminary walkthroughs or planning meetings with process owners. |
| `team-availability.md` | Optional | Your team's staffing availability, skill mix, and any constraints (planned leave, co-sourcing arrangements, certification requirements). If not provided, the LOE estimator will assume a mid-size team of 4-6 professionals. |
| `entity-context.md` | Optional | Background on the entity being audited: industry, size, key systems, recent changes (M&A, leadership turnover, system implementations), regulatory environment. |

## Format

Files can be plain text (.md or .txt) or copy-pasted content. There is no required format. The agents are designed to work with whatever you have available.

If you are using Skill #01 (Risk Assessment Deep Research), save its output directly to this folder as `risk-research.md`.
