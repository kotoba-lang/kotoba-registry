# Registry maintenance

- Preserve the Hermes `index.json`, `SKILL.md` and MCP `manifest.json` formats.
- Generate `index.json` with `node scripts/build-index.mjs`; use `--check` before publishing.
- Preserve immutable upstream source references and verify snapshot digests.
- MCP entries declare connection configuration; credentials never belong here.
- Extension catalog publication is separate from Kotoba package admission and execution.
- Keep repositories under `github/<org>/<repo>`, worktrees under `github/wt/<agent>/<task>`, and scratch under `github/workspaces/<agent>/<task>`.
