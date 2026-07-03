# Summit AI Notes MCP plugin

This repository is the marketplace for the official Summit AI Notes plugin. The plugin connects compatible AI clients to the local MCP server exposed by the Summit macOS app:

```text
http://127.0.0.1:8765/mcp
```

Meeting data remains on the Mac. The plugin does not configure a remote service or require API credentials. Summit AI Notes must be installed and running before the MCP connection can succeed.

## Codex

Add this repository as a marketplace, then install the `summit` plugin from it.

## Claude Code

Add this repository as a plugin marketplace, then install the `summit` plugin.

## MCP configuration

The plugin uses [`plugins/summit/.mcp.json`](./plugins/summit/.mcp.json):

```json
{
  "mcpServers": {
    "summit": {
      "type": "http",
      "url": "http://127.0.0.1:8765/mcp"
    }
  }
}
```

Learn more about Summit AI Notes at [summitnotes.app](https://summitnotes.app).
