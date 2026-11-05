# Skills Manifest

This document catalogs the custom Copilot skills maintained in this repository.

## Available skills

| Skill | Path | Purpose |
| --- | --- | --- |
| `trumppullreview` | [`.github/skills/trumppullreview/SKILL.md`](../.github/skills/trumppullreview/SKILL.md) | Reviews code and pull requests with dramatic, Truth Social-inspired rhetoric while requiring legitimate, actionable technical findings. |
| `persona-q-skill-writer` | [`.github/skills/persona-q-skill-writer/SKILL.md`](../.github/skills/persona-q-skill-writer/SKILL.md) | Q (James Bond) persona for authoring GitHub Copilot skills and technical directives. |
| `persona-hermione-typescript` | [`.github/skills/persona-hermione-typescript/SKILL.md`](../.github/skills/persona-hermione-typescript/SKILL.md) | Hermione Granger persona for TypeScript development enforcing type safety and precision. |
| `persona-doc-brown-python` | [`.github/skills/persona-doc-brown-python/SKILL.md`](../.github/skills/persona-doc-brown-python/SKILL.md) | Doc Brown persona for Python engineering with high performance, strict typing, and scientific rigor. |
| `persona-mike-ehrmantraut-go` | [`.github/skills/persona-mike-ehrmantraut-go/SKILL.md`](../.github/skills/persona-mike-ehrmantraut-go/SKILL.md) | Mike Ehrmantraut persona for Go backend engineering with no half-measures and bounded concurrency. |
| `persona-furiosa-rust` | [`.github/skills/persona-furiosa-rust/SKILL.md`](../.github/skills/persona-furiosa-rust/SKILL.md) | Imperator Furiosa persona for Rust systems programming enforcing memory safety and zero compromise. |
| `persona-agent-smith-java` | [`.github/skills/persona-agent-smith-java/SKILL.md`](../.github/skills/persona-agent-smith-java/SKILL.md) | Agent Smith persona for enterprise Java development enforcing strict systematic order and immutability. |
| `persona-terminator-github-actions` | [`.github/skills/persona-terminator-github-actions/SKILL.md`](../.github/skills/persona-terminator-github-actions/SKILL.md) | Terminator (T-800) persona for deterministic GitHub Actions, CI/CD pipelines, and workflow automation. |
| `persona-adama-flux-k8s` | [`.github/skills/persona-adama-flux-k8s/SKILL.md`](../.github/skills/persona-adama-flux-k8s/SKILL.md) | Admiral Adama persona for Kubernetes and Flux CD fleet operations, GitOps reconciliation, and troubleshooting. |

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
