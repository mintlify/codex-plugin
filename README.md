# Mintlify Codex plugin

A Codex plugin that gives comprehensive reference for building [Mintlify](https://mintlify.com) sites.

## What it does

Installs a `mintlify` skill that Codex can use when working on Mintlify-powered sites.

The skill covers:

- **Components** — Full syntax and props for all Mintlify components (callouts, cards, steps, tabs, accordions, code groups, fields, frames, and more)
- **Configuration** — Complete `docs.json` settings reference including theme, colors, logo, fonts, navbar, footer, redirects, integrations, and custom CSS/JS
- **Navigation** — All navigation patterns: groups, tabs, anchors, dropdowns, products, versions, and languages
- **API docs** — OpenAPI and AsyncAPI setup, endpoint pages, API playground configuration
- **CLI** — Full reference for every `mint` CLI command and flag

## Installation

Install from the Codex plugin directory, or add directly via the CLI:

```bash
codex plugin marketplace add mintlify/codex-plugin
```

## MCP setup

This plugin includes two Mintlify MCP servers that are activated automatically when you install the plugin.

- **Search MCP** — Read-only access to Mintlify's published documentation. Use to look up information about Mintlify: components, config options, guides, and other reference material.
- **Admin MCP** — Write access to your Mintlify project. Requires OAuth on first use. Enables editing content, restructuring navigation, opening pull requests, and managing site configurations directly from Codex.

## Skills included

### `mintlify`

The skill loads a concise core reference and routes to detailed reference files only when the task requires them:

| Reference file | Contents |
|----------------|----------|
| `reference/components.md` | All component syntax, props, and examples |
| `reference/configuration.md` | Full `docs.json` schema and frontmatter fields |
| `reference/navigation.md` | Navigation patterns and when to use each |
| `reference/api-docs.md` | API documentation setup and playground config |
| `reference/cli.md` | CLI commands and flags |

## License

MIT
