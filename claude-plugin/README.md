# FirstTouch for Claude

Connect Claude to FirstTouch through the hosted FirstTouch MCP server. Use it to build audiences, create and manage outreach flows, review enrollments, and work with assigned tasks. FirstTouch can use connected sources such as HubSpot and can support LinkedIn-related prospecting and outreach workflows, depending on the features and permissions enabled for your account.

## Connect

Install this plugin in Claude and connect your FirstTouch account when prompted. Authorization uses FirstTouch sign-in. The plugin points to `https://mcp.firsttouch.com` and does not require an API key or run local code.

The available actions depend on your account permissions, connected services, and FirstTouch settings. Some actions can create or change audiences, flows, enrollments, or outreach activity; review the requested action before approving it in Claude.

## Example requests

- "Show my FirstTouch account and team members."
- "Create an audience from my connected HubSpot list named New Leads."
- "Draft an outreach flow with an introductory email, a one-day wait, and a call task."
- "Show which contacts are waiting in this flow and start the first five."
- "List my assigned FirstTouch tasks."

## Data and support

Requests and relevant FirstTouch data used by this plugin are sent to the FirstTouch-hosted MCP endpoint. FirstTouch may access connected services when you request a workflow that uses them. See the [documentation](https://docs.firsttouch.com), [privacy policy](https://www.firsttouch.com/privacy-policy), and [contact page](https://www.firsttouch.com/contact) for more information.

## License

Licensed under the [Apache License 2.0](LICENSE).
