# Multi-Agent Example App

## Agentic flows

a) Planner -> Implementer -> Tester -> Reviewer -> Documenter

b) Intake -> Planner -> Implementer -> Tester -> Reviewer -> Documenter -> Submitter

## Agents
- Intake: get requirements from task such as JIRA or Notion
- Planner
- Implementer
- Tester
- Reviewer
- Documenter
- Submitter: push as feature commit or PR to code repo such as GitHub or BitBucket
- Security
- Debugger
- Analyst 

## Workflow
1. Generate instruction file for the repo: ```.github/copilot-instructions.md ```
2. Create agents folder: ```.github/agents/```
3. Define agents and subagents
4. Define optional files such as skills, etc.
5. Work on integrations via MCP servers setup (e.g., JIRA, etc.)

## Additional Agents
- Background agent: Select ```Background``` in a new chat window, then select the custom agent to run in the background for that chat session (e.g., debugger, security, analyst)
- Parallel subagents: Type in chat ```Run subagents to do something... ```, which will run in parallel then bring the results back to the main chat session, without clouding the main thread. More in the VSCode tutorial http://code.visualstudio.com/blogs/2026/02/05/multi-agent-development


## Integrations
Adding integrations with agents via MCP servers
https://code.visualstudio.com/docs/copilot/customization/mcp-servers

### Integration Steps
1. Set up MCP integration in VSCode for GitHub CoPilot
- 1a. Auto: Search for extension in VS Code's Extensions: ```@mcp PLUGINNAME```
- 1b. Manual: Configure the settings for an integration's MCP docs (e.g., Notion MCP server: https://github.com/makenotion/notion-mcp-server?tab=readme-ov-file)

2. Go through the integration steps within the integration provider's platform (e.g., Notion -> Internal Integrations via notion.so/profile/integrations)

### Integration Resources
- Notion MCP Server: https://github.com/makenotion/notion-mcp-server?tab=readme-ov-file


## Useful Chat Commands
- load workspace context: ```@workspace```
- load context file: ```#FILENAME```
- load context folder: select paperclip in chat window