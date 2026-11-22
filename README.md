# Username Search – Find Accounts on 3,000+ Sites: Username Search – Find Accounts on 3,000+ Sites Scraper API for Python & Node.js (2026)

Search any username across thousands of sites and get every matching profile URL with site, tags and status. No login needed. Export JSON, CSV or Excel.

**[▶ Try the Username Search – Find Accounts on 3,000+ Sites free on Scrapely](https://scrape.ly/store/cornerledger/username-osint-scraper)** · [Compare Scrapely vs other scraping tools](https://scrape.ly/compare)

This repository shows how to scrape Username Search – Find Accounts on 3,000+ Sites data with the [Username Search – Find Accounts on 3,000+ Sites](https://scrape.ly/store/cornerledger/username-osint-scraper) using the official
**Scrapely SDKs for JavaScript and Python**. You pass the input, Scrapely runs the username search – find accounts on 3,000+ sites scraper in the cloud
(proxies, retries, browser and scaling included) and returns clean, structured data as JSON, CSV or Excel.
No scraper code to maintain and no blocked requests to debug.

## Why use this Username Search – Find Accounts on 3,000+ Sites scraper

- **No-code or API:** run it from the [Scrapely Store](https://scrape.ly/store/cornerledger/username-osint-scraper) or from your code with the SDK.
- **Structured username search – find accounts on 3,000+ sites data:** ready-to-use fields instead of raw HTML.
- **Pay per result:** $17.00 per 1,000 profile found results, no monthly subscription required.
- **Maintained and monitored:** scrapers are tested around the clock and fixed fast when Username Search – Find Accounts on 3,000+ Sites changes.
- **Integrations:** n8n, Make, Zapier, LangChain, LlamaIndex, MCP (Claude, Cursor) and webhooks.

## What Username Search – Find Accounts on 3,000+ Sites data can you extract?

Search any username across thousands of sites and get every matching profile URL with site, tags and status. No login needed. Export JSON, CSV or Excel.

| Output field |
|---|
| `username` |
| `siteName` |
| `profileUrl` |
| `status` |
| `httpStatus` |
| `tags` |
| `alexaRank` |
| `fullName` |
| `location` |
| `scrapedAt` |

## Quick start

1. [Sign up for Scrapely](https://scrape.ly) (free plan available) and copy your API token from
   **Settings → API & Integrations**.
2. Clone this repo and set your token:

```bash
export SCRAPELY_TOKEN=your_token
```

### Node.js (JavaScript SDK)

```bash
npm install
node example.js
```

```js
const { ScrapelyClient } = require('scrapely-client');
const client = new ScrapelyClient({ token: process.env.SCRAPELY_TOKEN });

const run = await client.actor('cornerledger/username-osint-scraper').call({"usernames": ["nasa"], "topSites": 500, "proxyConfiguration": {"useScrapelyProxy": true, "scrapelyProxyGroups": ["DATACENTER"]}});
const { items } = await client.dataset(run.defaultDatasetId).listItems();
```

### Python (Python SDK)

```bash
pip install -r requirements.txt
python example.py
```

```python
from scrapely_client import ScrapelyClient
client = ScrapelyClient(os.environ['SCRAPELY_TOKEN'])

run = client.actor('cornerledger/username-osint-scraper').call(run_input={ "usernames": [ "nasa" ], "topSites": 500, "proxyConfiguration": { "useScrapelyProxy": True, "scrapelyProxyGroups": [ "DATACENTER" ] } })
items = list(client.dataset(run.default_dataset_id).iterate_items())
```

### REST API / cURL

```bash
curl -X POST "https://api.scrape.ly/v2/acts/cornerledger~username-osint-scraper/run-sync-get-dataset-items?token=$SCRAPELY_TOKEN" \
  -H "Content-Type: application/json" \
  -d @input.json
```

## Example input

```json
{
  "usernames": [
    "nasa"
  ],
  "topSites": 500,
  "proxyConfiguration": {
    "useScrapelyProxy": true,
    "scrapelyProxyGroups": [
      "DATACENTER"
    ]
  }
}
```

See every input option on the [Username Search – Find Accounts on 3,000+ Sites page](https://scrape.ly/store/cornerledger/username-osint-scraper).

## Pricing

**$17.00 per 1,000 profile found results.** Free plan available, no credit card needed to start. Check current pricing on the
[Store page](https://scrape.ly/store/cornerledger/username-osint-scraper) and see how Scrapely compares with other tools on [scrape.ly/compare](https://scrape.ly/compare).

## FAQ

**How do I scrape Username Search – Find Accounts on 3,000+ Sites with Python?** Install `scrapely-client-python`, set `SCRAPELY_TOKEN` and run
`example.py`. The scraper runs on Scrapely and you read the results from the dataset.

**How do I scrape Username Search – Find Accounts on 3,000+ Sites with Node.js?** Install `scrapely-client`, set `SCRAPELY_TOKEN` and run `example.js`.

**Is there a username search – find accounts on 3,000+ sites scraper API?** Yes. Call `POST https://api.scrape.ly/v2/acts/cornerledger~username-osint-scraper/runs`
or use `run-sync-get-dataset-items` to get results in one request.

**Do I need proxies?** No. Proxies, retries and browsers are handled by Scrapely.

**Is scraping Username Search – Find Accounts on 3,000+ Sites legal?** This scraper collects publicly available data. Check Username Search – Find Accounts on 3,000+ Sites's terms and the
laws that apply to you, especially for personal data (GDPR, CCPA).

**Can I schedule it or get results by webhook?** Yes. Use Scrapely schedules and webhooks, or n8n, Make and Zapier.

## Looking for an alternative?

Scrapely is an alternative to Apify, Bright Data, ScraperAPI, Firecrawl, Octoparse, PhantomBuster, SerpApi,
Zyte and others. See the side-by-side pricing on [scrape.ly/compare](https://scrape.ly/compare).

---

**Keywords:** username search – find accounts on 3,000+ sites, username search – find accounts on 3,000+ sites scraper, username search – find accounts on 3,000+ sites scraper api, username search – find accounts on 3,000+ sites scraper python, username search – find accounts on 3,000+ sites scraper node.js,
scrape username search – find accounts on 3,000+ sites, username search – find accounts on 3,000+ sites data extraction, username search – find accounts on 3,000+ sites crawler, username search – find accounts on 3,000+ sites api, export username search – find accounts on 3,000+ sites data to csv, username-osint-scraper

License: MIT. Example code only; the scraper runs on [Scrapely](https://scrape.ly/store/cornerledger/username-osint-scraper).
