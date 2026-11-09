# Changuito MCP tools

These are the nine tools documented by Changuito's application code; live `tools/list` is authoritative for current parameter schemas.

| Tool | Purpose | Writes? |
| --- | --- | --- |
| `get_requirements` | List countries, categories, templates and required information | No |
| `check_slug` | Check a proposed store URL/slug | No |
| `preview_store` | Validate and preview a store without creating it | No |
| `create_store` | Create a store after explicit user confirmation | Yes |
| `add_products` | Add products (documented limit: 25 per call) | Yes |
| `set_branding` | Set logo, cover, colors and template | Yes |
| `get_store_status` | Check setup status and next steps | No |
| `list_my_stores` | List stores created through this integration | No |
| `get_panel_link` | Obtain the store administration panel URL | No |

**Approval:** Always preview and ask for explicit consent before creating a store. Never request passwords, banking details or OAuth tokens in chat. Only modify stores belonging to the authorized account.

Application docs describe limits of 3 created stores per day, 10 per account, and 25 products per call. Live API limits take precedence.

**Scope note:** Digital products, courses, subscriptions, tickets, experiences, rentals and appointments are broader platform modules, not dedicated MCP tools in this published interface.
