# FirstTouch MCP: LinkedIn for AI agents

Give Claude, ChatGPT, Gemini, Cursor, Codex or any MCP client the ability to run LinkedIn outreach for your team: find and enrich prospects, send connection requests and messages, work the LinkedIn inbox, watch who engages with your posts, and sync it all to HubSpot. Every outreach action can require human approval before it goes out.

FirstTouch is used by 300+ revenue teams. HubSpot is optional.

## Connect

Hosted server, OAuth sign-in, no API key to paste:

```text
https://mcp.firsttouch.com
```

**Claude (claude.ai or desktop):** Settings, Connectors, Add custom connector, paste the URL above, then sign in to FirstTouch.

**Claude Code:**

```bash
claude mcp add --transport http firsttouch https://mcp.firsttouch.com
```

**ChatGPT:** FirstTouch is listed in ChatGPT's plugin directory. Install the [FirstTouch plugin](https://chatgpt.com/plugins/plugin_asdk_app_6a8c88cc224c8191ab9759b9cd6a5276), then sign in to FirstTouch. No URL or developer mode needed.

**Cursor, Windsurf, Codex, Gemini and other MCP clients:**

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

Full setup guide: https://docs.firsttouch.com/WebApp/Mcp/connect

## What your agent can do

- **LinkedIn outreach:** send connection requests and messages for a contact or a whole audience, as one-off actions or multi-step flows.
- **Approvals:** outreach actions are approval-required by default and configurable by action type. Approvals show up in FirstTouch, and as Slack messages once Slack is connected.
- **LinkedIn inbox:** read and reply to conversations across your team's connected LinkedIn accounts.
- **Engagement signals:** monitor LinkedIn profiles and company pages and pull the people who like and comment.
- **Prospecting and enrichment:** discover contacts, enrich profiles, find emails and phone numbers.
- **HubSpot:** build audiences from HubSpot lists and log completed LinkedIn activity to the contact timeline when engagement tracking is enabled.
- **Team view:** team members, credits, outreach queue and metrics.

60+ tools in total.

## Example requests

- "Find VPs of Sales at Series B SaaS companies in New York and draft a connection request for each. Hold them for my approval."
- "Send a LinkedIn connection request to everyone on my HubSpot list Q4 Enterprise Leads."
- "Who liked or commented on our CEO's last three LinkedIn posts? Draft a follow-up for the ones that match our ICP."
- "Show my unread LinkedIn conversations and draft replies."
- "How many connection requests did each rep send this week, and how many were accepted?"

## Pricing

$99 per connected LinkedIn account (sender) per month, with a 14-day free trial and no credit card required. Sending connection requests and messages uses no credits. https://www.firsttouch.com/pricing

## Network access and data

The connector talks only to the FirstTouch-hosted endpoint. Sign-in uses OAuth through FirstTouch. Each user acts within the workspace they authorize and with their own permissions. FirstTouch reads HubSpot data only when a user asks for a workflow that needs it. Nothing is installed or run locally.

## Links

- [FirstTouch for AI agents](https://www.firsttouch.com/mcp)
- [Documentation](https://docs.firsttouch.com)
- [API reference](https://docs.firsttouch.com/api-reference/introduction)
- [Sign up](https://app.firsttouch.ai)

## License

Apache License 2.0. See [LICENSE](LICENSE).
