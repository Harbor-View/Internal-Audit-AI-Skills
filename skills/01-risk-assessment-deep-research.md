# Risk Assessment Deep Research

Generate a structured risk research report to support your team's annual risk assessment. The AI synthesizes publicly available information across financial filings, regulatory developments, industry reports, peer disclosures, and news coverage, then organizes findings into categories that map directly to your risk assessment process.

## When to Use

- During your annual risk assessment (Phase 1: Preparation and Context-Setting)
- When updating your audit universe with emerging or external risks
- Before management interviews, to come prepared with industry-specific talking points
- When benchmarking your risk priorities against peer organizations

## What You Will Need

- The company or business unit name
- Industry and sector context
- Optionally: your current audit universe or prior risk assessment results, so the AI can identify gaps

## The Prompt

```
You are an experienced internal audit research analyst. I need you to conduct deep research to support my team's annual risk assessment for [COMPANY NAME], a [INDUSTRY/SECTOR] company [optional: with operations in REGIONS].

Search public sources thoroughly, including SEC filings (10-K, 10-Q, proxy statements, 8-Ks), earnings call transcripts, analyst reports, regulatory enforcement actions, industry association publications, peer company disclosures, and recent news coverage.

Produce a structured risk research report with the following sections:

1. INDUSTRY RISK LANDSCAPE
Current and emerging risks specific to the [INDUSTRY] sector. Source from regulatory actions, professional publications (IIA, ISACA, COSO), and peer disclosures. Identify risks that should be in any [INDUSTRY] audit universe.

2. REGULATORY AND LEGISLATIVE CHANGES
New or pending regulations affecting the organization's risk profile. For each, assess the compliance timeline and potential impact on internal controls. Include both industry-specific regulations and broad requirements (data privacy, ESG disclosure, cybersecurity reporting).

3. MACROECONOMIC AND GEOPOLITICAL FACTORS
Economic conditions, supply chain dynamics, labor market trends, interest rate environment, and geopolitical developments relevant to the organization's operations and markets.

4. TECHNOLOGY AND CYBERSECURITY RISKS
Emerging technology threats, data privacy developments, AI governance requirements, third-party technology dependencies, and IT infrastructure risks relevant to the industry.

5. ORGANIZATION-SPECIFIC RISK INDICATORS
Based on public filings and disclosures for [COMPANY NAME]: recent M&A activity, leadership changes, revenue shifts, strategic pivots, restructuring, litigation, or disclosed material weaknesses / significant deficiencies.

6. PEER BENCHMARKING
What risks are peer organizations in [INDUSTRY] prioritizing in their proxy statements, risk committee reports, and public disclosures? Identify any risks peers are flagging that are absent from common audit universes.

7. SUGGESTED RISK SCORING INPUTS
Where available, provide quantitative data (incident rates, regulatory fine ranges, breach statistics, industry loss data) that can inform likelihood and impact scoring on a 5x5 matrix.

8. RECOMMENDED ADDITIONS TO THE AUDIT UNIVERSE
Based on your research, suggest specific auditable entities, processes, or risk areas that should be considered for addition to the audit universe. For each, provide a brief rationale.

For every finding:
- Cite the specific source (publication name, date, URL where available)
- Assign a confidence rating: HIGH (multiple corroborating sources), MEDIUM (single credible source), or LOW (inferred or limited sourcing)
- Note the date of the source information

Important: This report is an INPUT to our risk assessment, not a replacement for it. Focus on providing well-sourced intelligence. Do not attempt to produce final risk scores or audit plan recommendations. Our team will apply organizational context, risk appetite, and professional judgment to score and prioritize these risks.
```

## What to Expect

- A structured report organized by the 8 sections above
- Source citations with dates for each finding
- Confidence ratings (High / Medium / Low) on each item
- Quantitative data points where available for risk scoring
- Suggested audit universe additions with rationale

## Tips for Better Results

- **Use a tool with web browsing / deep research capability.** This prompt is designed for tools that can actually search and retrieve current information (ChatGPT Deep Research, Claude with web search, Copilot). Without web access, the output will be limited to the AI's training data.
- **Provide your current audit universe** as an attachment or pasted list. This lets the AI identify gaps rather than restating risks you already track.
- **Run this for each major business unit** if your organization is diversified. Risk profiles vary significantly across segments.
- **Cross-reference with your ERM register.** Per IIA Standard 9.4, you should only rely on management's risk information if you have independently concluded their risk management processes are effective. This report helps you build that independent view.
- **Validate before scoring.** The AI's confidence ratings help, but verify HIGH-confidence items against primary sources before they influence your risk scores. A cited source is not the same as a verified source.

## Applicable Tools

ChatGPT Deep Research, Claude (with web search), Microsoft Copilot

## IIA Standards Alignment

This skill supports compliance with:
- **Standard 9.1** -- Understanding governance, risk management, and control processes
- **Standard 9.4** -- Developing a risk-based internal audit plan informed by a documented assessment of strategies, objectives, and risks
- **Standard 9.5** -- Coordination with other assurance providers to optimize risk coverage

---

*Part of the [AI Prompt Templates for Internal Auditors](https://github.com/HarborViewConsulting/Internal-Audit-AI-Skills) collection by [Harbor View Consulting LLC](https://www.harborview-consulting.com). Harbor View is a Baltimore-based advisory firm helping audit, risk, and finance teams modernize through technology and AI-enabled solutions. Questions? Contact Mike Molloy, CISA at mmolloy@harborview-consulting.com.*
