# MCP Webflow Server Setup Guide

## Overview

This guide helps you set up the Webflow MCP (Model Context Protocol) server to enable AI agents to interact with your Webflow sites programmatically.

## Configuration File

The `mcp-servers.json` file contains your MCP server configuration:

```json
{
  "mcpServers": {
    "webflow": {
      "url": "https://mcp.webflow.com/sse"
    }
  }
}
```

## Prerequisites

1. **Webflow API Token**: You'll need to generate a Webflow API token from the [Webflow API Playground](https://developers.webflow.com/data/docs/ai-tools)

## Setup Instructions

### For Cursor Editor

1. Open Cursor Settings
2. Navigate to `Settings` → `Cursor Settings` → `MCP`
3. Click `+ Add New Global MCP Server`
4. Paste the configuration from `mcp-servers.json`
5. Save the settings
6. Cursor will open a browser window for Webflow site authorization

### For Claude Desktop

1. Open Claude Desktop Settings
2. Go to `Settings` → `Developer`
3. Click `Edit Config`
4. Open `claude_desktop_config.json` in a code editor
5. Add the configuration from `mcp-servers.json`
6. Save and restart Claude Desktop
7. Authorize Webflow sites when prompted

### For VS Code

1. Open VS Code settings
2. Edit `settings.json`
3. Add the configuration from `mcp-servers.json`
4. Save the file
5. Click the `start` button that appears over the "webflow" key
6. Complete the OAuth authorization flow

## Features Enabled

Once configured, you can:

- List and edit your site's CMS data
- Interact with Webflow APIs programmatically
- Manage site content through AI agents
- Automate content workflows

## Troubleshooting

If you encounter OAuth issues, reset your tokens:

```bash
rm -rf ~/.mcp-auth
```

Then restart your MCP client and re-authorize.

## Important Notes

- The `mcp-remote` npm package is experimental as of April 2025
- You'll need to authorize each Webflow site you want to access
- Keep your API tokens secure and don't commit them to version control

## Additional Resources

- [Webflow MCP Documentation](https://developers.webflow.com/data/docs/ai-tools)
- [Webflow API Playground](https://developers.webflow.com/data/docs/ai-tools)
- [MCP Protocol Specification](https://modelcontextprotocol.io/)