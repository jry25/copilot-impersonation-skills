# Architecture

This repository treats each Copilot skill as a self-contained, portable
instruction package: a directory beneath `.github/skills/` containing a
`SKILL.md` file with YAML frontmatter and agent instructions.

## Distribution and community patterns

[Pollen](https://groupbees.github.io/pollen/) informs the repository's
packaging and distribution approach: keep each skill in a discoverable,
reusable unit that can be shared or copied into another project. This
repository does not depend on or execute Pollen; Pollen is a conceptual
reference for organizing and distributing the skill collection.

[Awesome Copilot Skills](https://awesome-copilot.github.com/skills/) provides
community examples and patterns for authoring agent skills. Skills in this
repository follow the same general idea of pairing a concise metadata
description with focused instructions, while adding persona-driven
presentation where useful.

## Agent execution model

When a compatible Copilot client has access to this repository, it can use
the skill metadata to identify a relevant skill and provide the skill's
instructions as context for a task. For example, `trumppullreview` guides a
code-review task toward a distinct rhetorical voice while requiring
technically valid, actionable findings. The skill is instructional content,
not executable code, and client discovery behavior may vary.

## Compliance verification

The GitHub Actions workflow in `.github/workflows/ci.yml` checks Markdown
formatting, parses repository JSON and YAML files, and validates that each
skill has YAML frontmatter with non-empty `name` and `description` values.
These static checks catch structural errors; they do not prove that a skill's
advice is correct or that all clients will follow it. Human review remains
necessary for technical accuracy, safety, and compatibility.
