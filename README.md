# FirstTouch MCP

Connect your AI assistant to your FirstTouch workspace to build audiences, create outreach flows, start selected contacts, track enrollment progress, and review tasks in natural language.

## Connect

Use the hosted FirstTouch MCP server:

```text
https://mcp.firsttouch.ai
```

The client opens a browser for FirstTouch sign-in and workspace approval. Authentication uses OAuth, so no API key needs to be pasted into the MCP configuration.

Generic MCP client configuration:

```json
{
  "mcpServers": {
    "firsttouch": {
      "type": "http",
      "url": "https://mcp.firsttouch.ai"
    }
  }
}
```

## What you can do

FirstTouch is the governed LinkedIn action layer for revenue teams and AI agents. Through this server your assistant can:

- Check the signed-in user, active workspace, team members, and assignment permissions.
- Find prospects with contact discovery and enrich contacts, companies, emails, and phone numbers.
- List HubSpot contact lists connected to the workspace and create audiences from them or from supplied contacts.
- Add contacts to an audience and attach an audience to a flow plan.
- List, inspect, and create outreach flow plans with LinkedIn, email, call, manual, wait, and branch actions.
- Queue LinkedIn connection requests, messages, and profile views for a single contact with Dynamic Actions.
- Read and reply in the team LinkedIn inbox, and monitor LinkedIn engagement signals.
- Review available flow variables and publish or unpublish a valid flow.
- Inspect awaiting contacts, start only the selected contacts, and follow enrollment progress.
- Review team metrics, credit usage, and tasks assigned to workspace members.

Human approval is on by default and is configured per action type, so a person reviews LinkedIn, email, and call actions before they go out unless your team turns approval off for that action type. Every touch is logged to the contact timeline in HubSpot when HubSpot is connected.

## Tools

The server exposes more than 60 tools across 12 capabilities: account and team, contact discovery, enrichment, audiences, flow plans, enrollments, dynamic actions, LinkedIn inbox, LinkedIn signals, outreach queue, tasks, and metrics. Call `get_auth_scopes` to see what the connected key or session may do, and `get_guide` for step-by-step guidance on flow creation, dynamic actions, and contact discovery. Full agent instructions are published at [docs.firsttouch.com/skill.md](https://docs.firsttouch.com/skill.md).

The same tool catalog is available as a REST API at `https://gateway.firsttouch.ai` with an `X-API-Key` header. See the [API reference](https://docs.firsttouch.com/api-reference/introduction).

## Example requests

- "Show my FirstTouch user, active workspace, and assignable team members."
- "Create a FirstTouch audience from my HubSpot list named Q3 Enterprise Leads."
- "Draft a flow that sends an intro email, waits one day, and creates a call task."
- "Show the awaiting contacts for this flow and enroll the first five."
- "List my FirstTouch tasks."

## Network access and data

The plugin connects to the FirstTouch-hosted MCP endpoint at `https://mcp.firsttouch.ai`. Browser-based authorization is handled by FirstTouch services.

FirstTouch accesses records from the workspace selected during authorization and respects that user's permissions. When a user explicitly requests a workflow involving a connected HubSpot account, FirstTouch may read the relevant HubSpot data. The plugin does not install or execute local code.

## Links

- [FirstTouch](https://www.firsttouch.com)
- [Documentation](https://docs.firsttouch.com)
- [Sign in](https://app.firsttouch.ai)

## License

Licensed under the [Apache License 2.0](LICENSE).
