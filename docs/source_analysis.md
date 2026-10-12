# Source Analysis

| Website | robots.txt | Terms mention scraping? | Static or JavaScript? | Decision |
|---|---|---|---|---|
| PriceOye | Product pages allowed, no query strings | Yes: Section 5 prohibits data mining, robots, collecting listings/prices | Static | DROPPED: Terms prohibit automated collection |
| Telex (Telemart) | Products and collections allowed; cart, checkout, account, orders, sort_by and filter URLs blocked | Confirmed: telex.pk uses the Telemart Terms. No explicit mention of scraping; commercial-use and IP clauses noted | Static; public /products.json feed works; no review data | Main source: use carefully |
| Daraz | /catalog/ (search), cart, checkout blocked; product pages allowed | Yes: Section E prohibits collecting product listings/prices and using data mining or robots | Not checked (not needed) | DROPPED: Terms prohibit automated collection |
## Decision Log

### Decision 1: PriceOye removed as a data source

- **Date:** 12 October 2026
- **Finding:** PriceOye's robots.txt allows product pages, but Section 5 ("License to access the site") of its Terms and Conditions prohibits data mining, robots, similar data gathering tools, and the collection and use of product listings, descriptions or prices.
- **Reasoning:** robots.txt and the Terms of Use are separate. Even though the site is technically easy to scrape, the Terms do not allow it, and this project follows both.
- **Action:** PriceOye will not be scraped. No PriceOye data is stored in this repository.
- **Ethics link:** Respecting website terms of service and acting within the law (ACM/IEEE codes of ethics, PECA 2016).

### Decision 2: Telex (Telemart) kept as a source with conditions

- **Date:** 12 October 2026
- **Finding:** Telemart now runs at telex.pk (a Shopify store). Its robots.txt allows product and collection pages. Its Terms do not mention scraping, but they restrict commercial use and protect the site's intellectual property.
- **Reasoning:** Nothing explicitly prohibits public price collection, and this project is academic and non-commercial. Because the Terms are not a clear permission, the scraper will be careful and polite.
- **Action:** Collect only public product data, wait 2 to 3 seconds between requests, avoid cart, checkout, account, sort and filter URLs, collect no personal data, and never republish the data.
- **Ethics link:** Minimising harm to the website, respecting privacy, and using data only for its stated academic purpose (ACM/IEEE codes of ethics).

### Decision 3: Daraz removed as a data source

- **Date:** 12 October 2026
- **Finding:** Daraz's robots.txt allows product and category pages, but Section E ("License to access the site") of its Terms and Conditions excludes the collection and use of product listings, descriptions or prices, and the use of data mining, robots or similar data extraction tools. The wording matches PriceOye's Terms.
- **Reasoning:** Following the rules of a website means following its Terms as well as its robots.txt. The Terms do not allow automated collection.
- **Action:** Daraz will not be scraped. No Daraz data is stored in this repository. A second source will be chosen using the same checks (robots.txt, Terms, page source).
- **Ethics link:** Respecting website terms of service and acting within the law (ACM/IEEE codes of ethics, PECA 2016).
