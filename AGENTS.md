# Innovation OS — AGENTS.md

This is the entry point for the **Innovation Operating System** — a portable enterprise product innovation framework usable by any AI coding agent (Codex, Claude Code, Cursor, Gemini CLI, Cline, RooCode, Aider, etc.).

## How AI Agents Should Use This

When you are asked to evaluate a project, proposal, RFP, SRS document, meeting notes, or solution architecture for product potential:

1. **Load the core skill**: `skills/enterprise-product-innovation/SKILL.md`
2. **Reference frameworks** as needed from `frameworks/`
3. **Use templates** to produce structured output from `templates/`
4. **Reference playbooks** for industry-specific guidance from `playbooks/`
5. **Invoke sub-agent prompts** for specialized analysis from `prompts/`
6. **Record findings** as case studies in `case-studies/`

## Core Principles

- **Never assume a project is only a project.** Always ask: "Who are the next 100 customers?"
- **Optimize for product creation, not project delivery.**
- **Score everything** using the Product Opportunity Scorecard (out of 45), with confidence weighting.
- **Grade all evidence** (A/B/C/D/E/V). Facts over assumptions over guesses.
- **Classify everything**: Custom Project → Reusable Framework → Enterprise Product → Industry Platform → Strategic Business Unit.
- **Stage everything**: EXPLORE → VALIDATE → INCUBATE → SCALE → OPTIMIZE.
- **Challenge every requirement.** Not "How do we build this?" but "How do we turn this into a reusable enterprise product?"
- **Know when to kill.** Every opportunity needs explicit kill criteria.

## Innovation OS Structure

```
innovation-os/
├── AGENTS.md                          ← You are here
├── README.md
├── skills/
│   └── enterprise-product-innovation/
│       └── SKILL.md                   ← Core skill (always load first)
├── frameworks/
│   ├── product-opportunity-scorecard.md
│   ├── productization-framework.md
│   ├── market-validation-framework.md
│   ├── competitor-analysis-framework.md
│   ├── enterprise-product-roadmap.md
│   ├── evidence-quality-framework.md  ← NEW: Evidence grading, confidence levels
│   ├── stage-gate-governance.md       ← NEW: EXPLORE→VALIDATE→INCUBATE→SCALE→KILL
│   ├── portfolio-strategy-framework.md ← NEW: Portfolio fit, opportunity cost, large-company lens
│   └── financial-modeling-framework.md ← NEW: Mandatory financials, ARR paths, funding
├── templates/
│   ├── product-assessment.md
│   ├── product-canvas.md
│   ├── business-case.md
│   └── investment-review.md
├── playbooks/
│   ├── telecom.md
│   ├── government.md
│   ├── banking.md
│   └── healthcare.md
├── prompts/
│   ├── venture-analyst.md
│   ├── product-extractor.md
│   ├── market-researcher.md
│   └── competitive-intelligence-analyst.md
└── case-studies/
    └── README.md
```

## The 5 Agent Workflow

For comprehensive analysis, chain these agents:

1. **Enterprise Product Innovation Director** (`skills/enterprise-product-innovation/SKILL.md`)
   — Find product opportunities. Score with confidence-weighted scorecard. Classify and stage the opportunity. Define kill criteria.

2. **Product Extractor** (`prompts/product-extractor.md`)
   — Identify reusable modules, classify core/config/custom layers, assess architecture for productization.

3. **Enterprise Venture Analyst** (`prompts/venture-analyst.md`)
   — Validate market opportunity. Evaluate unit economics with evidence grading. Assess investment worthiness with risk-adjusted returns.

4. **Competitive Intelligence Analyst** (`prompts/competitive-intelligence-analyst.md`)
   — Research competitors, substitutes, potential entrants. Identify market gaps, moats, and winning strategies.

5. **Market Researcher** (`prompts/market-researcher.md`)
   — Size the market, validate demand, provide pricing benchmarks with source attribution.

## Quick Start

To analyze a project, tell your AI agent:

> Read AGENTS.md and skills/enterprise-product-innovation/SKILL.md.
> Then analyze [project name / document] using the full Innovation OS framework.
> Produce a complete Product Assessment using the template in templates/product-assessment.md.
> Include evidence grading on all key claims and explicit kill criteria.

## Tool-Specific Setup

### opencode (Codex)
Place this repo at `~/.config/opencode/skills/` or configure in `opencode.json`:
```json
{
  "skills": {
    "paths": ["/path/to/innovation-os/skills"]
  }
}
```

### Claude Code
Add to `~/.claude/skills/` or reference in `CLAUDE.md`:
```
Read: /path/to/innovation-os/AGENTS.md
Always use the Innovation OS framework when evaluating project proposals.
```

### Cursor
Create `.cursor/rules/enterprise-product-innovation.mdc` referencing the framework.

### Cline
Add to `.clinerules`:
```
Always use Innovation OS framework from /path/to/innovation-os/
```

### Gemini CLI / Aider / Other
Provide the AGENTS.md or SKILL.md as initial context in your prompt.

## Build Your Product Memory

After each analysis, save results as a case study in `case-studies/`.
This builds institutional knowledge that future AI agents can reference:
> "Have we seen this pattern before? What did we decide?"
