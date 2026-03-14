# Multi-Agent Example App

## Agentic flows

a) Planner -> Implementer -> Tester -> Reviewer -> Documenter

b) Assigner -> Planner -> Implementer -> Tester -> Reviewer -> Documenter -> Pusher

- Assigner (get requirements from task such as JIRA or Notion)
- Pusher (push as feature commit or PR to code repo such as GitHub or BitBucket)

## Workflow
1. Generate instruction file for the repo: ```.github/copilot-instructions.md ```
2. Create agents folder: ```.github/agents/```
3. Define agents and subagents
4. Define optional files such as skills, etc.
5. Work on integrations via MCP servers setup (e.g., JIRA, etc.)

