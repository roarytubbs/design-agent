# Design Agent Manifest

## Included Skills

### synthetic-usability-testing

Purpose: AI-assisted usability preflight using artifact inspection, task scenarios, persona simulation, heuristic checks, severity and confidence scoring, independent verification, and a human validation plan.

Package shape:

```text
synthetic-usability-testing/
|-- SKILL.md
`-- references/
    |-- heuristic-checklist.md
    |-- human-validation-plan.md
    |-- persona-panel-template.md
    |-- report-template.md
    `-- severity-rubric.md
```

## What Was Converged

This repo consolidates the strongest portable pieces from the local usability research skills bundle:

- The broader synthetic testing workflow from `synthetic-usability-testing`.
- Persona panel defaults from the bundle, generalized for public use.
- Heuristic and cognitive-load checks from the critique workflow.
- Human validation planning from the research execution workflow.
- Report sections for scenario results, persona red flags, heuristic checks, instrumentation, and verifier review.

## What Was Not Pulled In

- HubSpot-specific research sources, personas, file paths, and MCP tools.
- Deterministic visual detector commands that depend on private local tooling.
- Full `research-trends`, `research-execution`, `critique`, and `ux-designer` skills. Those can become separate public skills later if they are generalized first.
