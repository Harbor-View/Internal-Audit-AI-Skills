# Plain English to SQL/Python Analytics

Translate a plain English description of what you want to monitor into a working SQL query or Python script. Designed for auditors who do not write code but need to build continuous monitoring queries or one-time analytics. The output can be pasted directly into Power BI, Tableau, Excel, or a database query tool.

## When to Use

- When you know what you want to test but do not know how to write the code
- When building continuous monitoring dashboards for recurring controls
- When your IT team asks you to "just send us the query" for a data request
- When you need to quickly analyze a data extract without waiting for IT support

## What You Will Need

- A plain English description of the monitoring rule or analytic you want to build
- The column names and data types from your source data (copy/paste the header row)
- Your target platform (Power BI, Tableau, Excel, direct SQL, Python script)

## The Prompt

```
You are a data analyst helping an internal auditor who does not write code. I need you to translate my plain English description into a working [SQL query / Python script / Excel formula].

MY DATA:
- Source: [DESCRIBE THE DATA, e.g., "AP transactions exported from SAP to CSV"]
- Columns: [PASTE THE HEADER ROW OR LIST COLUMNS, e.g., "Vendor_Name, Invoice_Number, Invoice_Date, Amount, Currency, Approver, Requestor, Cost_Center, Payment_Date, PO_Number"]
- Row count: [APPROXIMATE, e.g., "~25,000 rows monthly"]

WHAT I WANT TO MONITOR:
[Describe in plain English. Examples:]
- Flag any invoices where the person who approved the invoice is also the person who submitted the purchase request
- Identify vendors who received more than $100,000 in total payments this quarter
- Find invoices that were paid before the invoice date (possible backdating)
- Detect duplicate payments: same vendor, same amount, within 5 days of each other

TARGET PLATFORM: [Choose one]
- SQL query for [SQL Server / PostgreSQL / Snowflake / MySQL / Oracle]
- Python script using pandas (reads CSV, outputs Excel with results)
- Power BI DAX measure
- Excel formula (I'll add columns to my existing spreadsheet)

REQUIREMENTS:
1. Write the complete, working code. Do not use pseudocode or abbreviations.
2. Add a comment above each section explaining what it does in plain English.
3. Include a summary output that shows: total records analyzed, records flagged, percentage flagged.
4. If writing SQL, use only standard SQL functions (no proprietary extensions unless I specified the platform).
5. If writing Python, use only pandas and openpyxl. No other libraries.
6. If writing Excel formulas, tell me which cell to put each formula in and how to copy it down.

After the code, provide:
- DEPLOYMENT INSTRUCTIONS: Step-by-step instructions for how to run this in [TARGET PLATFORM], written for someone who has never done it before.
- MODIFICATION GUIDE: Explain which parts of the code to change if I want to adjust thresholds, add filters, or apply this to a different dataset.
```

## What to Expect

- A complete, working script or query with inline comments
- Summary statistics (total analyzed, flagged, percentage)
- Step-by-step deployment instructions for your platform
- A modification guide so you can adjust it without coming back to the AI

## Tips for Better Results

- **Paste your actual column headers.** Copy row 1 of your spreadsheet and paste it directly. This prevents the AI from guessing field names.
- **Start simple, then layer.** Get one monitoring rule working first. Then ask: "Now add a second test to the same script that also checks for [X]."
- **Ask for a data quality pre-check.** Add: "Before running the analytics, check for: null values in key fields, duplicate rows, inconsistent date formats, and outlier values. Report what you find."
- **Request a scheduled version.** If you want this to run automatically, add: "Also show me how to schedule this to run weekly in [Power BI / Windows Task Scheduler / cron]."
- **Save your prompts.** Once you have a working query, save the prompt alongside the code. When the data format changes next year, you can re-run the prompt with updated column names.

## Applicable Tools

ChatGPT, Claude, Microsoft Copilot

---

*Part of the [AI Prompt Templates for Internal Auditors](https://github.com/HarborViewConsulting/Internal-Audit-AI-Skills) collection by [Harbor View Consulting LLC](https://www.harborview-consulting.com). Harbor View is a Baltimore-based advisory firm helping audit, risk, and finance teams modernize through technology and AI-enabled solutions. Questions? Contact Mike Molloy, CISA at mmolloy@harborview-consulting.com.*
