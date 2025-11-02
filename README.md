# GoldenPine MCP Server

**Donate BTC**: bc1qx7yjzd9lmr8u2zzerrkh6mvnmw6zc4rj5aqsjg

Pine Script v6 Documentation MCP Server for Claude. Provides comprehensive function search, documentation access, and usage statistics for TradingView Pine Script development.

## Features

- Function search across 500+ Pine Script v6 functions
- Complete API documentation with syntax and parameters
- Multi-return function documentation (tuple handling)
- Usage statistics and performance tracking
- Community-contributed examples and tutorials

## Installation

### Claude Desktop Installation

**Method 1: MCPB Bundle (Recommended)**

1. Download `goldenpine-mcp-server.mcpb` from Releases
2. Move to Claude configuration directory:
   - macOS: `~/Library/Application Support/Claude/`
   - Windows: `%APPDATA%\Claude\`
3. Restart Claude Desktop
4. Verify installation in Claude tools menu

**Method 2: From ZIP**

1. Download `goldenpine-mcp-server.zip` from Releases
2. Rename file extension from `.zip` to `.mcpb`
3. Move to Claude configuration directory (see paths above)
4. Restart Claude Desktop

Note: `.mcpb` format is Claude's MCP Bundle format (renamed ZIP file).

### Manual Installation

```bash
git clone https://github.com/TelephoneJack/goldenpine-mcp.git
cd goldenpine-mcp
bun install
bun run build
```

Configure Claude Desktop (`claude_desktop_config.json`):

```json
{
  "mcpServers": {
    "goldenpine": {
      "command": "bun",
      "args": ["run", "/absolute/path/to/goldenpine-mcp-server/dist/server.js"]
    }
  }
}
```

Restart Claude Desktop.

## Usage

Query Pine Script functions through Claude:

```
"Search for moving average functions"
"Show me ta.sma documentation"
"What parameters does ta.rsi accept?"
"Find functions for volume analysis"
```

## Technical Specifications

**Language**: TypeScript/JavaScript  
**Runtime**: Bun  
**Protocol**: Model Context Protocol (MCP)  
**Target**: Claude Desktop  
**Pine Script Version**: v6

## Repository Structure

```
goldenpine-mcp-server/
├── src/                 # Source code
├── dist/                # Compiled output
├── examples/            # Community examples
│   ├── trend-indicators/
│   ├── momentum-indicators/
│   └── volume-analysis/
├── tutorials/           # Learning guides
│   ├── beginner/
│   ├── intermediate/
│   └── advanced/
└── edge-cases/          # Common errors and solutions
```

## Contributing

Community contributions accepted for:
- Usage examples
- Tutorials
- Edge case documentation
- Bug reports

See [CONTRIBUTING.md](CONTRIBUTING.md) for submission guidelines and formatting requirements.

## License

MIT

## Support

**Issues**: GitHub Issues  
**Documentation**: [Link to full documentation if applicable]

---

**Project Status**: Active Development  
**Maintainer**: TelephoneJack
