# Trending Domains and Business Ideas, daily

Every morning at 06:00 UTC Unique Domains publishes two editions: [Trending Domains](https://unique.domains/trending-domains?utm_source=github&utm_medium=referral&utm_campaign=repo_trending_domains_business_ideas&utm_content=readme) for domain investors and [Business Ideas](https://unique.domains/business-ideas?utm_source=github&utm_medium=referral&utm_campaign=repo_trending_domains_business_ideas&utm_content=readme) for founders. Each names the trends rising in search and one domain name for each trend; the founder edition adds a business idea written for the trend.

This dataset carries the five names each edition opens to every reader, for the newest 90 editions of each page, in the edition's own order. It never ranks or scores the names.

## Files

- `trending-domains.json`: the investor editions, 158 rows.
- `business-ideas.json`: the founder editions, 15 rows.
- `trending-domains.csv` and `business-ideas.csv`: the same rows and columns as CSV.
- `DATA_DICTIONARY.md`: every column, its type and what it holds.
- `LICENSE` and `CITATION.cff`.

## Fields

- `persona`, `date`: the page and the edition day (UTC).
- `trend`, `trend_slug`, `category`, `lane` (`weekly`: rising now; `yearly`: rising over the year), `searches` (monthly searches), `growth_percent`, `why_now` (one sentence written for the edition).
- `domain`, `ending`, `match_kind` (`exact`: the trend's own word; `related`), `relation` (how a related name relates to the trend).
- `status`, `price`, `price_kind`, `quoted_by`, `renewal_price`: the name as of the edition's publication.
- Founder rows: `five_year_cost`, `idea_title`, `idea_pitch`.
- Investor rows: `estimated_value`, `upside_percent` (an est. profit past 1,000% reads as the cap, with `upside_capped` true and no value), `liquidity`.
- `rating`: `strong` or `good` when the verdict holds at medium or high confidence, `unrated` otherwise; `risky` appears only on editions published before 2026-10-22, when Risky names stopped being published.

Updated on 2026-11-12 by UniqueDomains. Questions: kai@unique.domains.

From code: the [Node.js SDK and CLI](https://github.com/UniqueDomains/nodejs) (`npm install @uniquedomains/sdk`), the [Python client](https://github.com/UniqueDomains/python) (`pip install uniquedomains`) and the [MCP server](https://github.com/UniqueDomains/mcp-server) for AI assistants, hosted at `https://mcp.unique.domains/mcp`.

## How to cite

> Unique Domains, Trending Domains and Business Ideas, https://unique.domains/trending-domains, CC BY 4.0

Free under CC BY 4.0: see [LICENSE](./LICENSE). Citation metadata: [CITATION.cff](./CITATION.cff).
