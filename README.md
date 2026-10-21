# 1102tools plugins for Cursor

Nine free hosted MCP servers for federal contracting data, packaged as Cursor plugins. Each plugin connects one server. There is no account to create and no API key to enter.

| Plugin | What it covers | Page |
|---|---|---|
| SAM.gov | Contract opportunities, entity registrations, SBA certifications and exclusions | [1102tools.com/mcp/sam-gov](https://1102tools.com/mcp/sam-gov) |
| USAspending | Past federal awards: contracts, grants, recipients, agencies and subawards | [1102tools.com/mcp/usaspending](https://1102tools.com/mcp/usaspending) |
| eCFR | FAR, DFARS and agency supplement text, definitions, and what changed and when | [1102tools.com/mcp/ecfr](https://1102tools.com/mcp/ecfr) |
| GSA CALC+ | Awarded labor ceiling rates for pricing proposals and IGCEs | [1102tools.com/mcp/gsa-calc](https://1102tools.com/mcp/gsa-calc) |
| BLS OEWS | Market wages by occupation and location for pricing proposals and IGCEs | [1102tools.com/mcp/bls-oews](https://1102tools.com/mcp/bls-oews) |
| GSA Per Diem | Lodging and M&IE rates by city, state or ZIP for pricing travel | [1102tools.com/mcp/gsa-per-diem](https://1102tools.com/mcp/gsa-per-diem) |
| Federal Register | Proposed and final rules, notices, comment periods and FAR case history | [1102tools.com/mcp/federal-register](https://1102tools.com/mcp/federal-register) |
| Regulations.gov | Rulemaking dockets, documents and public comments | [1102tools.com/mcp/regulations-gov](https://1102tools.com/mcp/regulations-gov) |
| Acquisition.gov | FAR Overhaul model text, posted agency deviations and guidance | [1102tools.com/mcp/acquisition-gov](https://1102tools.com/mcp/acquisition-gov) |

## How it's laid out

Each plugin lives in `plugins/<name>/` with a `.cursor-plugin/plugin.json` manifest, an `mcp.json` that points to the hosted Streamable HTTP endpoint, and a logo. The marketplace manifest is `.cursor-plugin/marketplace.json`.

To check the layout:

```bash
node scripts/validate-template.mjs
```

## Source

The server code is open source at [github.com/1102tools-dev/federal-contracting-mcps](https://github.com/1102tools-dev/federal-contracting-mcps).

## License

MIT. See [LICENSE](LICENSE).
