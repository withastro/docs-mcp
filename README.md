### Cursor

Install automatically: [![Install MCP Server](https://cursor.com/deeplink/mcp-install-dark.svg)](cursor://anysphere.cursor-deeplink/mcp/install?name=Astro%20docs&config=eyJ1cmwiOiJodHRwczovL21jcC5kb2NzLmFzdHJvLmJ1aWxkL21jcCJ9)

[More info on MCP in Cursor](https://docs.cursor.com/context/mcp)

### Claude.ai / Claude Desktop

- Visit [Claude.ai connector settings](https://claude.ai/settings/connectors)
- Scroll down and click "Add custom connector"
- Enter the following details:
  - **Name**: Astro Docs
  - **Remote MCP server URL**: https://mcp.docs.astro.build/mcp

[More info on MCP in Claude.ai](https://support.anthropic.com/en/articles/10168395-setting-up-integrations-on-claude-ai#h_cda40ecb32)

### Claude Code

```sh
claude mcp add --transport http "Astro docs" https://mcp.docs.astro.build/mcp
```

[More info on MCP in Claude Code](https://docs.anthropic.com/en/docs/claude-code/mcp)

### VS Code

Install automatically: [Install](vscode:mcp/install?%7B%22name%22%3A%22Astro%20docs%22%2C%22url%22%3A%22https%3A%2F%2Fmcp.docs.astro.build%2Fmcp%22%7D)

[More info on MCP in VS Code](https://code.visualstudio.com/docs/copilot/chat/mcp-servers#_add-an-mcp-server)

### Windsurf

As of July 2025, Windsurf doesn't support streamable HTTP MCP servers, so you need to use a local proxy. Use the following configuration:

```json
{
  "mcpServers": {
    "Astro docs": {
      "command": "npx",
      "args": ["-y", "mcp-remote", "https://mcp.docs.astro.build/mcp"]
    }
  }
}
```

[More info on MCP in Windsurf](https://docs.windsurf.com/windsurf/cascade/mcp#mcp-config-json)
