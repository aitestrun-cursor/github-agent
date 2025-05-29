# Getting Started with MCP

## What is Model Context Protocol?

Model Context Protocol (MCP) is a powerful communication standard that enables AI models to interact with external tools and services in a structured, predictable way. It serves as the foundation for AI-powered development tools and assistants.

## Quick Start

### 1. Installation

```bash
# Install the Smithery CLI globally
npm install -g @smithery/cli

# Install specific MCP servers you need
npm install @smithery-ai/github
```

### 2. Basic Configuration

Create a configuration file named `mcp.json` in your project root:

```json
{
  "mcpServers": {
    "github": {
      "command": "npx",
      "args": [
        "@smithery/cli",
        "run",
        "@smithery-ai/github",
        "--key",
        "YOUR_GITHUB_TOKEN",
        "--profile",
        "your-profile"
      ]
    }
  }
}
```

### 3. Environment Setup

1. Set up your environment variables:
```bash
export SMITHERY_TOKEN=your_token_here
```

2. Configure your IDE (if applicable)
3. Test your connection

## Basic Usage

Here's a simple example of how MCP works:

1. **Tool Registration**: MCP servers register their capabilities
2. **Request Formation**: AI models form structured requests
3. **Execution**: The MCP server executes the request
4. **Response Handling**: Results are returned in a standardized format

## Next Steps

- Read the [Architecture Overview](./architecture.md)
- Explore [Available Tools](./tools.md)
- Learn about [Security Best Practices](./security.md)
- Check out [Advanced Features](./advanced.md)