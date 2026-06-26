# Agent team

This project uses a four-agent team orchestrated via GitHub Copilot CLI in a Codespace:

- Planner — Claude Opus 4.7: researches the codebase and produces ordered implementation plans (.github/agents/planner.agent.md)
- Orchestrator — Claude Opus 4.7: breaks plans into phases, delegates and coordinates specialists (.github/agents/orchestrator.agent.md)
- Coder — GPT-5.5 (copilot): implements code, fixes bugs, and prepares runnable app support (.github/agents/coder.agent.md)
- Designer — Gemini 3.1 Pro (copilot): UI/UX, accessibility, interaction flow, and visual design (.github/agents/designer.agent.md)

Each agent file lives under .github/agents/ and is used by the Copilot CLI to run, delegate, and verify work.