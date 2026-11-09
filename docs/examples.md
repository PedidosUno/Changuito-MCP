# Example MCP requests (reviewer guide)

Examples are suggested test scenarios, not proof of a successful live test.

1. **Store creation:** "Quiero crear una tienda de ropa en Argentina, en Pergamino, llamada Moda Demo." Expect requirements, slug check, preview, **explicit confirmation**, then `create_store`.
2. **Products:** "Agregá dos remeras a $10.000 y tres pantalones a $20.000." Expect `add_products`, scoped to the authorized store.
3. **Branding:** "Usá mi logo y los colores verde y blanco." Expect `set_branding` using user-provided assets.
4. **Status:** "¿Qué le falta a mi tienda?" Expect `get_store_status` and `get_panel_link`.

## Manual QA checklist

- Remote connection established using the actual endpoint.
- OAuth browser flow completed without revealing credentials to the assistant.
- Read-only tools function; unauthorized data is unavailable.
- Store creation requires user approval.
- Product/branding writes affect only an authorized store.
- AI connections can be revoked.
