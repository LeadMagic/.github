# LeadMagic: B2B Data Enrichment APIs and Developer Tools

<img src="https://raw.githubusercontent.com/LeadMagic/.github/main/profile/assets/leadmagic.svg" width="64" height="64" alt="LeadMagic logo">

LeadMagic provides [B2B data enrichment APIs](https://leadmagic.io/product/enrichment-apis?utm_source=github&utm_medium=readme&utm_campaign=github&utm_content=profile-readme-intro) for sales workflows and AI agents. Find work emails, validate existing email lists, enrich people and companies, and research hiring and advertising signals.

[B2B enrichment API documentation](https://leadmagic.io/docs?utm_source=github&utm_medium=readme&utm_campaign=github&utm_content=profile-readme-intro) · [LeadMagic dashboard](https://app.leadmagic.io?utm_source=github&utm_medium=readme&utm_campaign=github&utm_content=profile-readme-intro) · [Pricing](https://leadmagic.io/pricing?utm_source=github&utm_medium=readme&utm_campaign=github&utm_content=profile-readme-intro)

Explore the [Email Finder](https://leadmagic.io/product/email-finder?utm_source=github&utm_medium=readme&utm_campaign=github&utm_content=profile-readme-products) or read the [email validation API guide](https://leadmagic.io/docs/api-reference/email-validation?utm_source=github&utm_medium=readme&utm_campaign=github&utm_content=profile-readme-products) to choose the right workflow for your contact data.

## Choose an integration

- **REST API:** `https://api.leadmagic.io` with an `X-API-Key` header.
- **Hosted MCP:** `https://mcp.leadmagic.io/mcp` with browser OAuth for supported AI clients.
- **Terminal:** [lm-tui](https://leadmagic.io/docs/cli/installation?utm_source=github&utm_medium=readme&utm_campaign=github&utm_content=profile-readme-choose-an-integration) installs the `lm` command; sign in with `lm login`.
- **n8n:** Install `n8n-nodes-leadmagic` through Community Nodes on a supported n8n installation.

## Public repositories

| Repository | Purpose |
| --- | --- |
| [leadmagic-openapi](https://github.com/LeadMagic/leadmagic-openapi) | Public REST API specification and validation |
| [leadmagic-n8n](https://github.com/LeadMagic/leadmagic-n8n) | n8n community node for enrichment workflows |
| [leadmagic-cursor-plugin](https://github.com/LeadMagic/leadmagic-cursor-plugin) | Cursor plugin using hosted MCP |
| [leadmagic-claude-plugin](https://github.com/LeadMagic/leadmagic-claude-plugin) | Claude Code plugin using hosted MCP |
| [leadmagic-skills](https://github.com/LeadMagic/leadmagic-skills) | LeadMagic API and workflow skills |
| [gtm-skills](https://github.com/LeadMagic/gtm-skills) | Go-to-market playbooks and agent skills |
| [leadmagic-mcp](https://github.com/LeadMagic/leadmagic-mcp) | Local stdio MCP integration for the documented enrichment subset |

`cold-email-cli` and `smartlead-mcp-server` are archived historical projects.

## Credits and data quality

Costs vary by endpoint and plan. Check your balance with the free `GET /v1/credits` endpoint and consult [credits documentation](https://leadmagic.io/docs/v1/credits?utm_source=github&utm_medium=readme&utm_campaign=github&utm_content=profile-readme-credits-and-data-quality) before a large run. Work emails returned by Email Finder are already validated; Email Validation is for emails sourced elsewhere.

## Support and security

Use [support@leadmagic.io](mailto:support@leadmagic.io) for product questions and [security@leadmagic.io](mailto:security@leadmagic.io) for private vulnerability reports. Never post credentials or customer enrichment results in public issues.
