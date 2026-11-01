# Papua New Guinea Mining Tenements, Logging Concessions & Villages MCP

Connect your AI assistant (Claude, ChatGPT, Cursor) to [BumiAtlas](https://bumiatlas.com) for Papua New Guinea land-use research through the Model Context Protocol (MCP).

This listing is a focused entry point for:

- Mining tenements from the Mineral Resources Authority's ~2015 Landfolio export and a ~2013 snapshot: exploration licences, mining leases, special mining leases (Panguna, Ok Tedi, Lihir, Porgera), alluvial leases and easements, with titleholders and their equity
- Forestry concessions from the PNG Forest Authority, with type, plan id, dates, area and lifecycle remarks
- RSPO-certified palm oil estates, smallholder blocks and mills
- Census villages with ward, LLG, district, province and population
- Lookup by point, tenement code (`EL 1279`), name or holder

PNG has no public parcel cadastre: most land is customary. Tenement data stops at the snapshots: a licence past its expiry may since have been renewed or lapsed.

## Connect

```
https://bumiatlas.com/mcp/papuanewguinea
```

Add it as a custom connector in any MCP client and sign in with Google. Tools, examples and data notes: [bumiatlas.com/mcp-docs/papuanewguinea](https://bumiatlas.com/mcp-docs/papuanewguinea).

- **Claude:** Settings → Connectors → Add custom connector, paste the URL, then Connect.
- **ChatGPT:** Settings → Apps & Connectors → Advanced → Developer mode, then Create with the URL and OAuth authentication.

## Tools

| Tool | Description |
|---|---|
| `PG_concession_search` | Mining tenements, forestry concessions and palm oil sites at `latitude, longitude` or by code, name or holder; each record whole, boundaries as GeoJSON on request |
| `PG_village_search` | Census villages by name (narrowed by province, district or LLG) or near `latitude, longitude`, with population |

## Example prompts

- *"What mining tenements cover -5.4667, 143.1333?"*
- *"Who holds EL 2318, and when was it applied for?"*
- *"Which logging concessions are named Kamula Doso?"*
- *"Which census villages are near Port Moresby, and how many people live there?"*

## Data source

Tenements, concessions and palm oil © PNG Forest Authority (NFMS geo-portal); villages © DLPP LUIMS and the National Statistical Office. A copy of public data for research, not a legal record.
