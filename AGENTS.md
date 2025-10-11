# Agent Instructions for adaptive-docs

## Build/Development Commands
- **Local dev**: `mintlify dev` (requires `npm i -g mintlify`)
- **Validate**: `mintlify validate`
- **Check links**: `mintlify broken-links`
- **Deploy**: Automatic on push to main (or `mintlify deploy`)

## Code Style & Content Guidelines

### MDX Files
- Use frontmatter with `title`, `description`, `icon` fields
- Follow existing component patterns: `<Card>`, `<CardGroup>`, `<Steps>`, `<CodeGroup>`, `<Note>`, `<Tabs>`
- Keep code examples working and copy-paste ready in cURL, Python, JavaScript
- Place code examples in `<CodeGroup>` with language-specific tabs

### Content Principles
- **Outcome-driven**: Start with value proposition and cost savings
- **Progressive disclosure**: Essential info first, advanced in expandable sections
- **5-minute success**: Time-boxed examples that work immediately
- **No preamble**: Direct, concise writing without unnecessary explanations

### File Organization
- API docs → `api-reference/*.mdx`
- Features → `features/*.mdx`
- Integrations → `integrations/*.mdx`
- Examples → `examples/*.mdx`
- Navigation managed in `docs.json`

### Configuration
- Site config: `docs.json` (Mintlify navigation, API settings, branding)
- Brand colors: Gold primary (#d4af37), light (#f0e68c), dark (#b8860b)
- OpenAPI spec: `api-reference/openapi.json`
