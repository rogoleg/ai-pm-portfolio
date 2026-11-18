# Prompt Library

Versioned prompts for AI features. Each prompt lives in its own file and contains:

- **Intent** — the user job it serves
- **Constraints** — latency, cost, tone, refusal and safety rules
- **Known failure modes** — what breaks it in practice
- **Changelog** — what changed and why

Naming: `feature-name-vN.md`

Rules:

1. Never edit a shipped prompt in place — bump the version.
2. Every change needs an eval run before it ships (see `../eval-harness/`).
3. Keep the system prompt and the user template in the same file so diffs stay honest.
