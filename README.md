# AI Prompt Templates for Internal Auditors

A collection of ready-to-use AI prompt templates designed for Internal Audit professionals. Each template is a complete workflow you can copy, paste, and use immediately in ChatGPT, Claude, Microsoft Copilot, or any other AI tool. No coding or AI experience required.

**Created by** [Harbor View Consulting LLC](https://www.harborview-consulting.com)
**Companion to** "Practical AI Use Cases for Internal Auditors" (IIA Baltimore Chapter, April 2026)

---

## What Is This?

This is a library of AI "skills" for internal auditors. Each skill is a markdown file (.md) containing a detailed prompt template that tells an AI tool exactly what to do for a specific audit task.

Think of each skill as a set of instructions you hand to a very capable assistant who knows nothing about your organization. The prompt gives them the context, structure, and guardrails to produce useful output on the first try.

**You do not need to know how to code, program, or build anything.** You just need access to an AI tool and the ability to copy and paste.

---

## What Is in This Repo?

### Single-File Skills (11 templates)

| # | Skill | What It Does |
|---|-------|-------------|
| 01 | [Risk Assessment Deep Research](skills/01-risk-assessment-deep-research.md) | Generates a structured risk research report from public sources to support your annual risk assessment |
| 03 | [Smart PBC Request Generator](skills/03-smart-pbc-request.md) | Transforms vague PBC requests into specific, complete requests that get evidence on the first try |
| 04 | [Walkthrough Transcript to Workpaper](skills/04-walkthrough-to-workpaper.md) | Converts a meeting transcript into a formatted audit workpaper that meets IIA documentation standards |
| 05 | [Population Testing & Exception Filtering](skills/05-population-testing.md) | Writes SQL, Python, or Excel formulas to test 100% of a transaction population instead of sampling |
| 06 | [Cross-Audit Pattern Recognition](skills/06-cross-audit-patterns.md) | Analyzes findings across multiple audits to surface systemic root causes |
| 07 | [Audit Committee Dry-Run](skills/07-audit-committee-dryrun.md) | Simulates how your Audit Committee Chair would react to a draft report before the real meeting |
| 08 | [Clone the Reviewer](skills/08-clone-the-reviewer.md) | Teaches the AI your senior reviewer's editing style, then applies it to new draft reports |
| 09 | [Plain English to SQL/Python](skills/09-plain-english-analytics.md) | Translates plain English monitoring rules into working code you can paste into Power BI or Excel |
| 10 | [Recruiting Due Diligence](skills/10-recruiting-due-diligence.md) | Cross-references a candidate's resume against public records to validate claims before an interview |
| 11 | [Flashcard Generator](skills/11-flashcard-generator.md) | Converts IIA Standards, COSO updates, or any guidance document into study flashcards with page references |
| 12 | [New Hire Onboarding Q&A](skills/12-onboarding-qa.md) | Creates a tailored study guide and practice scenarios for onboarding new audit team members |

### Multi-Agent Workflow (1 advanced example)

| # | Skill | What It Does |
|---|-------|-------------|
| 02 | [Audit Scoping & LOE Estimation](skills/02-audit-scoping-loe/) | Three specialized AI agents work together to produce a complete audit scoping package with risk-based scope, standards alignment, and level-of-effort estimates |

---

## How to Use These Templates

### Option 1: Copy and Paste (Works With Any AI Tool)

This is the simplest approach and works with ChatGPT, Claude, Microsoft Copilot, or any other AI chat tool.

1. **Pick a skill** from the table above and click the link to open it
2. **Read the "What You Will Need" section** to gather your inputs (a draft PBC request, a transcript, a list of findings, etc.)
3. **Copy the prompt** from the "The Prompt" section (the text inside the code block)
4. **Paste it into your AI tool** (ChatGPT, Claude, Copilot, etc.)
5. **Replace the bracketed placeholders** like `[COMPANY NAME]` or `[PASTE YOUR DATA HERE]` with your actual information
6. **Send the prompt** and review the output

That's it. No setup, no installation, no account configuration.

### Option 2: Use With Claude Code (More Powerful)

[Claude Code](https://docs.anthropic.com/en/docs/claude-code) is a command-line tool from Anthropic that can read files, work with folders, and run multi-step workflows. If you use Claude Code, you can point it directly at these skill files instead of copying and pasting.

**For single-file skills:**

Open Claude Code and ask it to use a specific skill:

```
Read the skill file at skills/03-smart-pbc-request.md and use it to improve
this PBC request: [paste your request]
```

Or if you have cloned this repo locally:

```
Use the Smart PBC Request skill in this repo to rewrite my PBC request
for the Q1 2026 AP audit. Here is my draft: [paste your request]
```

**For the multi-agent workflow (Skill #2):**

Copy the `skills/02-audit-scoping-loe/` folder into your working directory. Claude Code reads the `CLAUDE.md` file automatically and coordinates the three agent files for you. Just provide your risk research and prior findings, and ask Claude Code to produce a scoping package.

### Option 3: Download a Single File

You do not need to download the entire repository. To grab just one skill:

1. Click the skill link in the table above
2. Click the **Raw** button (top right of the file view on GitHub)
3. Save the page (Ctrl+S or Cmd+S) as a `.md` file on your computer
4. Open it in any text editor (Notepad, TextEdit, VS Code) and copy the prompt

---

## Which AI Tool Should I Use?

All of these templates work across major AI tools. Some work better in certain tools:

| Tool | Best For | Notes |
|------|----------|-------|
| **ChatGPT** (Plus or Enterprise) | Most skills; especially Skill #1 and #10 | "Deep Research" mode is best for skills that require web searching |
| **Claude** (Pro or Team) | Skills with large inputs (#4, #8) | 1M token context window handles long transcripts and multiple reports |
| **Microsoft Copilot** | Teams already in the Microsoft 365 ecosystem | Works well for all skills; integrates with your existing Office workflow |
| **Claude Code** | Skill #2 (multi-agent workflow) | Reads folder structures and coordinates multiple agent files automatically |

If you are not sure where to start, use whichever AI tool you already have access to. These prompts are designed to work everywhere.

---

## Where to Start

If you are new to using AI in audit, start with these three. They require minimal setup and produce useful output on the first try:

1. **[Risk Assessment Deep Research](skills/01-risk-assessment-deep-research.md)** -- Pick a company you are about to audit and ask the AI to research its top risks. Compare the output to your current risk assessment.

2. **[Smart PBC Request Generator](skills/03-smart-pbc-request.md)** -- Before sending your next PBC request, paste a draft into the AI and ask it to make it more specific. Compare what comes back to what you would have sent.

3. **[Flashcard Generator](skills/11-flashcard-generator.md)** -- Paste the latest IIA Standards update and ask for 10 flashcards. You will have a study aid in under a minute.

---

## Tips for Getting Good Results

- **Be specific with your inputs.** The more context you provide (company name, industry, audit period, system name, column headers), the more useful the output.
- **Iterate.** If the first output is not quite right, tell the AI what to change. ("Make the PBC request more specific about date ranges." "Add a column for risk rating.") AI tools improve with feedback.
- **Verify before you rely.** AI can make mistakes. Always review the output with professional judgment before using it in your work. These tools augment your expertise; they do not replace it.
- **Start small.** Try one skill on one task. Once you see the value, expand to others.

---

## About

These templates were developed by [Harbor View Consulting LLC](https://www.harborview-consulting.com), a Baltimore-based advisory firm specializing in audit, risk, and technology consulting.

Questions or feedback? Reach out to **Mike Molloy, CISA** at mmolloy@harborview-consulting.com.

---

## License

This work is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

You are free to use, share, and adapt these templates for any purpose, including commercial use, as long as you provide attribution to Harbor View Consulting LLC. See [LICENSE](LICENSE) for details.
