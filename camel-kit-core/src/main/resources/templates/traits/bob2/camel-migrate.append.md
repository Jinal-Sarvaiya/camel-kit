## Agent Optimization: IBM Bob 2

For chained and standalone migration (design-only), switch to `camel-brainstorm-mode` before migration
discovery and design. Use `explore` subagents only for self-contained source analysis; keep the interview,
design decisions, and approval gate in the parent task.

For direct mode (`--direct` or auto-detected), switch to `camel-execute-mode` before starting. Direct mode
implements route files and support artifacts, runs validation, ACR, and the application — these require
implementation-capable edit permissions and worker subagents that `camel-brainstorm-mode` does not permit.

For a pipeline knowledge lookup, load `.bob/personas/knowledge-researcher.md` and spawn `camel-reviewer` with that complete role and query.
