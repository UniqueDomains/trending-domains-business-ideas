# Data Dictionary

The columns of `trending-domains.json`, `business-ideas.json` and their CSV twins, in file order.

| Field           | Type                           | Description                                                                                                   |
| --------------- | ------------------------------ | ------------------------------------------------------------------------------------------------------------- |
| persona         | founder or investor            | The page: Business Ideas (founder) or Trending Domains (investor).                                            |
| date            | date (YYYY-MM-DD)              | The edition day, UTC.                                                                                         |
| trend           | string                         | The trend the name answers.                                                                                   |
| trend_slug      | string or null                 | The trend's page slug.                                                                                        |
| category        | string or null                 | The trend's category.                                                                                         |
| lane            | weekly, yearly or null         | weekly: rising now; yearly: rising over the year.                                                             |
| searches        | number or null                 | Monthly searches for the trend.                                                                               |
| growth_percent  | number or null                 | The trend's search growth, in percent.                                                                        |
| why_now         | string or null                 | One sentence written for the edition.                                                                         |
| domain          | string                         | The domain name.                                                                                              |
| ending          | string                         | Its ending (TLD).                                                                                             |
| match_kind      | exact or related               | exact: the trend's own word; related: another word for it.                                                    |
| relation        | string or null                 | How a related name relates to the trend.                                                                      |
| status          | string                         | The name's status as of the edition's publication.                                                            |
| price           | number or null                 | Its price as of the edition, in USD.                                                                          |
| price_kind      | string or null                 | How the price was quoted: registration, premium, marketplace or auction.                                      |
| quoted_by       | string or null                 | Who quotes the price.                                                                                         |
| renewal_price   | number or null                 | The yearly renewal, in USD.                                                                                   |
| five_year_cost  | number or null                 | Founder rows: the first year plus four renewals.                                                              |
| estimated_value | number or null                 | Investor rows: the estimated value; empty when the est. profit passes 1,000%.                                 |
| upside_percent  | number or null                 | Investor rows: the est. profit over the price, as a percentage, capped.                                       |
| upside_capped   | boolean                        | True when the est. profit reads as the cap.                                                                   |
| liquidity       | high, medium, low or null      | Investor rows: how easily names like it sell.                                                                 |
| rating          | strong, good, risky or unrated | strong or good when the verdict holds at medium or high confidence; risky only on editions before 2026-11-05. |
| idea_title      | string or null                 | Founder rows: the business idea's title.                                                                      |
| idea_pitch      | string or null                 | Founder rows: the business idea.                                                                              |
