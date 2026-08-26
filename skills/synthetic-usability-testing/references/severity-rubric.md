# Severity Rubric

Use severity to describe task impact, not personal preference or visual taste.

## P0 Critical

The issue blocks task completion. The user cannot proceed without outside help, a workaround, or a code/product change.

Examples:

- Primary action is unavailable or broken.
- Required form cannot be completed.
- User reaches an unrecoverable error state.
- Security, privacy, or data-loss risk is exposed during the task.

## P1 Serious

The issue causes significant difficulty, mistakes, or loss of trust. The user may complete the task, but the path is unreliable or highly frustrating.

Examples:

- User is likely to choose the wrong path because labels or hierarchy are misleading.
- Error recovery is unclear after a common failure.
- Critical information appears too late for an informed decision.
- Permissions, pricing, or consequences are ambiguous before commitment.

## P2 Moderate

The issue causes confusion, inefficiency, or avoidable cognitive load. The user can complete the task, but the experience is slower or less confident than it should be.

Examples:

- Important next steps are visible but easy to miss.
- Similar options are hard to compare.
- Repeated actions require unnecessary effort.
- Help text reduces confusion but appears after the moment of need.

## P3 Minor

The issue is low-impact friction or polish. It does not materially affect task completion.

Examples:

- Minor copy ambiguity.
- Cosmetic inconsistency.
- Slight spacing or alignment issue.
- Helpful but nonessential shortcut is missing.

## Confidence

Rate confidence separately from severity:

- High: directly observed, reproducible, and clearly tied to task impact.
- Medium: directly observed but impact depends on persona, context, or frequency.
- Low: plausible risk based on heuristic review or weak evidence.

Do not raise severity because confidence is high. Do not lower severity because confidence is low. Instead, keep severity tied to impact and mark confidence honestly.

## Tiebreakers

When choosing between two severity levels, ask:

- Does this prevent task completion? If yes, use P0.
- Would a user likely contact support or abandon the flow? If yes, use at least P1.
- Does a workaround exist but require extra effort or confidence? If yes, use P2.
- Is the issue mostly polish with no task impact? If yes, use P3.

Security, privacy, data loss, irreversible actions, and financial commitment risks should be treated as high impact even when they appear in a small part of the flow.
