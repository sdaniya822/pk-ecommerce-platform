\# Source Analysis



| Website | robots.txt | Terms mention scraping? | Static or JavaScript? | Decision |

|---|---|---|---|---|

| | PriceOye | Product pages allowed, no query strings | Section 5 prohibits data mining, robots, collecting listings/prices | Static | DROPPED: Terms prohibit automated collection |

| Telex | Products and collections allowed, cart/checkout blocked | (your finding) | (your finding) | Main source |

| Daraz | /catalog/ (search), cart, checkout blocked | (your finding) | (your finding) | Optional |















\## Decision Log



\### Decision 1: PriceOye removed as a data source

\- Date: (write today's date)

\- Finding: PriceOye's robots.txt allows product pages, but Section 5

&#x20; ("License to access the site") of its Terms and Conditions prohibits

&#x20; data mining, robots, similar data gathering tools, and the collection

&#x20; and use of product listings, descriptions or prices.

\- Reasoning: robots.txt and the Terms of Use are separate. Even though the

&#x20; site is technically easy to scrape, the Terms do not allow it, and this

&#x20; project follows both.

\- Action: PriceOye will not be scraped. No PriceOye data is stored in this

&#x20; repository.

\- Ethics link: respecting website terms of service and acting within the

&#x20; law (ACM/IEEE codes of ethics, PECA 2016).

