# Design Agent

Open agent skills for design workflows.

`design-agent` is a home for reusable skills that help designers, researchers, and product teams use agents in practical design work. The focus is on workflows where agents can inspect artifacts, reason through user tasks, generate useful reports, and help teams decide what to improve or validate next.

The repo starts with synthetic usability testing, but the intent is broader: design critique, research planning, design-system checks, AI-assisted review workflows, and other repeatable tools for technical designers.

## Principles

- Make agent work useful to designers, not just impressive in isolation.
- Treat synthetic outputs as directional signal, not proof of real user behavior.
- Keep skills portable and public, without private company-specific assumptions.
- Prefer concrete artifacts: reports, rubrics, templates, recommendations, and validation plans.
- Preserve human judgment. Agents should help teams see risks earlier, not replace research or design decision-making.

## Skills

### `synthetic-usability-testing`

Runs a structured synthetic usability test against URLs, prototypes, Figma files, screenshots, docs, CLI/API workflows, and other interface artifacts.

The skill inspects the artifact, creates task scenarios, evaluates them through usability and persona lenses, writes a severity-rated report, and verifies its own findings before final output.

Canonical skill docs live in [SKILL.md](skills/synthetic-usability-testing/SKILL.md). The supporting rubrics and templates live in that skill's `references/` folder.

## Roadmap

Potential future skills:

- Design critique and heuristic review.
- Research planning from synthetic findings.
- Design-system drift and token checks.
- Accessibility preflight for design artifacts.
- AI-assisted content and UX copy review.
- Publication workflows for essays, case studies, and open-source project writeups.

## Install

Install any skill by copying its folder into a supported skills directory. For example:

```bash
mkdir -p ~/.codex/skills
cp -R skills/synthetic-usability-testing ~/.codex/skills/
```

Project-local installs work the same way:

```bash
mkdir -p .codex/skills
cp -R skills/synthetic-usability-testing .codex/skills/
```

Each installable skill should remain self-contained under `skills/<skill-name>/`.

## Related Work

This project is maintained by [Roary Tubbs](https://roarytubbs.com). Future design-agent skills and related open-source design tooling will be linked from this repo.

## License

MIT
