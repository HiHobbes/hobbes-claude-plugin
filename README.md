# Hobbes for Claude

Hobbes helps B2B sales and go-to-market teams work with their AI product-demo agents from Claude. Inspect agent Playbooks and versions, review saved demo conversations and prospect engagement, and create personalized demo links. Preview agent updates before applying approved changes, and publish a specific version through the available confirmation flow.

## Connect

You need an existing Hobbes account. Add or connect the bundled Hobbes connector, then sign in to Hobbes and select your organization. Available tools depend on the permissions you grant. Agent changes and personalized link creation require an organization admin. Keep login credentials in the Hobbes sign-in flow.

In Claude, open Customize, then Connectors, choose Add, Custom, and Web. Name the connector Hobbes and enter `https://api.hihobbes.com/mcp`. Use the detected OAuth sign-in settings, sign in to Hobbes, and select the organization you want Claude to access. For agent inspection and updates, select only the additional Playbook, coaching, or publishing permissions you need. An organization's Claude administrator may need to enable the connector first.

You can also upload this plugin as a ZIP from Customize, Plugins, Add, Upload plugin. Open the installed plugin's Connectors tab to connect Hobbes. In Claude Code, install from the marketplace repository:

```text
/plugin marketplace add HiHobbes/hobbes-claude-plugin
/plugin install hobbes@hobbes
```

The remote MCP endpoint is https://api.hihobbes.com/mcp. The package contains workflow instructions and branding; it does not contain the server implementation or account credentials.

## Example requests

- How did our production demos perform last month?
- What objections did this prospect raise? Use the saved transcript.
- Show the Playbook and draft versus production versions for our named agent.
- Preview this Playbook change and show the exact before and after.
- Create one personalized demo link using the prospect details I provide.

Hobbes does not send outreach, change CRM records, or process payments through this connector. Treat recommendations, saved drafts, and successful production publication as separate outcomes.

## Help and data handling

- [Connection instructions](#connect)
- [Privacy policy](https://www.hihobbes.com/privacy-policy)
- [Terms of use](https://www.hihobbes.com/terms-of-use)
- Support: support@hihobbes.com

Claude receives the information returned by tools in the conversation. Anthropic's terms, your Claude plan, and your account settings govern Anthropic's handling of that information. Revoking a Hobbes connection stops future authorized access and does not remove information already returned to Claude. This differs from Hobbes's direct AI-provider API processing.

Package rights are reserved. Use of the Hobbes service is governed by its existing terms of use.
