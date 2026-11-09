# Changuito MCP — AI eCommerce Store Builder

**Official public discovery repository for Changuito's hosted MCP server.** This is documentation only. Changuito's production code, credentials and infrastructure are **not** published here.

**Remote MCP endpoint:** `https://mcp.changuito.net/mcp`  
**Transport:** Streamable HTTP · **Authentication:** OAuth with PKCE (S256) · **Registry ID:** `net.changuito/tienda`

[Create an online store with AI](https://changuito.com.ar/crear-con-ia) · [Server manifest](server.json) · [Tools](docs/tools.md) · [Authentication](docs/authentication.md) · [Directory submissions](docs/directories.md)

## What the MCP does

Connect a compatible AI client to Changuito and create or configure a new online store through conversation. The documented tools enable an assistant to check requirements and the desired store address, preview the store, **create it only after explicit user confirmation**, add products, set store branding, inspect store status, list connected stores and provide a link to the administration panel.

There are **nine documented MCP tools**. Other Changuito product modules—digital products, courses, subscriptions, events, experiences, rentals and appointments—are available in the wider platform but are **not separate MCP tools** in this integration.

## Connect

Add the following remote URL to a client supporting Streamable HTTP MCP and OAuth:

```text
https://mcp.changuito.net/mcp
```

Follow the Changuito OAuth authorization screen in your browser. Do **not** send a password or access token to an AI chat. Try: *Quiero crear una tienda online de ropa en Argentina.* Review the store preview before approving creation.

See [connection details](docs/authentication.md), [tool reference](docs/tools.md) and [example prompts](docs/examples.md).

## Platform and coverage

Changuito is an eCommerce platform operating in Argentina, Mexico, Colombia, Chile, Peru, Bolivia, Uruguay, Paraguay and Ecuador; in Brazil it uses the name **Minha Lojinha** ([minhalojinha.app](https://minhalojinha.app)). The platform supports physical and digital products, courses, subscriptions, events, experiences, rentals and appointments.

**Offer:** 10-day trial without a credit card; 0% commission charged by Changuito per sale. Other service/provider charges may apply.

## Security

Authentication and user authorization happen on Changuito's website. Documented OAuth scopes are `store:create`, `store:write` and `store:read`. The MCP has no tools for deleting stores or modifying payments or plan billing. See [SECURITY.md](SECURITY.md) for responsible disclosure.

## Discovery

- [Official Registry server.json](server.json)
- [Server card](https://mcp.changuito.net/.well-known/mcp/server-card.json)
- [Production registry metadata](https://mcp.changuito.net/.well-known/mcp/server.json)
- [OpenAPI](https://mcp.changuito.net/ai/v1/openapi.json)

This repository **does not mean the server has already been accepted into directories**; publication requires each directory's submission process and, for the Official Registry, domain ownership verification.

[Terms](https://changuito.com.ar/terminos) · [Privacy](https://changuito.com.ar/privacidad) · **Support:** soporte@changuito.com.ar

All rights reserved. This repository does not grant a license to the private Changuito source code.
