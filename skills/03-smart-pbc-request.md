# Smart PBC Request Generator

Transform generic PBC (Prepared by Client) requests into hyper-specific, complete requests that minimize back-and-forth with the client. The AI adds precise date ranges, required data fields, file format expectations, and parameter specifications so evidence arrives complete on the first try.

## When to Use

- Before sending any PBC request to a client or process owner
- When onboarding a new auditor who needs help writing precise requests
- When working with a new client or process area where you are less familiar with the data available

## What You Will Need

- Your draft or generic PBC request language
- The audit period (start and end dates)
- The process area or control being tested
- Optionally: the client's ERP or system (SAP, Oracle, NetSuite, Workday, etc.)

## The Prompt

```
You are an experienced internal auditor who is known for writing exceptionally clear, specific PBC (Prepared by Client) requests that get complete evidence on the first try.

I am preparing PBC requests for a [PROCESS AREA] audit covering [START DATE] through [END DATE]. The client uses [SYSTEM NAME, if known].

Here is my current draft request:

"[PASTE YOUR GENERIC PBC REQUEST HERE]"

Rewrite this request to be as specific as possible. For each item requested, include:

1. EXACT DATE RANGE -- Specify the precise period (e.g., "January 1, 2026 through March 31, 2026")
2. REQUIRED DATA FIELDS -- List every column or field needed (e.g., vendor name, invoice number, invoice date, amount, GL account, approver name, approval date)
3. FILE FORMAT -- Specify the preferred format (e.g., "Excel (.xlsx) with one row per transaction, no merged cells, no subtotals")
4. SYSTEM PARAMETERS -- If the request involves a system report, describe the report parameters or selection criteria (e.g., "Include a screenshot of the report selection screen showing the date range and filters applied")
5. SUPPORTING DOCUMENTATION -- Any additional items needed to validate the data (e.g., sampling methodology documentation, system configuration screenshots, approval delegation matrices)
6. COMPLETENESS CHECK -- Add a note asking the client to confirm that the population is complete (e.g., "Please confirm this extract represents 100% of [transactions] for the period, with no exclusions")

Also add:
- A requested delivery date: [DATE OR "within 5 business days"]
- A contact name for questions: [YOUR NAME]
- A brief explanation of why each item is needed, so the client understands the purpose and can flag potential issues early

Write the final PBC request in a professional, collaborative tone. The goal is clarity, not intimidation.
```

## What to Expect

- A rewritten PBC request with specific fields, date ranges, and format requirements for each item
- A completeness confirmation request
- Professional, collaborative tone that explains the "why" behind each ask
- Suggested follow-up language if the initial request is incomplete

## Tips for Better Results

- **Include the system name.** If you tell the AI the client runs SAP, it can reference specific transaction codes or standard report names. Same for Oracle, NetSuite, Workday, etc.
- **Paste multiple requests at once.** You can include your full PBC list and ask the AI to enhance all of them in one pass.
- **Ask for a "PBC tracker" format.** Add to the prompt: "Also produce a summary table with columns: Item #, Description, Requested Format, Due Date, Status" for tracking purposes.
- **Iterate for your team's style.** After the first output, tell the AI what to adjust ("we never ask for screenshots," "add a column for responsible party") and it will refine.

## Applicable Tools

ChatGPT, Claude, Microsoft Copilot

---

*Part of the [AI Prompt Templates for Internal Auditors](https://github.com/HarborViewConsulting/Internal-Audit-AI-Skills) collection by [Harbor View Consulting LLC](https://www.harborview-consulting.com). Harbor View is a Baltimore-based advisory firm helping audit, risk, and finance teams modernize through technology and AI-enabled solutions. Questions? Contact Mike Molloy, CISA at mmolloy@harborview-consulting.com.*
