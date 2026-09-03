# FirstTouch MCP

Connect your AI assistant to your FirstTouch workspace to build audiences, create outreach flows, start selected contacts, track enrollment progress, and review tasks in natural language.

## Connect

Use the hosted FirstTouch MCP server:

```text
https://mcp.firsttouch.com
```

The client opens a browser for FirstTouch sign-in and workspace approval. Authentication uses OAuth, so no API key needs to be pasted into the MCP configuration.

Generic MCP client configuration:

```json
{
  "mcpServers": {
    "firsttouch": {
      "type": "http",
      "url": "https://mcp.firsttouch.com"
    }
  }
}
```

## What you can do

- Check the signed-in user, active workspace, team members, and assignment permissions.
- List HubSpot contact lists connected to the workspace.
- Create audiences from supplied contacts or a connected HubSpot list.
- Add contacts to an audience and attach an audience to a flow plan.
- List, inspect, and create outreach flow plans with email, call, manual, wait, and branch actions.
- Review available flow variables and publish or unpublish a valid flow.
- Inspect awaiting contacts, start only the selected contacts, and follow enrollment progress.
- Review tasks assigned to workspace members.

Every email and call outreach action created through this connection requires human approval before execution.

## Example requests

- "Show my FirstTouch user, active workspace, and assignable team members."
- "Create a FirstTouch audience from my HubSpot list named Q3 Enterprise Leads."
- "Draft a flow that sends an intro email, waits one day, and creates a call task."
- "Show the awaiting contacts for this flow and enroll the first five."
- "List my FirstTouch tasks."

## Network access and data

The plugin connects to the FirstTouch-hosted MCP endpoint at `https://mcp.firsttouch.com`. Browser-based authorization is handled by FirstTouch services.

FirstTouch accesses records from the workspace selected during authorization and respects that user's permissions. When a user explicitly requests a workflow involving a connected HubSpot account, FirstTouch may read the relevant HubSpot data. The plugin does not install or execute local code.

## Links

- [FirstTouch](https://www.firsttouch.com)
- [Documentation](https://docs.firsttouch.com)
- [Sign in](https://app.firsttouch.ai)

## License

Licensed under the [Apache License 2.0](LICENSE).
