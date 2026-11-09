# Authentication and connection

**MCP URL:** `https://mcp.changuito.net/mcp` (remote Streamable HTTP).

**OAuth:** PKCE S256 with dynamic client registration. Documented scopes: `store:create store:write store:read`.

## Discovery URLs

- [Authorization server metadata](https://mcp.changuito.net/.well-known/oauth-authorization-server)
- [Protected resource metadata](https://mcp.changuito.net/.well-known/oauth-protected-resource)
- [MCP server card](https://mcp.changuito.net/.well-known/mcp/server-card.json)
- [Registry metadata](https://mcp.changuito.net/.well-known/mcp/server.json)
- [OpenAPI](https://mcp.changuito.net/ai/v1/openapi.json)

## How to connect

1. Add a custom remote MCP server in a client that supports OAuth and Streamable HTTP.
2. Paste `https://mcp.changuito.net/mcp`.
3. Follow the authorization flow on Changuito's own website and approve the connection.
4. Use a read-only tool first, then preview store details before requesting confirmation for creation.

Never enter passwords, private keys, bearer tokens or authorization codes in an AI chat, public issue, or this repository.

Authorized connections can be revoked in **Mi cuenta → Conexiones de IA** in Changuito.

These instructions describe the application's configured authentication. Client interoperability must be verified with an end-to-end test against production.
