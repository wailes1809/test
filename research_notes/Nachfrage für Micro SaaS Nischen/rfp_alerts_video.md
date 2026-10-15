# Public-Tender/RFP Alert Web App for Video Production Companies (AI relevance filter, summaries, deadline reminders)

> Research date: 2026-10-15. Sources accessed 2026-10-15 unless stated otherwise.
> **Method limitation (important for the report writer):** In this session WebFetch could not resolve any domain (DNS errors on open.gsa.gov, api.census.gov, rfpmart.com, govtribe.com, network.demandstar.com; reddit.com blocked). Direct shell access to the same hosts was refused by the egress proxy. After ~17 searches the shared web-search budget (200 calls per turn across all agents) ran out. So every finding below comes from **search-result snippets/summaries, not from full-page reads**. Several key questions (SAM.gov monthly counts, official Census counts, demand quotes, channels, half the competitor prices) are therefore **open gaps**, marked as such. A follow-up run with a fresh search budget should close them; the concrete queries/URLs to use are listed under each "Gaps" section.

## 1. Volume: how many video production tenders appear per month?

### Takeaway
No monthly count could be confirmed for any portal. The evidence available is qualitative: video production RFPs do appear regularly at federal level (NAICS 512110, PSC T006) and, more visibly, at state/local level (cities, water utilities, education agencies). RFPMart's indexed listings show at least 9 US state/local "Video Production Services" RFPs from May 2024 to Sep 2026 in a single search. Quantification is the biggest open item.

