# Persona Panel Template

Use this template when the user has not supplied personas. Select 2-4 personas based on the artifact and task. Do not invent demographic detail unless it changes the usability risk.

## General Product Panel

| Persona | Capability | What They Need | Synthetic Watchpoints |
|---|---:|---|---|
| First-time user | New to the product or category | Clear first action, plain language, reassurance | Jargon, unclear next steps, missing confirmation, weak help |
| Repeat user | Familiar with the task | Speed, memory, shortcuts, predictable paths | Slow repeated work, hidden frequent actions, inconsistent patterns |
| Accessibility-dependent user | Keyboard, screen reader, low vision, cognitive or motor needs | Semantic structure, focus order, visible focus, sufficient contrast | Click-only controls, unlabeled fields, color-only meaning, tiny targets |
| Edge-case tester | Pushes limits and recovery paths | Clear constraints, graceful errors, preserved work | Dead ends, lost input, silent failure, weak recovery |

## Developer Or Technical Tooling Panel

| Persona | Capability | What They Need | Synthetic Watchpoints |
|---|---:|---|---|
| Expert developer | High technical confidence | Speed, composability, scriptable paths | Hidden prerequisites, non-copyable examples, weak debugging, docs drift |
| New builder | Semi-technical or new to the stack | Guided setup, safe defaults, examples | Required advanced config, unexplained terms, dead-end errors |
| Platform admin | Governance owner | Permission clarity, auditability, rollback | Hidden permissions, unclear ownership, no review or rollback path |
| Downstream user | Affected by developer setup | Reliability, continuity, low friction | Broken handoffs, unclear consequences, missing status |

## Operational Agent Panel

| Persona | Capability | What They Need | Synthetic Watchpoints |
|---|---:|---|---|
| Admin | System owner | Control, safety, audit trail, cost visibility | Overbroad permissions, weak escalation, missing policy controls |
| Manager | Team operator | Outcome visibility, triage, exception handling | No status hierarchy, unclear handoff context, weak prioritization |
| Task performer | Front-line user | Continuity, trust, simple next steps | Surprise automation, unclear handoffs, too much operational detail |

## Custom Persona Format

```markdown
### [Persona Name]
- Capability band:
- Primary goal:
- Prior knowledge:
- Anxiety:
- Success signal:
- Likely failure mode:
- Accessibility or context needs:
```

## Selection Guidance

- Use the general panel for most product surfaces.
- Use the developer panel when the task involves building, deploying, debugging, APIs, CLI, docs, or technical setup.
- Use the operational agent panel when the surface governs agents, automation, handoffs, approval, escalation, operations, or cost.
- Add a first-time persona whenever onboarding, activation, setup, or first-run value is in scope.
- Add a repeat-user persona whenever efficiency, power use, or frequent task completion matters.
- Include the accessibility-dependent user whenever the artifact is visual or interactive.
