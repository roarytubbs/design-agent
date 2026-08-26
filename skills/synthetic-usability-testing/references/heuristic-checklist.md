# Heuristic And Cognitive-Load Checklist

Use this checklist during the Scenario pass. The goal is to expose likely usability risks, not to produce a decorative score.

## Nielsen Heuristics

Mark each heuristic as Pass, Risk, or Fail.

### 1. Visibility of system status

Users should know what is happening.

Check for loading states, save confirmation, progress indicators, current location, and validation feedback.

### 2. Match to user language and mental model

The interface should speak in terms the target user understands.

Check for plain language, familiar terminology, recognizable icons, natural reading order, and domain terms that are explained when needed.

### 3. User control and reversibility

Users need exits from unwanted states.

Check for undo, cancel, back, clear filters, escape from modals, and recovery from multi-step flows.

### 4. Consistency and standards

Similar words, states, and actions should behave consistently.

Check terminology, interaction patterns, visual treatment, platform conventions, and repeated components.

### 5. Error prevention

The design should prevent likely mistakes before they happen.

Check destructive-action safeguards, constraints, validation, smart defaults, autosave, and review steps for high-impact actions.

### 6. Recognition over recall

Users should not need to remember hidden paths or prior information.

Check visible options, labels on icons, contextual help, recent items, autocomplete, and preserved context between steps.

### 7. Efficiency for repeat users

Frequent users need faster paths.

Check keyboard support, shortcuts, bulk actions, saved preferences, recent items, and advanced options that do not complicate first-run use.

### 8. Minimalism and hierarchy

Every visible element should have a job.

Check visual hierarchy, competing calls to action, decorative noise, overlong copy, dense option sets, and whether the primary path is obvious.

### 9. Error recovery

Errors should be specific, plain-language, and actionable.

Check whether messages explain what happened, what it means, how to recover, and whether user work is preserved.

### 10. Help and documentation

Help should be easy to find, task-focused, and close to the moment of need.

Check inline guidance, tooltips, examples, docs links, support paths, and whether help content matches the real workflow.

## Cognitive Load

Count failures against these checks:

- Single focus: the primary task is not competing with unrelated elements.
- Chunking: information is grouped into small, digestible sets.
- Grouping: related controls and content are visually connected.
- Visual hierarchy: the next important action is obvious.
- One thing at a time: the user can make one decision before the next.
- Minimal choices: decision points avoid unnecessary option overload.
- Working memory: the user does not need to remember key information from earlier screens.
- Progressive disclosure: complexity appears when needed, not all at once.

Classify load:

- Low: 0-1 failed checks.
- Moderate: 2-3 failed checks.
- High: 4 or more failed checks.

## Output Notes

- Name the specific element, step, command, or section causing the risk.
- Prioritize task completion, confidence, recovery, and trust.
- Do not inflate issues that are only visual preference.
- If a heuristic cannot be assessed from the artifact, mark it as not inspected instead of guessing.
