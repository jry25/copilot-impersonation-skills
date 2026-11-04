# Skills Manifest

This document catalogs the custom Copilot skills maintained in this repository.

## Available skills

| Skill | Path | Purpose |
| --- | --- | --- |
| `trumppullreview` | [`.github/skills/trumppullreview/SKILL.md`](../.github/skills/trumppullreview/SKILL.md) | Reviews code and pull requests with dramatic, Truth Social-inspired rhetoric while requiring legitimate, actionable technical findings. |

## Adding a skill

1. Create `.github/skills/<skill-name>/SKILL.md`.
2. Add YAML frontmatter at the start of the file with non-empty `name` and
   `description` fields. Use a short, lowercase name that matches the
   directory.
3. Write focused instructions describing when the skill applies, how the
   agent should perform the task, and the expected output.
4. For persona-driven skills, keep the persona separate from technical
   requirements. Never let a style constraint weaken correctness, safety, or
   clarity.
5. Add the skill to the table above and mention it in the README when
   appropriate.
6. Run the repository checks and request human review before sharing the skill.

The CI workflow verifies Markdown formatting and basic skill metadata.
Authors remain responsible for reviewing a skill's content, technical
claims, and compatibility with their Copilot client.
