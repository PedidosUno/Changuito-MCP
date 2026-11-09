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
| Official MCP Registry | https://registry.modelcontextprotocol.io/ | Publisher CLI, domain ownership verification |
| MCP.so | https://mcp.so/submit | Follow current submission form |
| MCP Directory | https://mcp.directory/submit | Follow current submission form |
| Glama | https://glama.ai/mcp/servers | Check current submission/claim process |
| Smithery | https://smithery.ai/ | Check current catalog submission policy |
| Awesome MCP Servers | https://github.com/punkpeye/awesome-mcp-servers | Follow contribution guidelines; PR if accepted |

A public GitHub repository is **not** an automatic submission or directory acceptance.

## Official MCP Registry

The remote server descriptor in [../server.json](../server.json) uses namespace `net.changuito/tienda`, which requires proof of control over **changuito.net**.

1. Download the publisher CLI from https://github.com/modelcontextprotocol/registry/releases .
2. In this repository, check `mcp-publisher --help` and validate `server.json`.
3. Follow the [official publishing guide](https://github.com/modelcontextprotocol/registry/blob/main/docs/modelcontextprotocol-io/quickstart.mdx) to authenticate via DNS or HTTP domain ownership. **Never commit the signing key or verification secrets.**
4. Publish the manifest and verify the resulting entry in the Official Registry.
5. Submit the public GitHub URL and remote MCP endpoint to other catalogs.

**Important:** GitHub login is not equivalent to ownership of the `net.changuito` domain namespace. The production metadata may use an older schema; the repository manifest must pass official CLI validation before publication.

**Recommended tags:** ecommerce, online-store, store-builder, business, latin-america, remote-mcp, oauth.
