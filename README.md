# Pakistan Import Export Data MCP

**Pakistan Customs Data: Importers, Suppliers & HS Codes.** Pakistan import export data for your AI assistant. Search Pakistan customs shipment records, find importers and foreign suppliers, and break down trade by HS code, partner country and counterparty company, through the Model Context Protocol.

An AI-native alternative to Pakistan trade data from Panjiva, ImportGenius, Volza, Seair, TradeInt and ExportGenius: ask in plain language instead of exporting spreadsheets.

The MCP connection is provided by [The Company Atlas](https://thecompanyatlas.com). This repository does not run a separate server.

## Connect

```
https://thecompanyatlas.com/mcp/trade/pakistan
```

Add this URL as a custom MCP connector in Claude, ChatGPT, Cursor, or any MCP-compatible client. Sign in with Google when prompted.

- Transport: Streamable HTTP
- Auth: Google OAuth (sign in once, stays authorized)
- Free accounts get 50 credits per calendar month
- Defaults to Pakistan: the server tells your AI to filter on `PK` unless you ask about another country

## Pakistan data coverage

- **Years:** 2019–2026
- **Records:** Import declarations: Pakistani importer, foreign supplier, origin country, HS code, goods description, value, quantity, port and date.
- **Country code:** `PK` (use `buyerCountry: "PK"` for imports into Pakistan)
- **Common products:** refined fuel (HS 2710), raw cotton (HS 5201), palm oil (HS 1511), cars (HS 8703)

## Notable traders in the data

Companies that appear most often in recent Pakistan records (by number of declaration lines, not value):

**Importers**

- Pakistan State Oil
- Gas & Oil Pakistan
- Parco Gunvor
- Attock Petroleum
- Shell Pakistan
- Paracha Textile Mills

## Example prompts

- *"Who are the top importers of palm oil (HS 1511) into Pakistan?"*
- *"Which Pakistani textile mills import raw cotton (HS 5201)?"*
- *"What does Pakistan State Oil import, by origin country?"*
- *"List importers of solar panels (HS 8541) into Pakistan in 2025"*
- *"Show recent shipments for Attock Petroleum"*

## Tools

### Trade search

| Tool | Description |
|---|---|
| `Trade_search_trades` | Paginated customs shipment search: filter by HS code, buyer, seller, country, port, value and date range |
| `Trade_company_trade_volume_by_year` | Rank importers or exporters by declared value and line counts per year, with HS code and country filters |

### Trade analytics

| Tool | Description |
|---|---|
| `Trade_hs_code_breakdown` | For one company, import and export value by HS chapter, heading or subheading |
| `Trade_year_country_breakdown` | For one company, trade value by year and counterparty country |
| `Trade_partner_breakdown` | For one company, trade value by year and matched counterparty company |

### Company registry

| Tool | Description |
|---|---|
| `Company_search` | Search the global company registry by name or id, with optional country filter |
| `Company_get_by_id` | Full company profile by id |

## Keywords

Pakistan import data, Pakistan export data, Pakistan customs data, Pakistan shipment data, importers in Pakistan, Pakistan buyers and suppliers, HS code search, Pakistan import data, Pakistan customs data, list of importers in Pakistan, HS code
