# Innovation OS

A portable enterprise product innovation framework usable by any AI coding agent.

## What This Is

Innovation OS transforms how you think about custom software projects. Instead of asking "How do we build this?", it asks **"How do we turn this into a reusable enterprise product?"**

It contains:
- A core **skill** for AI agents (the Enterprise Product Innovation Director)
- **Frameworks** for scoring, productizing, and validating opportunities
- **Templates** for structured analysis and business cases
- **Playbooks** for industry-specific guidance
- **Prompt cards** for specialized sub-agents
- **Case study templates** for building institutional product knowledge

## Philosophy

```
Client Project → Reusable Framework → Enterprise Product → Industry Platform → Strategic Business Unit
```

**Never assume a project is only a project.** Always ask: "If this solution succeeds for one customer, who are the next 100?"

## Quick Start

1. Read `AGENTS.md` — the entry point for AI agents
2. Load `skills/enterprise-product-innovation/SKILL.md` as the core skill
3. Use `frameworks/` for analysis methodology
4. Use `templates/` for structured output
5. Use `playbooks/` for industry context
6. Use `prompts/` for specialized sub-agent analysis
7. Save results in `case-studies/` as product memory

## For AI Agents (any tool: opencode, Claude Code, Cursor, Gemini CLI, Cline, etc.)

When asked to evaluate a project for product potential:
1. This AGENTS.md is your entry point
2. Always load the core skill first
3. Always produce a Product Opportunity Scorecard (/45)
4. Always classify the opportunity
5. Always answer the 8 mandatory innovation questions

## Structure

```
innovation-os/
├── AGENTS.md                           Entry point for AI agents
├── README.md                           You are here
├── skills/
│   └── enterprise-product-innovation/
│       └── SKILL.md                    Core skill — always load first
├── frameworks/
│   ├── product-opportunity-scorecard.md
│   ├── productization-framework.md
│   ├── market-validation-framework.md
│   ├── competitor-analysis-framework.md
│   └── enterprise-product-roadmap.md
├── templates/
│   ├── product-assessment.md           Complete project → product assessment
│   ├── product-canvas.md               One-page product summary
│   ├── business-case.md                Full investment business case
│   └── investment-review.md            Periodic portfolio review
├── playbooks/
│   ├── telecom.md
│   ├── government.md
│   ├── banking.md
│   └── healthcare.md
├── prompts/
│   ├── venture-analyst.md              "Should we invest?"
│   ├── product-extractor.md            "What's reusable?"
│   ├── market-researcher.md            "Is there a market?"
│   └── competitive-intelligence-analyst.md  "Who competes?"
└── case-studies/
    └── README.md                       Template + instructions
```
