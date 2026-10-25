---
name: scutum
description: >-
  Scutum Spec-Driven Development (SDD) framework and AI governance workflows.
  Use this skill whenever the user invokes any /scutum command (such as /scutum.specify,
  /scutum.plan, /scutum.tasks, /scutum.implement, /scutum.constitution, /scutum.test,
  /scutum.converge, /scutum.scutum, etc.) or requests to execute Scutum workflows.
---

# Scutum SDD Governance Skill

This skill guides the agent through executing Scutum Spec-Driven Development workflows within Antigravity IDE.

## Available Commands

All command definitions reside in `.agents/commands/`:

- `/scutum.scutum` (`.agents/commands/scutum.scutum.md`): Concierge & router entrypoint
- `/scutum.constitution` (`.agents/commands/scutum.constitution.md`): Establish or amend project constitution
- `/scutum.specify` (`.agents/commands/scutum.specify.md`): Requirements specification (`spec.md`)
- `/scutum.clarify` (`.agents/commands/scutum.clarify.md`): Requirements clarification
- `/scutum.checklist` (`.agents/commands/scutum.checklist.md`): Quality and review checklists
- `/scutum.plan` (`.agents/commands/scutum.plan.md`): Technical architecture & implementation plan (`plan.md`)
- `/scutum.tasks` (`.agents/commands/scutum.tasks.md`): Actionable task decomposition (`tasks.md`)
- `/scutum.implement` (`.agents/commands/scutum.implement.md`): Phased code implementation
- `/scutum.converge` (`.agents/commands/scutum.converge.md`): Verify implementation completeness
- `/scutum.test` (`.agents/commands/scutum.test.md`): Comprehensive test suite execution
- `/scutum.analyze` (`.agents/commands/scutum.analyze.md`): Structural analysis & health check
- `/scutum.redesign` (`.agents/commands/scutum.redesign.md`): Rework an isolated UI component or endpoint
- `/scutum.revamp` (`.agents/commands/scutum.revamp.md`): Cross-module phased revamp
- `/scutum.upgrade` (`.agents/commands/scutum.upgrade.md`): Dependency & framework version upgrade
- `/scutum.tracer` (`.agents/commands/scutum.tracer.md`): Issue/root-cause tracing
- `/scutum.prototype` (`.agents/commands/scutum.prototype.md`): Lightweight throwaway PoC
- `/scutum.deploy` (`.agents/commands/scutum.deploy.md`): Containerization & deployment pipeline setup
- `/scutum.operate` (`.agents/commands/scutum.operate.md`): Production telemetry & observability
- `/scutum.postmortem` (`.agents/commands/scutum.postmortem.md`): Incident post-mortem & learnings
- `/scutum.brd` (`.agents/commands/scutum.brd.md`): Business Requirements Document for existing code

## Execution Protocol

1. Read the matching command file from `.agents/commands/scutum.<command>.md`.
2. Inspect prerequisite artifacts and context in `.scutum/memory/constitution.md` and feature directories.
3. Follow the phase gates, templates (`.scutum/templates/`), and rules described in the command file.
