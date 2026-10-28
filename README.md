# Integrate.io MCP Server

The official MCP server for Integrate.io ETL and Reverse ETL. Connect Claude, ChatGPT, Cursor, OpenAI Codex or any MCP-compatible AI client to your Integrate.io account and build, run and monitor data pipelines in plain language.

> Integrate.io was formerly called Xplenty. Our API domain (api.xplenty.com)
> and this GitHub organization still use the old name.

- Product page: https://www.integrate.io/platform/mcp/
- Documentation: https://www.integrate.io/docs/etl/integrateio-mcp-server

## Connect

1. Copy your MCP server URL from Settings → Developer Settings → Connected Applications in the Integrate.io dashboard. It looks like
   https://api.xplenty.com/YOUR_ACCOUNT/api/mcp
2. Add it to your AI client as a remote MCP server and sign in with OAuth.
   Clients without OAuth support use a Personal Access Token, and
   stdio-only clients (Claude Desktop, Cursor, Codex) use the mcp-remote
   bridge. The docs have a ready-to-paste config for each.

Step-by-step setup for claude.ai, Claude Desktop, Claude Code, ChatGPT, Cursor
and OpenAI Codex: https://www.integrate.io/docs/etl/integrateio-mcp-server

## What it can do

44 tools in three groups:

| Group | Examples |
| --- | --- |
| Reading and inspecting | List connections, packages and runs; discover schemas; preview and profile data |
| Building and editing | Build a pipeline from a description; clone and edit packages; roll back versions |
| Jobs and schedules | Run, cancel and retry jobs; diagnose failures; manage schedules |

Full reference:
https://www.integrate.io/docs/etl/integrateio-mcp-server#tool-reference

## Security

- Actions follow the same roles and permissions as the Integrate.io app
- Every change made through MCP is recorded in the account's audit history
- Package edits are versioned and can be rolled back
- Access can be revoked at any time from Connected Applications
- Credentials, TLS certificates and SSL keys are never returned

## Support and privacy

- Support: https://www.integrate.io/support/
- Privacy policy: https://www.integrate.io/privacy/

<!-- mcp-name: io.github.xplenty/integrateio-mcp-server -->
