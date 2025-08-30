# Rostro's MCP Server

Turn any language model into a multimodal powerhouse that can generate images, music, videos and more on the fly. Rostro's tools are designed to be used by language models from the ground up, expanding capabilities with minimal context bloat.

## Quick Setup

**MCP Server URL:** `https://proto.rostro.dev/mcp`

## Quick Install Links

- **Cursor**: [Install in Cursor](https://cursor.com/en/install-mcp?name=Rostro&config=eyJ1cmwiOiJodHRwczovL3Byb3RvLnJvc3Ryby5kZXYvbWNwIiwiaGVhZGVycyI6e319)
- **LM Studio**: [Install in LM Studio](https://lmstudio.ai/install-mcp?name=rostro&config=eyJ1cmwiOiJodHRwczovL3Byb3RvLnJvc3Ryby5kZXYvbWNwIn0%3D)

## API Key Setup (Optional)

For fixed API authentication instead of OAuth, add this to your settings:

```json
"rostro": {
    "url": "https://proto.rostro.dev/mcp",
    "headers": {
        "Authorization": "Bearer <YOUR_API_KEY>"
    }
}
```

Get an API key from your [account page](https://rostro.dev/account).

## Client-Specific Setup

### Claude Desktop and Claude.ai

1. Go to [Claude Connectors](https://claude.ai/settings/connectors)
2. Click "Add Custom Connector"
3. Fill out the form:
   - Name: "Rostro"
   - URL: "https://proto.rostro.dev/mcp"
4. Click "Add"
5. Hit "Connect" and follow the OAuth flow
6. Optionally, click "Configure" to give Claude preapproval for individual tools

### Claude Code

Install using the command line:

```bash
claude mcp add rostro -t http https://proto.rostro.dev/mcp
```

Then start Claude and follow the instructions to complete authentication.

## What is MCP?

Model Context Protocol (MCP) is an open standard that allows language models to securely connect to third-party data sources and tools.

[Learn more about MCP](https://modelcontextprotocol.io/docs/getting-started/intro)
