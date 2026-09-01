# Smart Brevity

An [Agent Skill](https://agentskills.io/specification) that teaches AI coding agents to write and revise stakeholder-facing communications using the Axios Smart Brevity method: lead with the news, explain audience impact, prioritize scannable evidence, and state the decision or next step.

It is built for editorial judgment rather than mechanical shortening — the goal is the shortest *complete* communication, not the fewest words. The skill preserves qualifiers, uncertainty, warnings, and scope, and it explicitly declines to govern material where completeness must lead (contracts, filings, safety procedures, runbooks).

## What it covers

- **When to use the format** — and when to use it only as a summary layer over an authoritative source.
- **A communication contract** — audience, purpose, news, impact, support, next step, constraints — established before drafting.
- **A default information architecture** — title, lead, *Why it matters*, prioritized supporting blocks, action/decision, *Go deeper*.
- **Two workflows** — creating a new draft, and transforming an existing one via a preservation ledger so no decision-relevant detail is lost to compression.
- **Audience adaptation** — executives, project stakeholders, teams, customers, and incident audiences.
- **Accuracy guardrails** — never manufacture a metric, cause, deadline, owner, or consensus; keep denominators, calibrated language, and controlling legal or safety text intact.

## Installation

The skill itself lives in the `smart-brevity/` subdirectory — symlink that, not the repository root, so repository metadata stays out of your skills directory.

**Claude Code**

```bash
ln -s "$PWD/smart-brevity" ~/.claude/skills/smart-brevity
```

**Codex**

```bash
ln -s "$PWD/smart-brevity" ~/.codex/skills/smart-brevity
```

**Both at once** — Codex, Copilot CLI, and Gemini CLI all read the shared cross-runtime path:

```bash
ln -s "$PWD/smart-brevity" ~/.agents/skills/smart-brevity
```

Restart your agent session afterward so the skill is picked up.

## Usage

Agents load the skill on their own when a request matches its triggers — executive updates, project status, announcements, meeting recaps, customer notices, and incident updates. You can also invoke it by name:

```
/smart-brevity rewrite this status update for the exec team
```

By default the skill returns the polished communication itself, not an explanation of the method. Ask for commentary if you want the reasoning.

## Structure

```
smart-brevity-skill/               # This repository
├── README.md
└── smart-brevity/                 # The skill — symlink this directory
    ├── SKILL.md                   # Core method, workflows, and guardrails
    └── references/
        ├── review-checklist.md    # Pre-send audit, including an over-compression check
        ├── templates.md           # Working structures per communication type
        └── examples.md            # Before/after rewrites (original, fictional)
```

`SKILL.md` is the only file loaded on activation; the references are pulled in on demand.

## Compatibility

Conforms to the Agent Skills specification: `name` and `description` frontmatter only, `SKILL.md` under 500 lines, references one level deep. It contains no scripts, no `allowed-tools` declaration, and no harness-specific syntax, so it behaves identically across Claude Code, Codex, and other spec-compliant runtimes.

## Note

Smart Brevity is a method popularized by Axios. This skill is an independent implementation and is not affiliated with, endorsed by, or certified by Axios.
