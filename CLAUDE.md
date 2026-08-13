# OpenHands Agent Instructions

Read and follow [`AGENTS.md`](AGENTS.md) before changing this repository.

For this machine's managed OpenHands deployment:

- Keep secrets in Windows User environment variables. Never commit API keys, bearer tokens, or generated Canvas credentials.
- Use `agentcore-gateway` as the only MCP entry. Do not add raw SwarmRecall, SwarmVault, SQL, or duplicate memory MCP servers.
- Keep OpenHands native persistent memory disabled; durable project memory flows through AgentCore.
- Treat `.openhands/` and `.cursor/` as local runtime state, not source-controlled application code.
- Use a task branch or isolated worktree for implementation. Verify tests and review the diff before merging.
- Do not claim a feature is enabled from configuration alone; prove the live model, MCP, skill, and runtime paths.
