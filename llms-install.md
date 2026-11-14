# Install Station

Station is a hosted MCP server. There is nothing to clone, build or run.

Add this server to the MCP settings:

```json
{
  "mcpServers": {
    "station": {
      "type": "streamableHttp",
      "url": "https://rooms.station.site/mcp",
      "disabled": false,
      "autoApprove": []
    }
  }
}
```

No API key or header is needed. The first tool call opens a browser to sign in to Station with OAuth. In Cline's CLI, `cline mcp` has "Authorize OAuth" to sign in again.

Check it worked: call `rooms_list`. It lists the person's Station rooms.
