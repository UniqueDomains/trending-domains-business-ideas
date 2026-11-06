# Trending Domains and Business Ideas, daily

Every morning at 06:00 UTC Unique Domains publishes two editions: [Trending Domains](https://unique.domains/trending-domains?utm_source=github&utm_medium=referral&utm_campaign=repo_trending_domains_business_ideas&utm_content=readme) for domain investors and [Business Ideas](https://unique.domains/business-ideas?utm_source=github&utm_medium=referral&utm_campaign=repo_trending_domains_business_ideas&utm_content=readme) for founders. Each names the trends rising in search and one domain name for each trend; the founder edition adds a business idea written for the trend.

This dataset carries the five names each edition opens to every reader, for the newest 90 editions of each page, in the edition's own order. It never ranks or scores the names.

## Files

- `trending-domains.json`: the investor editions, 145 rows.
- `business-ideas.json`: the founder editions, 0 rows.

## Fields

- `persona`, `date`: the page and the edition day (UTC).
- `trend`, `trend_slug`, `category`, `lane` (`weekly`: rising now; `yearly`: rising over the year), `searches` (monthly searches), `growth_percent`, `why_now` (one sentence written for the edition).
- `domain`, `ending`, `match_kind` (`exact`: the trend's own word; `related`), `relation` (how a related name relates to the trend).
- `status`, `price`, `price_kind`, `quoted_by`, `renewal_price`: the name as of the edition's publication.
- Founder rows: `five_year_cost`, `idea_title`, `idea_pitch`.
- Investor rows: `estimated_value`, `upside_percent` (an upside past 1,000% reads as the cap, with `upside_capped` true and no value), `liquidity`.
- `rating`: `strong` or `good` when the verdict holds at medium or high confidence, `unrated` otherwise; `risky` appears only on editions published before 2026-10-22, when Risky names stopped being published.

Updated on 2026-11-06 by UniqueDomains. Questions: kai@unique.domains.

## Terms

Permission is granted to view, download, quote, and cite this public extract for research, editorial, evaluation, and internal decision-support use, provided attribution to Unique Domains is preserved.

You may not:

- remove provenance or citation metadata,
- resell or redistribute this public extract as a competing bulk dataset without written permission,
- present the names as a ranking of the best domains.

All data is provided "as is" without warranties of completeness, accuracy, availability, legal clearance, or commercial outcome.

For commercial redistribution, API access, or partnership requests, contact kai@unique.domains.
