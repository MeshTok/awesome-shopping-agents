# awesome-shopping-agents

> [!TIP]
> **Build your own shopping agent in 5 minutes** — [BayDeep](https://baydeep.com) is a free hosted commerce gateway for AI agents: 7,000+ products, flight deals and attributed buy links via [one MCP URL](https://github.com/MeshTok/baydeep). [Get a free key →](https://baydeep.com/console/)

A curated list of open-source AI agents that browse, compare and shop — plus tools and gateways for building your own.

## Contents

- [Autonomous shopping agents](#autonomous-shopping-agents)
- [Browser-use shopping demos](#browser-use-shopping-demos)
- [Commerce gateways & tools](#commerce-gateways--tools)
- [Build your own](#build-your-own)

## Autonomous shopping agents

- [Agent-E](https://github.com/EmergenceAI/Agent-E) — autonomous agent for web tasks including price monitoring and form filling, built on Playwright + LLMs.
- [Operator-style computer-use agents](https://platform.openai.com/docs/guides/tools-computer-use) — computer-use models can navigate storefronts and checkouts directly.

## Browser-use shopping demos

- [browser-use](https://github.com/browser-use/browser-use) — the most-starred browser automation agent; commonly demoed on shopping flows (compare products, fill carts).
- [Playwright MCP](https://github.com/microsoft/playwright-mcp) — Microsoft's official Playwright MCP server; lets any MCP client drive a browser for product research.

## Commerce gateways & tools

- [BayDeep](https://github.com/MeshTok/baydeep) — hosted MCP + REST gateway: 7,000+ AliExpress products and flight fares as tools; free tier, keyless search, attributed buy links. ([docs](https://baydeep.com/docs/))
- [Playwright MCP](https://github.com/microsoft/playwright-mcp) — general browser tools (see above) usable as a shopping layer.

## Build your own

1. **Mount a commerce catalog as tools** — see the [BayDeep quickstart](https://baydeep.com/docs/quickstart.html) (one MCP URL, keyless search works immediately).
2. **Add attributed buy links** — `convert_link` turns any aliexpress.com URL into a tracked affiliate link per API key.
3. **Ship to users** — Claude/Cursor via MCP config; web apps via REST (`api.baydeep.com/v1`).

Example: an "under $50 air fryer" agent = `shelf_search(q="air fryer", price_max=50)` + `convert_link(detail_url)` + your UI.

## Contributing

PRs welcome — open-source shopping agents, MCP commerce servers, and tutorials. Keep entries real and maintained.
