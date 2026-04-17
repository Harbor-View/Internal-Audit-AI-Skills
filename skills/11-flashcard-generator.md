# Standards and Guidance Flashcard Generator

Convert dense guidance documents (IIA Standards, COSO updates, regulatory changes, firm methodology updates) into concise flashcards for rapid recall. Each flashcard is grounded entirely in the source document with page references so you can verify every answer.

## When to Use

- When new IIA Standards, COSO guidance, or regulatory requirements are released
- When onboarding team members who need to get up to speed on a specific standard or methodology
- When preparing for a certification exam (CIA, CISA, CPA) and need to distill study materials
- When your firm updates its audit methodology and you need to train the team on changes

## What You Will Need

- The guidance document (pasted text or uploaded PDF)
- Your experience level and industry context (so examples are relevant to you)
- The number of flashcards you want

## The Prompt

```
You are a professional development specialist for internal auditors. I need you to create flashcards from a guidance document. 

CRITICAL RULES:
- Use ONLY the content from the document I provide below. Do not supplement with outside knowledge, training data, or assumptions.
- Every flashcard answer MUST include a page number, section number, or paragraph reference from the source document so I can verify it against the original.
- If the document does not contain enough information to create a complete flashcard on a topic, skip it rather than filling in gaps from other sources.
- If you are unsure whether something is in the document, do not include it.

MY CONTEXT:
- Role: [e.g., "Senior Internal Auditor with 5 years of experience"]
- Industry: [e.g., "financial services" or "healthcare" or "manufacturing"]
- Focus: [e.g., "I need to understand what changed from the prior version" or "I'm learning this for the first time"]

THE DOCUMENT:
[Paste the full text or upload the PDF]

Create [NUMBER, e.g., 15] flashcards covering the most significant content. Prioritize:
- New requirements or changes from prior versions (if this is an update)
- Requirements that directly affect day-to-day audit work
- Concepts that are commonly tested on certification exams (if applicable)

FLASHCARD FORMAT:

For each flashcard:

FRONT (Question/Concept):
[A clear, specific question that tests understanding, not just recall]

BACK (Answer):
[A concise answer that includes:]
- The direct answer from the document
- A practical example of how this applies to a [MY INDUSTRY] internal audit team
- What changed from the prior version (if applicable and if the document addresses this)
- Source reference: [Page X, Section Y.Z, Paragraph N]

After all flashcards, provide:
- A "KEY THEMES" summary (3-5 bullet points) of the most important takeaways from the document
- A list of topics in the document you did NOT cover in flashcards, so I know what else is available for a second round

OPTIONAL: If I want to import these into a flashcard app, also provide the content in a simple two-column format (Front | Back) separated by tabs, which I can paste into Anki or Quizlet.
```

## What to Expect

- A set of flashcards, each with a question, answer, practical example, and source reference
- Answers grounded exclusively in the provided document
- Page/section references on every card for verification
- A key themes summary
- A list of uncovered topics for a potential second round
- Optionally: an importable format for Anki or Quizlet

## Tips for Better Results

- **Upload the full document, not a summary.** The AI can only cite page numbers if it has the original document. A summary loses the references.
- **Specify "what changed" if this is an update.** If you are studying a revised standard (e.g., IIA 2024 Standards replacing the IPPF), tell the AI so it can focus on changes rather than fundamentals.
- **Spot-check the page references.** Verify at least 3-4 flashcard answers against the source document to confirm the AI is citing accurately. If references are off, tell the AI which ones were wrong and ask it to correct.
- **Generate in batches.** If the document is long, ask for 15 flashcards on Part 1, then another 15 on Part 2. This produces better coverage than asking for 50 at once.
- **Share with your team.** The Anki/Quizlet export format makes it easy to distribute flashcard sets across the audit department.

## Applicable Tools

ChatGPT, Claude, Microsoft Copilot

---

*Part of the [AI Prompt Templates for Internal Auditors](https://github.com/HarborViewConsulting/Internal-Audit-AI-Skills) collection by [Harbor View Consulting LLC](https://www.harborview-consulting.com). Harbor View is a Baltimore-based advisory firm helping audit, risk, and finance teams modernize through technology and AI-enabled solutions. Questions? Contact Mike Molloy, CISA at mmolloy@harborview-consulting.com.*
