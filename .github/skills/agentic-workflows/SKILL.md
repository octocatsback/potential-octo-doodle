---
name: agentic-workflows
description: Route gh-aw workflow design/create/debug/upgrade requests to the right prompts.
---

# Agentic Workflows Router

Use this skill when a user asks to design, create, update, debug, or upgrade GitHub Agentic Workflows in this repository.

This skill is a dispatcher: identify the task type, load the matching workflow prompt/skill file, and follow it directly. Keep responses concise and ask a clarifying question if the correct prompt is unclear.

The prompt files below live in the public `github/gh-aw` repository. Load them from there when they are not present locally.

After loading the matching workflow prompt or skill, follow it directly:

- Design workflows from scratch via interview: `skills/agentic-workflow-designer/SKILL.md`
- Create new workflows: `.github/aw/create-agentic-workflow.md`
- Update existing workflows: `.github/aw/update-agentic-workflow.md`
- Debug, audit, or investigate workflows: `.github/aw/debug-agentic-workflow.md`
- Upgrade workflows and fix deprecations: `.github/aw/upgrade-agentic-workflows.md`
- Create shared components or MCP wrappers: `.github/aw/create-shared-agentic-workflow.md`
- Create report-generating workflows: `.github/aw/report.md`
- Fix Dependabot manifest PRs: `.github/aw/dependabot.md`
- Analyze coverage workflows: `.github/aw/test-coverage.md`
- Choose workflow architecture and patterns: `.github/aw/patterns.md`

When creating or editing agentic workflow files in this repository, do not compile them. Only create or update the markdown workflow file unless the user explicitly asks to compile.
