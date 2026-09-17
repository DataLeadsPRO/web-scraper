# Web Scraper API (Anti-Bot)

> Fetch, crawl, and browse protected pages with anti-bot handling - renders in a real browser and returns clean JSON or markdown.

Part of the **DataLeads** API suite (Data category). Requests render in a real browser with anti-bot handling and protected-page support built in - no proxies to manage, no infrastructure to run.

## Endpoints

| Method | Path | Description |
|---|---|---|
| POST | `/fetch` | V1 Fetch |
| POST | `/web/crawl` | V1 Web Crawl |
| POST | `/browse` | V1 Browse |
| POST | `/captcha/solve` | V1 Captcha Solve |

## Quick start

```bash
curl -X POST https://data.dataleads.pro/v1/fetch \
  -H 'Content-Type: application/json' \
  -d '{"clientKey": "YOUR_CLIENT_KEY", "url": "https://www.zillow.com/homes/Austin,-TX_rb/"}'
```

Replace `YOUR_CLIENT_KEY` with your key. Get one at [https://data.dataleads.pro](https://data.dataleads.pro) - free tier included.

## MCP server

- **Remote (Streamable HTTP):** `https://data.dataleads.pro/mcp/web-scraper`
- **Stdio (Docker):** `docker run -e DATALEADS_API_KEY=yourkey ghcr.io/dataleads/web-scraper-mcp:latest`

## Pricing

| Tier | Price | Requests |
|---|---|---|
| Free | $0 | 500/mo |
| Starter | $9/mo | 5,000 |
| Pro | $29/mo | 25,000 |
| Business | $99/mo | 100,000 |
| Enterprise | custom | custom |

Full plan details at [https://data.dataleads.pro](https://data.dataleads.pro).

## License

MIT - see [LICENSE](LICENSE).
