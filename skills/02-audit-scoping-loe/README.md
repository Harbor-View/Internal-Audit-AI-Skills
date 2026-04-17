# Audit Scoping and LOE Estimation (Multi-Agent Workflow)

This skill demonstrates how to use a folder structure with multiple agent files to orchestrate a complex audit planning workflow. Instead of a single prompt, three specialized agents work under an orchestrator to produce a complete audit scoping package.

This is a **Claude Code** example. It uses CLAUDE.md files and agent sub-folders that Claude Code reads automatically when working in a project directory. If you are not using Claude Code, you can still use the individual agent prompts as standalone templates in any AI tool.

## How It Works

```
02-audit-scoping-loe/
├── README.md                                   # This file
├── CLAUDE.md                                   # Orchestrator (coordinates the agents)
├── inputs/                                     # You put your files here
│   ├── README.md                               # Describes what to provide
│   ├── risk-research.md                        # Required: risk research output
│   ├── prior-findings.md                       # Recommended: prior audit findings
│   ├── walkthrough-notes.md                    # Optional: walkthrough notes
│   ├── team-availability.md                    # Optional: staffing info
│   └── entity-context.md                       # Optional: entity background
├── outputs/                                    # Agents write results here
│   ├── README.md                               # Describes what gets produced
│   ├── risk-summary.md                         # From: Research Synthesizer
│   ├── standards-alignment.md                  # From: Standards Alignment
│   ├── loe-estimate.md                         # From: LOE Estimator
│   └── scoping-package.md                      # From: Orchestrator (final deliverable)
└── agents/                                     # One subfolder per agent
    ├── research-synthesizer/
    │   └── agent.md                            # Synthesizes risk research into scoping inputs
    ├── standards-alignment/
    │   └── agent.md                            # Maps scope to IIA/ISACA standards
    └── loe-estimator/
        └── agent.md                            # Builds the LOE and resource estimate
```

**The orchestrator** (CLAUDE.md) coordinates the three agents in sequence:
1. The **Research Synthesizer** reads your inputs and distills them into a ranked list of auditable areas with risk rationale.
2. The **Standards Alignment** agent maps proposed scope items to IIA Standards and relevant frameworks, ensuring nothing required is missed.
3. The **LOE Estimator** takes the scoped items and produces a staffing, timeline, and effort estimate grounded in complexity analysis.

The orchestrator combines their outputs into a single audit scoping package written to `outputs/scoping-package.md`, ready for senior review and board approval.

## What You Will Need

Place your input files in the `inputs/` folder. See `inputs/README.md` for details on each file.

| File | Required? | Description |
|------|-----------|-------------|
| `risk-research.md` | **Required** | Risk research output (from Skill #01 or your own assessment) |
| `prior-findings.md` | Recommended | Prior audit findings with ratings and remediation status |
| `walkthrough-notes.md` | Optional | Preliminary walkthrough notes or meeting transcripts |
| `team-availability.md` | Optional | Team size, skills, availability, and constraints |
| `entity-context.md` | Optional | Entity background (industry, size, systems, recent changes) |

## Using With Claude Code

1. Copy this entire `02-audit-scoping-loe/` folder into your project directory
2. Place your input files in the `inputs/` folder
3. Open Claude Code in the folder and say: "Run the audit scoping workflow using the inputs I provided"
4. Claude Code reads the CLAUDE.md orchestrator, runs each agent in sequence, and writes results to `outputs/`
5. Review `outputs/scoping-package.md` and adjust before presenting to leadership

## Using Without Claude Code

You can use each agent's prompt independently in any AI tool by running them in sequence:

1. **Open** `agents/research-synthesizer/agent.md`, copy the instructions, and paste them into your AI tool along with your risk research and prior findings. Save the output.
2. **Open** `agents/standards-alignment/agent.md`, copy the instructions, and paste them into your AI tool along with the output from Step 1. Save the output.
3. **Open** `agents/loe-estimator/agent.md`, copy the instructions, and paste them into your AI tool along with the outputs from Steps 1 and 2, plus your team availability info. Save the output.
4. **Combine** all three outputs into a single scoping document using the format in CLAUDE.md.

## What You Get

After running the workflow, the `outputs/` folder will contain:

- **risk-summary.md** -- Ranked auditable areas with risk scores, rationale, and prior finding history
- **standards-alignment.md** -- Mapping to IIA Standards and control frameworks, with gap analysis
- **loe-estimate.md** -- Hours by phase, staffing plan, timeline, and resource assumptions
- **scoping-package.md** -- The complete deliverable combining all of the above, ready for review

## Applicable Tools

- **Full workflow:** Claude Code (reads the folder structure natively)
- **Individual prompts:** ChatGPT, Claude, Microsoft Copilot

---

*Part of the [AI Prompt Templates for Internal Auditors](https://github.com/HarborViewConsulting/Internal-Audit-AI-Skills) collection by [Harbor View Consulting LLC](https://www.harborview-consulting.com). Harbor View is a Baltimore-based advisory firm helping audit, risk, and finance teams modernize through technology and AI-enabled solutions. Questions? Contact Mike Molloy, CISA at mmolloy@harborview-consulting.com.*
