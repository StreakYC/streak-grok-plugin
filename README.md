# Streak CRM plugin

Connect Cursor and Grok Bot to [Streak](https://www.streak.com), the CRM built into Gmail.

## What it does

Search and manage pipelines, deals (boxes), contacts, organizations, tasks, and timeline activity through Streak's hosted MCP server.

## Connect

1. Add the Streak plugin in your client's plugin settings or marketplace when available.
2. Complete the Streak sign-in and authorization flow.
3. Ask about your CRM, for example: "Summarize my sales pipeline" or "Find deals that need follow-up."

A Streak account on Pro, Pro+, or Enterprise is required. Each person signs in to their own account. Access follows their Streak permissions. The connector can read and change CRM data.

## Configuration

The MCP endpoint is `https://api.streak.com/mcp`. It uses HTTP and OAuth. No API key or local server is needed. This package contains no credentials, executable scripts, or copy of the Streak backend.

[Connection help](https://support.streak.com/en/articles/13931874-connect-streak-to-ai-tools-via-mcp)

## Development

This package uses the Cursor Plugin format. The manifest is `.cursor-plugin/plugin.json`; the server configuration is `mcp.json`.

For a local check, copy this directory into `~/.cursor/plugins/local/streak`, reload Cursor, and find Streak in Customize. Authenticate, confirm tools appear, and try a read such as listing pipelines. Test writes only against records created for testing.

## License

The configuration and documentation are MIT licensed. The Streak logo and name remain Streak trademarks; the software license does not grant trademark rights. Use of the hosted Streak service remains subject to its terms.
