# Publish Changuito MCP to public directories

## Ready-to-copy directory listing

**Name:** Changuito — AI eCommerce Store Builder  
**GitHub:** https://github.com/PedidosUno/Changuito-MCP  
**Remote MCP:** https://mcp.changuito.net/mcp  
**Website:** https://changuito.com.ar/crear-con-ia  
**Category:** eCommerce, Business, Store Builder  
**Support:** soporte@changuito.com.ar  
**Privacy:** https://changuito.com.ar/privacidad

**English short description:** Create and customize online stores through AI chat in 10 Latin American countries.

**English long description:** Changuito connects AI assistants to online store setup via secure remote MCP. With the user's authorization and confirmation, an assistant can preview and create an online store, add products, configure branding, check setup status and provide the administration panel link. Supports 10 Latin American countries, with the Minha Lojinha brand in Brazil. 10-day free trial, no card required, and 0% Changuito commission on sales.

**Descripción en español:** Creá tu tienda online desde el chat con IA. Autorizá el acceso, revisá la vista previa y confirmá la creación. Luego podés cargar productos, personalizar tu marca y obtener el enlace al panel. 10 días de prueba gratis, sin tarjeta ni comisión de Changuito por venta.

## Directories to submit

| Directory | Destination | Notes |
| --- | --- | --- |
| Official MCP Registry | https://registry.modelcontextprotocol.io/ | GitHub Actions OIDC, no DNS verification |
| MCP.so | https://mcp.so/submit | Follow current submission form |
| MCP Directory | https://mcp.directory/submit | Follow current submission form |
| Glama | https://glama.ai/mcp/servers | Check current submission/claim process |
| Smithery | https://smithery.ai/ | Check current catalog submission policy |
| Awesome MCP Servers | https://github.com/punkpeye/awesome-mcp-servers | Follow contribution guidelines; PR if accepted |

A public GitHub repository is **not** an automatic submission or directory acceptance.

## Official MCP Registry — automated publishing

This repository's `server.json` uses **`io.github.PedidosUno/changuito-mcp`** to match the repository owner. The live MCP endpoint remains `https://mcp.changuito.net/mcp`.

The workflow [publish-mcp-registry.yml](../.github/workflows/publish-mcp-registry.yml) runs after changes to the manifest or publish workflow are merged to `main`. It can also be started manually using **Actions → Publish Changuito MCP to Official Registry → Run workflow**, selecting `main`.

The workflow checks the namespace and endpoint, downloads the official `mcp-publisher` release, validates `server.json`, authenticates with **`mcp-publisher login github-oidc`** using GitHub's short-lived OIDC token (`id-token: write`), publishes and checks that the public Registry API returns the record.

The [validation workflow](../.github/workflows/validate-metadata.yml) validates metadata on every PR; merge only when it succeeds. The private production application is never deployed or modified by either workflow.

**No GitHub Personal Access Token, domain key, DNS TXT record or repository secret is needed for GitHub OIDC.**

The Official Registry entry is a **different registry identifier** from the application's legacy discovery name `net.changuito/tienda`. Clients still connect to the same remote MCP URL. The live application's internal discovery metadata is not changed here.

**Check publication:** https://registry.modelcontextprotocol.io/v0.1/servers?search=io.github.PedidosUno%2Fchanguito-mcp

**Recommended tags:** ecommerce, online-store, store-builder, business, latin-america, remote-mcp, oauth.
