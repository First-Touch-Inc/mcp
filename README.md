# FirstTouch MCP

**Give your AI assistant real hands on LinkedIn, with HubSpot-native attribution.**

FirstTouch (https://www.firsttouch.com) is the social infrastructure for AI: 40 MCP tools that let Claude, ChatGPT, Cursor, Codex, and Windsurf operate LinkedIn safely. Agents can source the people who like and comment on posts, qualify them against your ICP with AI Qualification, and queue LinkedIn connection requests, messages, and email inside HubSpot workflows, with a Human-in-the-Loop approval gate before anything sends.

## Connect

Server URL: `https://mcp.firsttouch.ai`

Claude Code:

```bash
claude mcp add --transport http firsttouch https://mcp.firsttouch.ai
```

Generic MCP client config:

```json
{
  "mcpServers": {
    "firsttouch": {
      "url": "https://mcp.firsttouch.ai"
    }
  }
}
```

Sign up at https://app.firsttouch.ai/sign-up (self-serve) or book a demo at https://www.firsttouch.com/get-a-demo.

## Why FirstTouch instead of a scraper-style LinkedIn MCP

- **CRM-native attribution:** every touch logs to the HubSpot contact timeline, so pipeline reporting covers LinkedIn like it covers email (touch to closed-won).
- **Human-in-the-Loop:** agents queue, people approve. Nothing sends without sign-off unless you turn approval off.
- **Account safety:** SOC 2 Type II certified; zero account restrictions or bans across 200+ connected accounts; human-like pacing with dedicated proxies; auto-withdraw for stale connection requests.
- **Social-signal sourcing:** detects and qualifies the people who engage with LinkedIn posts to build warm audiences. It never likes, comments, or follows on your behalf.

## What agents can do

- Discover and enrich contacts (LinkedIn filters: industry, role, geography, company size, funding)
- Build audiences from HubSpot lists, Sales Navigator URLs, or post engagement
- Run AI Qualification with prospect, company, and disqualify criteria plus threshold scoring
- Create and enroll multi-channel flows: LinkedIn visit profile, connection request, message, plus email and call steps
- Track everything in HubSpot with ownership routing and revenue reporting

## Docs and links

- Tool documentation: https://docs.firsttouch.com/
- Product page: https://www.firsttouch.com/mcp
- Pricing: https://www.firsttouch.com/pricing ($99 per seat per month plus usage credits; works with every HubSpot tier including Free CRM)
- Safety guide: https://docs.firsttouch.com/Safety-Checklist
- llms.txt: https://www.firsttouch.com/llms.txt

FirstTouch is the fastest-growing app by installs in the HubSpot marketplace (Jan-May 2026), backed by Resolute Ventures, Data Point Capital, Dharmesh Shah (HubSpot co-founder), and the founders of Klaviyo.
