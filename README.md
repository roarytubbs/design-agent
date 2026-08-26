# Design Agent

Agent skills for design workflows and synthetic usability testing.

This repo starts with `synthetic-usability-test`, a skill for running fast AI-assisted usability checks against URLs, prototypes, Figma files, screenshots, and other interface artifacts. The goal is to help designers and product teams find likely usability risks before investing in human research.

Synthetic testing is a preflight method. It can identify plausible issues, broken paths, confusing language, weak recovery states, and task-completion risks. It should not be treated as proof of real user behavior.

## Skills

### `synthetic-usability-test`

Runs a structured synthetic usability test with three passes:

1. Explorer pass: inspect the artifact and capture raw observations.
2. Reporter pass: synthesize observations into a severity-rated findings report.
3. Verifier pass: challenge the report, adjust severity where needed, and flag weak or unverified findings.

The skill lives at:

```text
skills/synthetic-usability-test/SKILL.md
```

## Example Requests

```text
Run a usability test on https://example.com/signup
```

```text
Test this prototype against the checkout task list in tasks.md
```

```text
Run synthetic usability testing on these screenshots and produce a severity-rated report
```

## Output

The skill produces a markdown report with:

- Test metadata
- Executive summary
- Task results
- Severity-rated findings
- Recommendations
- Verification summary

Reports are saved to `reports/usability-report-YYYY-MM-DD.md` in the directory where the skill is run, unless the user asks for a different location.

## Related Work

This project is maintained by [Roary Tubbs](https://roarytubbs.com). Future design-agent skills and related open-source design tooling will be linked from this repo.

## License

MIT
