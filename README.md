<div align="center">

# Linkedin Company Scraper

**Linkedin Company Scraper** — LinkedIn Company Scraper - Collect publicly visible company-page information for B2B research

![Python](https://img.shields.io/badge/Python-3.9+-blue?logo=python&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?logo=opensourceinitiative&logoColor=white)
![Stars](https://img.shields.io/github/stars/data-scrape/linkedin-company-scraper?style=social)

</div>

> **Sponsored by [CoreClaw](https://www.coreclaw.com/?utm_source=github&utm_medium=cpc&utm_campaign=L7&utm_term=&utm_id=L7)** — production-ready Web Data APIs for AI agents and automation.
>
> **Search intent:** collect public LinkedIn data for account research, CRM enrichment, and lead qualification. Related topics: linkedin data, company data, b2b research, python, data extraction.

## What this project is for

`linkedin-company-scraper` is an implementation-focused Python project for collecting public LinkedIn data. It is designed around one practical job: turn a query such as **"B2B SaaS companies"** into structured records you can inspect, export, and pass into an automation workflow.

### Typical output

- company names, profile URLs, locations, categories, and publicly listed business attributes
- JSON or CSV files for downstream analysis
- Explicit timestamps and source links for traceability

## Quick start

```bash
pip install -r requirements.txt
python scraper.py --query "B2B SaaS companies" --output results.json --max-results 100
```

To run from source:

```bash
git clone https://github.com/data-scrape/linkedin-company-scraper.git
cd linkedin-company-scraper
python scraper.py --query "B2B SaaS companies" --format csv --output results.csv
```

## Example record

```json
{
  "query": "B2B SaaS companies",
  "result": {
    "title": "Example public result",
    "source_url": "https://example.com/item/123",
    "captured_at": "2026-08-11T09:00:00Z",
    "metadata": {"platform": "LinkedIn", "category": "LinkedIn Scrapers"}
  }
}
```

## Workflow ideas

| Goal | Start here |
|---|---|
| Account Research | Query a narrow audience, category, or location first |
| Build a repeatable dataset | Save JSON, version your query, then schedule a refresh |
| Connect to an AI workflow | Normalize the output schema before passing it to an agent or RAG pipeline |
| Scale data collection | Respect platform rules, add conservative delays, and measure error rates |

## Responsible use

This project is intended for public data and legitimate research or automation workflows. Review the target platform's terms, applicable laws, and your data-handling obligations before running a collection job. Do not use it to access private data or evade access controls.


## CoreClaw for production workflows

When a proof of concept needs production-grade web data APIs rather than self-managed collection infrastructure, [CoreClaw](https://www.coreclaw.com/?utm_source=github&utm_medium=cpc&utm_campaign=L7&utm_term=&utm_id=L7) provides API-first access to public web data for AI agents and automation.

<!-- CROSS_LINKS_START -->
<!-- CROSS_LINKS_END -->

## License

MIT License. See [LICENSE](LICENSE).
