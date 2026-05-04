# Skill Registry — lyrasis-site

_Generated: 2026-05-04 | Project: lyrasis-site_

## Active Skills

| Skill | Trigger | Source |
|-------|---------|--------|
| branch-pr | When creating a pull request, opening a PR, or preparing changes for review | user (~/.claude/skills/) |
| gentle-ai-chained-pr | When a PR would exceed 400 changed lines, or planning chained/stacked PRs | user (~/.config/opencode/skills/) |
| cognitive-doc-design | When writing guides, READMEs, RFCs, onboarding docs, architecture docs, or review-facing documentation | user (~/.claude/skills/) |
| comment-writer | When drafting or posting feedback, review comments, maintainer replies, Slack messages, or GitHub comments | user (~/.claude/skills/) |
| issue-creation | When creating a GitHub issue, reporting a bug, or requesting a feature | user (~/.claude/skills/) |
| judgment-day | When user says "judgment day", "dual review", "doble review", "juzgar", "que lo juzguen" | user (~/.claude/skills/) |
| landing-page-design | landing page, hero section, conversion optimization, CTA button, SaaS landing page | user (~/.claude/skills/) |
| work-unit-commits | When implementing a change, preparing commits, splitting PRs, or planning chained PRs | user (~/.claude/skills/) |
| skill-creator | When user asks to create a new skill, add agent instructions, or document patterns for AI | user (~/.claude/skills/) |

## SDD Skills (loaded by orchestrator — not directly invoked)

| Skill | Phase |
|-------|-------|
| sdd-explore | Exploration/investigation |
| sdd-propose | Change proposal |
| sdd-spec | Specifications |
| sdd-design | Technical design |
| sdd-tasks | Task breakdown |
| sdd-apply | Implementation |
| sdd-verify | Verification |
| sdd-archive | Archive/close |

## Project Convention Files

_No AGENTS.md, CLAUDE.md, or .cursorrules found in project root._

## Notes

- No test suite in this project — `go-testing` skill not applicable
- Static Jekyll site — no backend framework skills needed
- Ruby/Jekyll stack: no JS/TS, no Go, no Python
