# Population Testing and Exception Filtering

Move from sample-based testing to population-level analysis. The AI writes test scripts (SQL, Python, or Excel formulas) that validate every transaction in a dataset against your defined criteria, then filters down to only the exceptions that require human judgment.

## When to Use

- When you have a full data extract and want to test 100% of the population instead of sampling
- When building continuous monitoring queries for recurring control tests
- When you need a script but nobody on the team writes SQL or Python

## What You Will Need

- A transaction data export (CSV or Excel)
- The control criteria or test conditions you want to apply
- Your preferred output format (Python, SQL, or Excel formula)
- Optionally: tolerance thresholds or materiality limits

## The Prompt

```
You are a data analyst supporting an internal audit team. I have a data export and need to test the full population against specific control criteria.

DATA DESCRIPTION:
- Source: [SYSTEM NAME AND REPORT NAME, e.g., "SAP FBL1N vendor line items"]
- Record count: [APPROXIMATE NUMBER, e.g., "approximately 10,000 transactions"]
- Columns: [LIST ALL COLUMN NAMES AND DATA TYPES, e.g., "Vendor Name (text), Invoice Number (text), Invoice Date (date), Amount (decimal), Approver (text), Requestor (text), GL Account (text), Payment Date (date)"]
- Period: [START DATE] through [END DATE]

TEST CRITERIA:
[Describe each test in plain English. Examples:]
- Flag any invoice where the Approver is the same person as the Requestor (segregation of duties violation)
- Flag any invoice amount that exceeds $10,000 without a secondary approval
- Flag any invoice where the Payment Date is more than 5 business days before the Invoice Date
- Flag duplicate invoice numbers for the same vendor

[Add any thresholds:]
- Materiality threshold: [AMOUNT, e.g., "ignore exceptions under $500"]
- Known exceptions to exclude: [ANY ITEMS TO FILTER OUT, e.g., "exclude vendor 'PETTY CASH'"]

OUTPUT FORMAT: [Choose one]
- Python script (pandas) that reads a CSV and outputs an Excel file of exceptions
- SQL query I can run against [DATABASE TYPE, e.g., "SQL Server, PostgreSQL, Snowflake"]
- Excel formulas I can add to my existing spreadsheet

For each test, the output must include:
1. The test script or formula with inline comments explaining each step
2. A summary section that calculates: total records tested, exceptions found, exception rate (%)
3. The exception listing with all relevant fields for each flagged record
4. A "Test Results" header block with: test name, test criteria, population size, sample size (N/A for full population), exceptions, and a placeholder for the auditor's conclusion

Explain what each part of the code does so I can modify it for future tests. Do not use any external libraries beyond pandas and openpyxl (for Python) or standard SQL functions.
```

## What to Expect

- A working script or formula set with inline comments
- An exception listing with all relevant fields for each flagged item
- Summary statistics: total tested, exceptions found, exception rate
- Clear explanations of the logic so you can modify it later

## Tips for Better Results

- **Paste your column headers directly.** Copy the first row of your spreadsheet and paste it into the prompt. This avoids mismatched field names.
- **Start with one test, then add more.** Get a working script for your first test condition, verify it works, then ask the AI to add additional tests to the same script.
- **Ask for a "data quality check" first.** Before running your tests, add: "First, check the data for: null values in key fields, duplicate records, date format inconsistencies, and any obvious data quality issues."
- **Request a visualization.** Add: "Also create a simple bar chart showing exception counts by [vendor / department / month]" for reporting purposes.
- **Test the code on a small sample first.** Run the script on the first 100 rows to verify it works before processing the full population.

## Applicable Tools

ChatGPT, Claude, Microsoft Copilot (for script generation); execute results in Python, SQL client, or Excel

---

*Part of the [AI Prompt Templates for Internal Auditors](https://github.com/HarborViewConsulting/Internal-Audit-AI-Skills) collection by [Harbor View Consulting LLC](https://www.harborview-consulting.com). Harbor View is a Baltimore-based advisory firm helping audit, risk, and finance teams modernize through technology and AI-enabled solutions. Questions? Contact Mike Molloy, CISA at mmolloy@harborview-consulting.com.*