### Cited Findings
- NAICS 512110 (Motion Picture and Video Production) federal profile: **382 contractors** and **$198.4M in obligations** (time window not shown in snippet); recent awards come from GSA, among others. — [GovCon in a Box, NAICS 512110](https://www.govconinabox.com/explore/naics/512110)
- USFCR's NAICS 512110 page lists current federal solicitations, including a Veterans Affairs item with **Publish Date 09/18/2026**, but **most of the items listed under 512110 are not video work**. This points to noisy NAICS coding, which supports the case for an AI relevance filter. — [USFCR NAICS 512110 search](https://usfcr.com/search/naics/?naics=512110)
- Federal examples under NAICS 512: a "Video Production and Video Streaming Services Base IDIQ Contract", and a DoD combined synopsis/solicitation coded 512110. — [GovContractFinder NAICS 512](https://govcontractfinder.com/contracts/naics/512)
- An Army Corps of Engineers opportunity for "filming, editing, and producing research-based videos" (closed) is listed under 512110. — [Bidscope NAICS 512110 list](https://bidscopeai.com/lists/naics-code-512110)
- The PSC code **T006** appears in federal contract records as "Film/Video Tape Production Services" (records from about 2004–2009; aggregated FPDS copy, not the official PSC manual). — [openjurist.org PSC taxonomy](https://openjurist.org/gov/taxonomy/term/14638)
- State/local "Video Production Services" RFPs indexed by RFPMart (all in RFPMart's **"Marketing and Branding"** category):
  - Massachusetts, agency, short- and long-form videos, deadline **26 Sep 2025** — [RFPMart #1016843](https://www.rfpmart.com/1016843-usa-massachusetts-video-production-services-rfp.html)
  - California, city "state of the city" broadcast-quality video, deadline **10 Sep 2026** — [RFPMart #1148462](https://www.rfpmart.com/1148462-usa-california-video-production-services-rfp.html)
  - California, deadline **19 Jun 2025** — [RFPMart #976898](https://www.rfpmart.com/976898-usa-california-video-production-services-rfp.html)
  - Ohio, deadline **30 May 2025** — [RFPMart #935793](https://www.rfpmart.com/935793-usa-ohio-video-production-services-rfp.html)
  - Pennsylvania, water agency, educational/promotional videos, deadline **10 Sep 2025** — [RFPMart #1010275](https://www.rfpmart.com/1010275-usa-pennsylvania-video-production-services-rfp.html)
  - Pennsylvania, educational video production, deadline **15 May 2026** — [RFPMart #1113810](https://www.rfpmart.com/1113810-usa-pennsylvania-educational-video-production-services-rfp.html)
  - New York, deadline **3 May 2024** — [RFPMart #723076](https://www.rfpmart.com/723076-usa-new-york-video-production-services-rfp.html)
  - Colorado, deadline **13 May 2025** — [RFPMart #933650](https://www.rfpmart.com/933650-usa-colorado-video-production-services-rfp.html)
  - Hawaii, video production, broadcast and distribution, deadline **19 May 2025** — [RFPMart #940256](https://www.rfpmart.com/940256-usa-hawaii-video-production-broadcast-and-distribution-services-rfp.html)
- Other non-federal video RFP examples: CRDF Global (nonprofit) video solicitation (2024) — [CRDF Global Procurement & RFPs](https://www.crdfglobal.org/?p=20962); East Bay MUD campaign video RFP (2022) — [EBMUD](https://www.ebmud.com/download_file/force/10614/2253); Michigan education "Video Production Services – #proudMIeducator" — [cleat.ai listing](https://www.cleat.ai/government/contracts/video-production-services-proudmieducator-1woj)
- Canada and the UK also show "Marketing and Branding" RFPs for creative/brand work (e.g., BC visual identity/brand development, deadline 6 Feb 2026; PEI strategic marketing, deadline 6 Dec 2024). Creative services beyond video are a possible adjacent niche. — [RFPMart #1060034](https://www.rfpmart.com/1060034-canada-british-columbia-comprehensive-visual-identity-messaging-framework-and-brand-development-service-rfp.html); [RFPMart #877749](https://www.rfpmart.com/877749-canada-price-edward-island-strategic-marketing-and-promotions-service-rfp.html)

### Inferences
- The RFPMart samples are mostly **state/local** (cities, utilities, education). Video work seems to sit more in SLED than in federal procurement, where 512110 is noisy. **[Schätzung]**
- RFPMart listing IDs rose from ~723,000 (May 2024) to ~1,148,000 (Sep 2026). If the IDs are sequential across all categories, that would mean roughly 15,000 new listings per month across all categories worldwide. This is an indicator of aggregator scale only, not of video volume. **[Schätzung, IDs might not be sequential]**
- Because 512110 is noisy (USFCR snippet), a NAICS-only filter would generate irrelevant alerts. Keyword + PSC T006 + LLM classification is a concrete differentiator. **[Schätzung]**

### Gaps
- **No monthly counts** for SAM.gov (NAICS 512110 / PSC T006 / keyword "video production"), Contracts Finder, Find a Tender, CanadaBuys, AusTender or NZ GETS. These need a live query: e.g., the SAM.gov search UI with NAICS 512110 over the last 12 months; the CanadaBuys "all notices since Aug 2022" CSV filtered by title keyword "video"; a Contracts Finder OCDS search over 12 months with keyword filtering client-side.
- The current official PSC label for T006 is unconfirmed (only 2004–2009 records were seen).
- No data found on state/local volume for BidNet, DemandStar, Bonfire or OpenGov.
- NZ GETS: nothing found (search budget ran out).

## 2. Data access: public APIs / open data and their terms

### Takeaway
Free access without scraping exists for **CanadaBuys** (daily CSV, Open Government Licence – Canada, no key), **UK Contracts Finder** (public OCDS search API) and **UK Find a Tender** (OCDS API, OGL v3.0). **SAM.gov** has a public Opportunities API, but personal non-federal keys are tightly rate-limited (reported ~10 calls/day, unverified). **AusTender's** OCDS API covers awarded contracts only, not open tenders. **State/local portals** (BidNet, DemandStar etc.) have no public API evidence and are closed vendor platforms, so under the "no API without public access" rule they are out of scope for an MVP.

### Cited Findings
**SAM.gov (US federal)**
- The Get Opportunities API is reported at **~10 calls/day for non-federal (personal) accounts** and **~1,000/day for system accounts**. Query window max 1 year, `limit` up to 1,000 with offset paging. — [cleat.ai SAM.gov API developer guide](https://www.cleat.ai/developers/sam-gov-api)
- **Conflicting:** a (retired) Apify actor states **40 calls/day for new non-federal accounts** and **1,000/day for approved** ones, and says approval can take weeks. — [Apify foxlabs/sam-gov](https://apify.com/foxlabs/sam-gov)
- A state agency's SAM.gov user guide describes system accounts for REST API use but gives no quota numbers. — [NCDA&CS SAM system account user guide](https://www.ncagr.gov/food-distribution/system-award-management-sam-system-account-user-guide/download)
- Official documentation (open.gsa.gov/api/get-opportunities-public-api/) **could not be read** in this session (DNS failure).

**UK – Contracts Finder (below-threshold UK public contracts)**
- `GET Published/Notices/OCDS/Search` takes `publishedFrom`, `publishedTo`, `stages`, `limit` (1–100, default 100) and `cursor`. — [Contracts Finder API docs](https://www.contractsfinder.service.gov.uk/apidocumentation/Notices/1/GET-Published-Notice-OCDS-Search)
- Rate limiting: no numeric quota is published. Too many requests return **HTTP 403** ("The request rate limit may have been exceeded"), and clients should wait **5 minutes**. — [Contracts Finder API docs](https://www.contractsfinder.service.gov.uk/apidocumentation/Notices/1/GET-Published-Notice-OCDS-Search)
- The public endpoint filters only by date and stage, so keyword filtering has to happen client-side. — [Apify lafabbricallc/uk-contracts-finder-tenders](https://apify.com/lafabbricallc/uk-contracts-finder-tenders)
- API overview — [Contracts Finder API Help Page](https://www.contractsfinder.service.gov.uk/apidocumentation); OCDS implementation guide (PDF) — [GOV.UK](https://assets.publishing.service.gov.uk/media/5e99b67dd3bf7f0318cff3b8/Guide-to-Open-Contracting-Data-Standard-implementation-on-Contracts-Finder-V.2.1.pdf)

**UK – Find a Tender (above-threshold; Procurement Act 2023 notices)**
- `/api/{version}/ocdsReleasePackages` returns OCDS release packages with `limit` 1–100 (default 100), a `cursor`, and an `updatedFrom` filter. — [Find a Tender API docs](https://www.find-tender.service.gov.uk/apidocumentation/1.0/GET-ocdsReleasePackages); [Data and API documentation](https://www.find-tender.service.gov.uk/Developer/Documentation)
- Licence: **Open Government Licence v3.0** (per the OCDS data registry). — [Open Contracting data registry: Find a Tender](https://data.open-contracting.org/en/publication/41)
- No official rate-limit figure was found. A third-party actor reports 429/503 with `Retry-After` (unverified). — [Apify civicrows/uk-find-a-tender-notices](https://apify.com/civicrows/uk-find-a-tender-notices)

**Canada – CanadaBuys**
- An official open-data **CSV** dataset covers tender notices open on or after 8 Aug 2022. Files include open notices, new notices and all notices since Aug 2022. It is refreshed **daily between 7:00 and 8:30 ET**. — [open.canada.ca: CanadaBuys tender notices](https://open.canada.ca/data/en/dataset/6abd20d4-7a1c-4b38-baa2-9525d0bb2fd2)
- Licence: **Open Government Licence – Canada**, which allows commercial reuse with attribution. **No API key and no dedicated REST API**: access is by bulk CSV. — [open.canada.ca dataset](https://open.canada.ca/data/en/dataset/6abd20d4-7a1c-4b38-baa2-9525d0bb2fd2); [DEV Community 2026 guide](https://dev.to/truenorthdata/how-to-get-canadian-government-tenders-by-api-2026-guide-4oa1)
- The archived tender-notice datasets (from April 2023) are no longer updated. — [open.canada.ca archived tender notices](https://open.canada.ca/data/en/dataset/ffd38960-1853-4c19-ba26-e50bea2cb2d5)

**Australia – AusTender**
- The public OCDS API (api.tenders.gov.au/ocds) exposes **contract notices (awards)**, searchable by published, start, end and last-modified dates back to about 2013. — [GitHub austender/austender-ocds-api](https://github.com/austender/austender-ocds-api)
- **Approaches to Market (open tenders) are not in the OCDS API.** One vendor claims AusTender does not license ATM data for redistribution (unverified). — [Apify lafabbricallc AusTender](https://apify.com/lafabbricallc/australia-austender-contract-notices); background: [Open Contracting Partnership 2020](https://www.open-contracting.org/2020/02/11/what-does-australias-open-contracting-data-look-like/)
- Licence reportedly **CC BY 3.0 AU** (vendor claim, unverified). — [firecrawl AusTender page](https://www.firecrawl.dev/alexandria/tenders-gov-au)

**Market signal: many scrapers/wrappers already exist**
- There are Apify actors for SAM.gov, Contracts Finder, Find a Tender, CanadaBuys and AusTender. — e.g. [Apify crawlerbros/sam-gov-scraper](https://apify.com/crawlerbros/sam-gov-scraper), [Apify jungle_synthesizer CanadaBuys](https://apify.com/jungle_synthesizer/canadabuys-government-tenders-scraper), [Apify parseforge UK Contracts Finder](https://apify.com/parseforge/uk-contracts-finder-scraper)

### Inferences
- An MVP that stays within the hard rule could cover **US federal (SAM.gov API) + UK (Contracts Finder + Find a Tender) + Canada (CanadaBuys CSV)**. Australia open tenders and US state/local would need scraping, which breaks the rule. **[Schätzung]**
- If the SAM.gov personal-key limit really is about 10 calls/day, a once-daily pull of the last 24 h filtered by NAICS/PSC/keyword (a few calls, paged at 1,000 records) is still workable for a small number of users, since all users share one central pull. **[Schätzung]**
- The core weakness: the visible video RFPs are mostly state/local (section 1), and that layer is **not openly accessible**. A federal/UK/CA-only product may feel thin to a US video company. **[Schätzung]**

### Gaps
- The official SAM.gov API terms, rate limits per role and key-approval time are **not verified** (open.gsa.gov unreachable). Also unverified: whether SAM.gov's public "Contract Opportunities" bulk CSV extract on the Data Services page (known from prior knowledge, not checked here) can replace the API.
- NZ GETS: no API/open-data information found.
- No evidence found either way on public APIs/feeds for US state portals (e.g., Cal eProcure, NYS Contract Reporter, Texas ESBD) or for Bonfire/OpenGov/Periscope. Many state portals publish public HTML search pages and some publish RSS. This needs checking per state.

## 3. Free alternatives

### Takeaway
The most important free substitutes confirmed in this session are BidNet Direct's free Basic account (real-time email matches for member agencies) and DemandStar's free single-agency notifications. SAM.gov saved-search alerts and UK Contracts Finder alerts are widely known but were **not verified** here. Several new "free alternative" startups (GovBid, Civic IQ) are also positioning against the paid incumbents.

### Cited Findings
- **BidNet Direct Basic is free and permanent (not a trial):** browse and submit bids to member agencies and get real-time matches by email. Registration is required. — [Civic IQ BidNet Direct review (checked Aug 2026)](https://civiciq.com/blog/civic-iq-bidnet-direct-review); [BidNet Direct vendor solutions](https://www.bidnetdirect.com/vendor-solutions); [GovBid comparison](https://govbid.ca/compare/bidnet-direct)
- **DemandStar Basic is free** for notifications from **one** procurement agency, and members can search the whole bid database for free. Downloading a bid package costs a **$5 fee** for non-subscribers. — [DemandStar supplier pricing](https://network.demandstar.com/pricing-suppliers/); older Onvia-era "Free Agency" terms: [City of Deltona PDF](https://www.deltonafl.gov/DocumentCenter/View/537/Onvia-Demand-Star-Vendor-Subscription-Options-PDF)
- GovBid markets itself as a **"free alternative"** to BidNet Direct and DemandStar (2026). — [GovBid vs DemandStar](https://govbid.ca/compare/demandstar)
- GovTribe offers a 7-day free trial with no credit card (third-party). — [stork.ai GovTribe](https://www.stork.ai/en/govtribe)

### Inferences
- A video company can get free email alerts from SAM.gov, BidNet (member agencies) and DemandStar (one agency). The pain is fragmentation and noise, not lack of alerts. The value proposition has to be "one feed, video-only, summarized, with deadlines", not "access". **[Schätzung]**

### Gaps
- Not verified this session: SAM.gov saved-search email notifications (features and frequency), Contracts Finder / Find a Tender email alerts, CanadaBuys alerts, AusTender ATM email notifications, Bonfire/OpenGov free vendor accounts.
- APEX Accelerators (formerly PTACs) reportedly offer free bid-matching to small businesses (prior knowledge, **unverified**). This is relevant as both a free substitute and a channel.

## 4. Paid competitors and exact prices

### Takeaway
Paid tools range from **RFPMart at $35–50/month** (category-based; video RFPs sit in "Marketing and Branding") through BidNet Direct ($599–1,999/yr) and DemandStar ($60/county to ~$2,699/yr national) to federal intelligence platforms (GovTribe $1,500–6,000/yr). None was found offering a video-specific AI filter. A user complaint about irrelevant notifications was found on G2 for BidPrime. **RFPMart is the closest low-price comparator** and anchors willingness-to-pay at about $35–50/month.

### Cited Findings
| Vendor | Price (as found) | Source / date |
|---|---|---|
| **RFPMart** | "Marketing and Branding Services @ **$50 US/Month** (*No commitment)"; "Marketing, Branding and Related Services (Yearly) @ **$500 US/Year**"; recurring fees non-refundable | [RFPMart subscription page](https://www.rfpmart.com/view-subscription.html) (snippet, accessed 2026-10-15) |
| RFPMart (listing pages) | "Monthly Unlimited Subscription starts from **$35**, depends upon the category"; single RFP document **$7**; 2024 listings said from $30; cancel anytime, no partial refunds | e.g. [RFPMart #1129131 (NY, deadline Jul 2026)](https://www.rfpmart.com/1129131-usa-new-york-marketing-and-advertising-company-service-rfp.html); [RFPMart #1148462](https://www.rfpmart.com/1148462-usa-california-video-production-services-rfp.html) |
| RFPMart category fit | Video production RFPs are filed under **"Marketing and Branding RFP"** (no separate video category seen) | listing titles above |
| **GovTribe** | Launch **$1,500/yr** (federal, 1 user, 50-record export); Launch Plus **$1,900/yr** (federal+state+local); Growth **$5,000/yr** (federal, 5 users); Growth Plus **$6,000/yr** (fed+SLED); Scale custom | [GovTribe user guide: choose the right plan](https://govtribe.com/docs/govtribe-user-guide/guides/choose-the-right-govtribe-plan) (undated) |
| GovTribe (conflicting) | ~$1,350/yr federal, ~$1,800 fed+state (Jorpex); "~$25,000/yr" (Fed-Spend, a competitor, likely refers to something else) | [Jorpex](https://jorpex.com/compare/govtribe-alternatives/); [Fed-Spend 2026](https://fed-spend.com/blog/govtribe-pricing-2026-four-numbers-it-will-not-show) |
| **HigherGov** | No official price found. SoftwareSuggest: Starter **$500** (1 user), Standard $2,500 (≤10 users), Leader $5,000 (≤50 users), billing period unclear. Competitor GovContractFinder claims $150–500+/mo plus a **$995/yr SLED add-on** (biased) | [SoftwareSuggest HigherGov pricing](https://www.softwaresuggest.com/highergov/pricing); [GovContractFinder HigherGov pricing](https://govcontractfinder.com/compare/highergov/pricing) |
| **BidNet Direct** | Free Basic; paid **$599/yr one state, $1,199/yr three states, $1,999/yr nationwide**; Federal add-on $149/yr or $25/mo; Advertising Profile $249/yr | [Civic IQ review (checked Aug 2026)](https://civiciq.com/blog/civic-iq-bidnet-direct-review) |
| BidNet Direct (older/conflicting) | $9/state/month (group agencies), $36/state/month (state & local), ~$45/state/month federal bundle; up to 20% off for 2-year terms. Civic IQ says these no longer match the live page | [Walturn](https://www.walturn.com/insights/bidnet-direct-and-beyond-navigating-public-procurement-platforms-for-startups); [research.com](https://research.com/software/reviews/bid-net-direct-review) |
| **DemandStar** | Free (1 agency); County from **$60/yr per county**; State **$100–1,499/yr** (depends on agencies in state); National ~**$2,699/yr** (third-party, Jun 2026); $5 per bid download for non-subscribers | [DemandStar supplier pricing](https://network.demandstar.com/pricing-suppliers/); [GovBid (Jun 2026)](https://govbid.ca/compare/demandstar) |
| DemandStar (conflicting) | "from $99/month" | [ConstructionBids.ai 2026](https://constructionbids.ai/blog/demandstar-review-pricing-alternatives-2026) (contradicts the official per-year pricing) |
| **BidPrime** | No official price found. A G2 reviewer paid **$749** one year, then was auto-renewed at **>$812**; no online way to turn off auto-renew; 10% charge if cancelling within 10 days of renewal | [G2 BidPrime reviews](https://g2.com/products/bidprime/reviews) |

**Reviews / complaints about noise**
- BidPrime (G2): one reviewer complained of **too many irrelevant notifications despite keyword tuning**. Another said "Pricing and subscription costs feels high especially for small firms starting with bid sourcing". A positive reviewer valued the daily email of bids "released in all over US". — [G2 BidPrime reviews](https://g2.com/products/bidprime/reviews)

**New AI/"free" gov-bid entrants seen in 2026 search results (pricing not checked)**
- Civic IQ ([civiciq.com](https://civiciq.com/blog/civic-iq-bidnet-direct-review)), GovBid ([govbid.ca](https://govbid.ca/compare/demandstar)), BidSparq ([bidsparq.com](https://bidsparq.com/vs/demandstar)), Bidscope AI ([bidscopeai.com](https://bidscopeai.com/lists/naics-code-512110)), cleat.ai ([cleat.ai](https://www.cleat.ai/developers/sam-gov-api)), SamSearch ([samsearch.co](https://samsearch.co/naics-ai-lookup/512110)), GovCon in a Box ([govconinabox.com](https://www.govconinabox.com/explore/naics/512110)), Gov Contract Finder ([govcontractfinder.com](https://govcontractfinder.com/tools/government-contracting-software-pricing-guide)), Fed-Spend ([fed-spend.com](https://fed-spend.com/blog/govwin-govspend-govtribe-bloomberg-pricing-compared-2026)), gngo.app ([gngo.app](https://gngo.app/compare/bidnet)), ConstructionBids.ai (vertical: construction) ([constructionbids.ai](https://constructionbids.ai/blog/demandstar-review-pricing-alternatives-2026)), Jorpex ([jorpex.com](https://jorpex.com/compare/govtribe-alternatives/)), Revuo ([revuo.ai](https://www.revuo.ai/category/tender-management/bidnet-direct)).
- GovTribe itself has shipped AI features: "GovTribe AI access" in plans, and credit-billed "GovTribe MCP tools". — [GovTribe user guide](https://govtribe.com/docs/govtribe-user-guide/guides/choose-the-right-govtribe-plan); [GovTribe blog Q2 2026](https://blog.govtribe.com/whats-new-in-govtribe-q2-2026)

### Inferences
- **ConstructionBids.ai shows the "vertical AI bid finder" pattern already exists for construction.** No video/creative-specific equivalent appeared in the results. The niche looks open but adjacent to a crowded horizontal space. **[Schätzung]**
- Price anchor: a video-only tool at **$29–49/month** would sit at or just below RFPMart's category price and far below BidNet's nationwide plan (~$167/mo equivalent). **[Schätzung]**
- RFPMart's "Marketing and Branding" category mixes video with ads, PR and web work, so a video owner paying $35–50 still has to filter manually. That is the noise gap an AI filter targets. **[Schätzung]**

### Gaps
- Not researched (search budget exhausted): **GovWin IQ (Deltek), GovSpend, Periscope/ConnectBid, FindRFP, Instant Markets, Bidscout**, plus marketing/creative-agency RFP newsletters (e.g., agency-focused RFP digests). There are **no verified prices** for these.
- The RFPMart $35 vs $50 discrepancy is unresolved: listing pages say "from $35, depends on category", while the subscription page shows $50 for Marketing & Branding.
- No Capterra or Trustpilot review complaints were collected. Only one G2 complaint (BidPrime) is documented.

## 5. Demand signals (owners discussing government bids/RFPs and tools)

### Takeaway
**No quotes collected.** Reddit could not be fetched and the search budget ran out before demand-signal queries were run. This is the most important gap to close before building.

### Cited Findings
- Indirect signal only: the video-production RFP guides and templates published by production companies/agencies show the topic matters to video vendors (though they target buyers writing RFPs). — [Levitate Media video production RFP guide](https://levitatemedia.com/learn/video-production-rfp); [Thrive Agency RFP template](https://thriveagency.com/video-production-rfp-template)
- Indirect signal: BidPrime users value daily US-wide bid emails but complain about irrelevant alerts and high prices for small firms (see section 4). — [G2 BidPrime reviews](https://g2.com/products/bidprime/reviews)

### Inferences
- Indirect evidence only. Demand from small video companies for government work is **unproven** in this research. **[Schätzung]**

### Gaps
- Needed for the follow-up run (aim for 4+ quotes with URL and date): `site:reddit.com/r/videography government contract`, `r/videography RFP`, `r/GovernmentContracting video production`, `r/smallbusiness government bids video`, `LinkedIn "video production" "RFP" government`, `"video production" "SAM.gov" blog`, and a YouTube search for "government contracts for video production companies".

## 6. Potential customers: number of video production businesses

### Takeaway
No official count was retrieved. The 2022 County Business Patterns (released 27 Jun 2024) contains the figure, but the Census API was unreachable. Third-party sites quote roughly **16,700 companies** or **~25,000 establishments** for NAICS 512110. Those figures conflict and are unverified. Only **382 contractors** show federal 512110 obligations, which is the "already selling to government" segment.

### Cited Findings
- Census released **2022 CBP on 27 Jun 2024**. It covers establishments with paid employees by 6-digit NAICS (2017 NAICS) and by employment-size class (US and state level). — [Census press release 2024](https://census.gov/newsroom/press-releases/2024/county-business-patterns.html); [api.census.gov 2022 CBP](https://api.census.gov/data/2022/cbp)
- Third-party figures (search-snippet level, conflicting, exact attribution within the result set could not be verified because the pages could not be opened):
  - **16,737 companies** in NAICS 512110, one site attributing this to Census Bureau data; another site reports **9,368** "verified active" companies (a database count). — among [naicslist.com 512110](https://naicslist.com/naics/512110), [siccode.com 512110](https://siccode.com/naics-code/512110/motion-picture-video-production), [naicscodes.org 512110](https://naicscodes.org/code/512110-motion-picture-and-video-production/)
  - **24,972 establishments** ("2025 annual average"), with California at 6,730 (38.8%). That share implies a national total of ~17,300, so the profile is internally inconsistent. — [fairmarketvalue.com 512110 report](https://www.fairmarketvalue.com/resources/industries/512110/motion-picture-and-video-production)
- Federal: **382 contractors** with 512110 obligations (time frame not shown). — [GovCon in a Box](https://www.govconinabox.com/explore/naics/512110)
- NAICS 512110 is unchanged between the 2017 and 2022 NAICS revisions. — [naicslist.com](https://naicslist.com/naics/512110)

### Inferences
- The employer-establishment count is probably in the high teens of thousands (consistent with 16.7k–17.3k). The CBP count excludes the large number of non-employer freelancers/solo videographers. **[Schätzung]**
- The realistic early-adopter pool is small, because most video firms do not bid on public work. If even 2–5% of ~17k employer firms actively bid on public RFPs, that is ~350–850 US firms. That squares with the 382 federal contractors figure. **[Schätzung]**

### Gaps
- Official 2022 CBP 512110 establishment count by size class. Retrieve with: `https://api.census.gov/data/2022/cbp?get=NAICS2017_LABEL,EMPSZES,EMPSZES_LABEL,ESTAB,EMP&for=us:*&NAICS2017=512110` (unverified query, API unreachable here). Also Nonemployer Statistics for 512110.
- UK (ONS UK Business Counts, SIC 59112 "Video production activities"), Canada (StatCan Canadian Business Counts, NAICS 512110) and Australia (ABS Counts of Australian Businesses, ANZSIC 5511): **not retrieved**.

## 7. Channels to the first 10 paying customers

### Takeaway
**Not researched** (search budget exhausted). No association, community or newsletter data with sources was collected.

### Cited Findings
- Only incidental finding: the RFPMart listings show the same video RFPs are public. Posting curated "this week's video production RFPs" content (with links to the public source) is technically feasible as a lead magnet, since the notices are public records. — [RFPMart #1148462](https://www.rfpmart.com/1148462-usa-california-video-production-services-rfp.html) (example notice)

### Inferences
- Channel candidates from prior knowledge, **all unverified in this session [Schätzung]**: subreddits r/videography, r/VideoEditing, r/GovernmentContracting, r/smallbusiness; LinkedIn (video production company owners); APEX Accelerators (free government-contracting counselors who could refer clients); wedding/event videographer and commercial-producer associations; video-industry newsletters/podcasts; Facebook groups for video business owners. A free weekly "video RFP digest" newsletter is the natural no-ad-budget funnel into a paid alert tier.

### Gaps
- Needed: names, member counts and URLs for video industry associations (US/UK/CA/AU), subreddit subscriber counts, relevant newsletters with subscriber numbers, and whether APEX Accelerators accept vendor-tool partnerships. None was verified.
