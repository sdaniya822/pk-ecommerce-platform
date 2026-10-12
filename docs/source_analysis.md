# Source Analysis

| Website | robots.txt | Terms mention scraping? | Static or JavaScript? | Decision |
|---|---|---|---|---|
| PriceOye | Product pages allowed, no query strings | Yes: Section 5 prohibits data mining, robots, collecting listings/prices | Static | DROPPED: Terms prohibit automated collection |
| Telex | Products and collections allowed, cart/checkout blocked | Not checked yet | Not checked yet | Candidate source |
| Daraz | /catalog/ (search), cart, checkout blocked | Not checked yet | Not checked yet | Candidate source |

## Decision Log

### Decision 1: PriceOye removed as a data source

- **Date:** 12 October 2026
- **Finding:** PriceOye's robots.txt allows product pages, but Section 5 ("License to access the site") of its Terms and Conditions prohibits data mining, robots, similar data gathering tools, and the collection and use of product listings, descriptions or prices.
- **Reasoning:** robots.txt and the Terms of Use are separate. Even though the site is technically easy to scrape, the Terms do not allow it, and this project follows both.
- **Action:** PriceOye will not be scraped. No PriceOye data is stored in this repository.
- **Ethics link:** Respecting website terms of service and acting within the law (ACM/IEEE codes of ethics, PECA 2016).
