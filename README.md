# Agentic GitHub Copilot Skills & Impersonation Framework

A collection of GitHub Copilot agent skills that pair recognizable personas
with practical, technically grounded engineering guidance.

[![CI](https://github.com/jry25/copilot-impersonation-skills/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/jry25/copilot-impersonation-skills/actions/workflows/ci.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Pollen](https://img.shields.io/badge/distribution-Pollen-inspired-5b8c5a)](https://groupbees.github.io/pollen/)

## Quickstart

1. Make this repository available to your coding agent by opening it in a
   supported IDE or using it as the repository context for a GitHub Copilot
   cloud agent.
2. Keep the skill under `.github/skills/<skill-name>/SKILL.md` in the
   repository where you want Copilot to discover it. To reuse a skill, copy
   its directory into that location.
3. Ask Copilot to review a diff or pull request with the skill name, for
   example: “Review this diff using the `trumppullreview` skill.”

Skills provide instructions and context to an agent; they do not install
software or guarantee that every Copilot client supports custom skills. Check
your client’s current documentation for skill discovery and enablement details.

## Skills

- [`trumppullreview`](.github/skills/trumppullreview/SKILL.md) — a technically
  grounded code review in a dramatic, Truth Social-inspired rhetorical style.

## Framework references

- [Pollen](https://groupbees.github.io/pollen/) — distribution concepts that
  inform how skills can be packaged and shared.
- [Awesome Copilot Skills](https://awesome-copilot.github.com/skills/) —
  community examples and patterns for agent skills.

See [the architecture overview](docs/architecture.md) and
[skills manifest](docs/skills-manifest.md) for implementation details and
contribution guidance.
