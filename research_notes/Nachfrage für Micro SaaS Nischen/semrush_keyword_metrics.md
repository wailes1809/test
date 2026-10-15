# Search demand & competitor traffic for 8 micro-SaaS niches (Semrush attempt + public proxies)

> **SEMRUSH STATUS (checked 2026-10-15): NOT AVAILABLE. These notes contain no numbers from the Semrush MCP.**
>
> - `keyword_research` (discovery call, no params) returned code `no_api_units`. Message (verbatim): "The user has an active Semrush subscription, but does not have enough API units to complete this request." url (verbatim): https://www.semrush.com/mcp-access (trace_id 6e0deb9dd17329d984c8bfb0e87554ac)
> - `competitors_research` (discovery call, no params) returned code `no_api_units`. Message (verbatim): "The user has an active Semrush subscription, but does not have enough API units to complete this request." url (verbatim): https://www.semrush.com/mcp-access (trace_id 79f30194bbd42f02a93a7172e4499102)
> - `traffic_overview` (discovery call, no params) returned code `no_subscription`. Message (verbatim): "The user does not have a Semrush plan that includes MCP access." url (verbatim): https://www.semrush.com/analytics/traffic/trends-api (trace_id 10e4100d579d339ae8456376455faadd)
>
> As instructed, Semrush use stopped after these three calls. `get_report_schema`, `execute_report` and `domain_overview` were never called.
>
> **Limits on the fallback (public proxies):**
> - WebFetch could not resolve any external host in this environment (`getaddrinfo ENOTFOUND`). This affected suggestqueries.google.com (Google autocomplete), similarweb.com, semrush.com (public pages) and ispionage.com. No page could be opened to check its numbers directly.
> - Only WebSearch result summaries were available. The shared WebSearch budget for this turn (200 calls across all agents) ran out after 14 searches by this agent.
> - **Every number below that is not Semrush MCP data is labeled [Schätzung].** Each comes from a WebSearch summary of a third-party page, is undated or loosely dated, and has not been checked against the page itself.

## Q1: Can the Semrush MCP be used for keyword and traffic metrics?

### Takeaway
No. The account has no API units for Keyword/Competitive Research and no plan with MCP access to Traffic Analytics, so none of the requested Semrush report data exists (see the status box above). Getting the data needs more API units at https://www.semrush.com/mcp-access and a plan for Traffic Analytics (https://www.semrush.com/analytics/traffic/trends-api).

### Cited Findings
- `keyword_research` returned `no_api_units`, `retryable: false`. Source: Semrush MCP tool response, trace_id 6e0deb9dd17329d984c8bfb0e87554ac — [Semrush MCP access](https://www.semrush.com/mcp-access)
- `competitors_research` returned `no_api_units`, `retryable: false`. Source: Semrush MCP tool response, trace_id 79f30194bbd42f02a93a7172e4499102 — [Semrush MCP access](https://www.semrush.com/mcp-access)
- `traffic_overview` returned `no_subscription`, `retryable: false`. Source: Semrush MCP tool response, trace_id 10e4100d579d339ae8456376455faadd — [Semrush Traffic API](https://www.semrush.com/analytics/traffic/trends-api)

### Inferences
- Because all three discovery calls failed, the requested columns (volume, KD, CPC, competition, US and UK databases, traffic) are "keine Daten" throughout. Rerunning the same plan after units are added needs no change to the requests (the errors' hint: "the request itself needs no changes").

### Gaps
- Not tested: `domain_overview` and `organic_research`. They were not called because of the instruction to stop after the first `no_api_units`/`no_subscription`. They probably draw on the same unit pool.

## Q2: Keyword metrics per niche (seed terms + 10–15 related terms)

### Takeaway
No Semrush data for any niche. Public proxies turned up figures for only two areas. COI tracking: "certificate of insurance tracking" at about 210 searches/month with a CPC of about $10 [Schätzung]. Frame.io: the brand term at about 110K searches [Schätzung], not the "alternative" query. For the other 6 niches, and for every related/phrase-match list, there are no data.

Legend: **Vol** = monthly search volume, **KD** = keyword difficulty, **CPC** in USD, **Comp** = competition. "keine Daten" = no data. Semrush report/DB for every cell: none, because Semrush could not be used (Q1).

### Cited Findings

#### Niche 1: Video delivery paywall for freelance editors (DB us)
| Keyword | Vol | KD | CPC | Comp | Source / report / DB |
|---|---|---|---|---|---|
| frame.io alternative | keine Daten | keine Daten | keine Daten | keine Daten | no source found |
| client video review software | keine Daten | keine Daten | keine Daten | keine Daten | – |
| video review and approval | keine Daten | keine Daten | keine Daten | keine Daten | – |
| watermark video for client | keine Daten | keine Daten | keine Daten | keine Daten | – |
| video delivery platform | keine Daten | keine Daten | keine Daten | keine Daten | – |
| how to get paid for video editing | keine Daten | keine Daten | keine Daten | keine Daten | – |
| pixieset video | keine Daten | keine Daten | keine Daten | keine Daten | – |
| *(proxy)* "Frame.io" brand topic | 110K "search volume", growth +286% [Schätzung] | keine Daten | keine Daten | keine Daten | Exploding Topics' own metric. Region and date not stated (topic "discovered May 13th 2020") — [Exploding Topics](https://explodingtopics.com/topic/frameio?period=120) |

- Qualitative demand signal: Fast.io writes that since Adobe bought Frame.io, many teams have started looking at independent alternatives. This is a vendor's own content, so it is self-interested — [Fast.io](https://fast.io/resources/frame-io-alternative/)
- G2's small-business list of Frame.io alternatives puts iconik first and names Ziflow, Wistia, Filestage and Loom as similar tools — [G2](https://www.g2.com/products/frame-io/competitors/alternatives/small-business)
- Two pages with near-identical spun text about a "cheaper Frame.io alternative" turned up. They are not usable evidence — [houstonsfirst](https://live.houstonsfirst.org/?p=52827), [jturnerresearch](https://v9-albert.jturnerresearch.com/?p=35218)

#### Niche 2: Captions for local-government meeting videos, ADA Title II (DB us)
| Keyword | Vol | KD | CPC | Comp | Source / report / DB |
|---|---|---|---|---|---|
| ada title ii | keine Daten | keine Daten | keine Daten | keine Daten | – |
| ada title ii website compliance | keine Daten | keine Daten | keine Daten | keine Daten | – |
| closed captioning services | keine Daten | keine Daten | keine Daten | keine Daten | – |
| captioning services for government | keine Daten | keine Daten | keine Daten | keine Daten | – |
| meeting minutes software | keine Daten | keine Daten | keine Daten | keine Daten | – |
| board meeting transcription | keine Daten | keine Daten | keine Daten | keine Daten | – |

Demand driver (regulatory facts, not keyword metrics):
- DOJ Title II web rule deadlines: April 24, 2026 for public entities serving a population of 50,000 or more, and April 26, 2027 for entities under 50,000 and special districts — [Venable, 04/2026](https://www.venable.com/insights/publications/2026/04/ada-title-ii-website-accessibility-regulations); [SBA Office of Advocacy, 2024-04-25](https://advocacy.sba.gov/2024/04/25/justice-department-finalizes-rule-requiring-state-and-local-governments-to-make-their-websites-accessible/). **Conflict:** CivicPlus gives April 26, 2028 for entities under 50,000 and for special districts — [CivicPlus](https://www.civicplus.com/blog/wa/ada-updates-101/)
- The rule adopts WCAG 2.1 AA, which requires captions for live and prerecorded video — [AI-Media](https://www.ai-media.tv/knowledge-hub/insights/ada-title-ii-goes-digital-what-public-entities-need-to-know/); [3Play Media](https://3playmedia.com/blog/ada-update-final-rule-a-clearer-picture-for-captioning-and-audio-description-in-higher-education)
- The rule covers content "provided or made available" by a public entity, including content that a contractor or vendor delivers — [AI-Media](https://www.ai-media.tv/knowledge-hub/insights/ada-title-ii-goes-digital-what-public-entities-need-to-know/)
- Competitors are moving. AI-Media launched an "ADA Title II Compliance Initiative" aimed at public entities — [Bernama press release](https://web11.bernama.com/en/press/news.php?id=2498273); 3Play Media publishes Title II content — [3Play Media](https://www.3playmedia.com/blog/ada-video-requirements)

#### Niche 3: COI tracking (DB us)
| Keyword | Vol | KD | CPC | Comp | Source / report / DB |
|---|---|---|---|---|---|
| coi tracking software | keine Daten | keine Daten | keine Daten | keine Daten | no source found |
| certificate of insurance tracking | ~210 [Schätzung] | keine Daten | ~$10.07 [Schätzung] | keine Daten | iSpionage competitor page for ebix.com (CertsOnline). Undated, region not stated, Ebix at avg. position ~7.5 — [iSpionage](https://www.ispionage.com/Competitive_Intelligence_directory/e/66/ebix_com_656269782E636F6D) |
| *(related)* certificate of insurance tracking software | ~30 [Schätzung] | keine Daten | ~$11.35 [Schätzung] | keine Daten | same iSpionage page |
| *(related)* insurance certificate tracking | ~70 [Schätzung] | keine Daten | ~$8.85 [Schätzung] | keine Daten | same iSpionage page |
| subcontractor insurance tracking | keine Daten | keine Daten | keine Daten | keine Daten | – |
| vendor insurance compliance software | keine Daten | keine Daten | keine Daten | keine Daten | – |
| mycoi | keine Daten | keine Daten | keine Daten | keine Daten | – |

- TrustLayer's own marketing (llms.txt) claims customers rank it ahead of myCOI, Jones and BCS on ease of use, support and ROI. This is a self-reported claim — [TrustLayer llms.txt](https://www.trustlayer.io/llms.txt); TrustLayer also runs a comparison page against myCOI — [TrustLayer vs myCOI](https://trustlayer.io/pages/trustlayer-vs-mycoi)
- Certificial's blog says TrustLayer offers access to "298,000+ companies" (citing TrustLayer's website). Unverified, and written by a competitor — [Certificial](https://certificial.com/blog-post/trustlayer-alternatives)
- Apps Run The World estimates TrustLayer's customers split 50% companies with 0–100 employees and 50% with 101–1,000 employees — [Apps Run The World](https://www.appsruntheworld.com/customers-database/products/view/trustlayer)
- myCOI serves commercial and residential construction, real estate, property management, manufacturing, retail, transportation, utilities and government — [CB Insights](https://www.cbinsights.com/compare/mycoi-vs-trustlayer)
- BCS (getbcs.com) has a public "COI Tracker – Plans & Pricing" page. The price figures did not come through in the search — [BCS pricing](https://getbcs.com/pricing)

#### Niche 4: Creator sponsorship tracker (DB us)
| Keyword | Vol | KD | CPC | Comp | Source / report / DB |
|---|---|---|---|---|---|
| brand deal tracker | keine Daten | keine Daten | keine Daten | keine Daten | – |
| sponsorship tracker | keine Daten | keine Daten | keine Daten | keine Daten | – |
| influencer invoice template | keine Daten | keine Daten | keine Daten | keine Daten | – |
| creator crm | keine Daten | keine Daten | keine Daten | keine Daten | – |
| youtube sponsorship rates | keine Daten | keine Daten | keine Daten | keine Daten | – |

#### Niche 5: Music cue sheets (DB us)
| Keyword | Vol | KD | CPC | Comp | Source / report / DB |
|---|---|---|---|---|---|
| music cue sheet | keine Daten | keine Daten | keine Daten | keine Daten | searched; no source found |
| cue sheet template | keine Daten | keine Daten | keine Daten | keine Daten | – |
| cue sheet software | keine Daten | keine Daten | keine Daten | keine Daten | – |
| ascap cue sheet | keine Daten | keine Daten | keine Daten | keine Daten | – |
| bmi cue sheet | keine Daten | keine Daten | keine Daten | keine Daten | – |

- Orfium (a rights-management firm) has a public FAQ that touches on cue sheets. This shows only that the topic exists, not how big the demand is — [Orfium FAQ](https://orfium.com/frequently-asked-questions)

#### Niche 6: RFP alerts for video production (DB us)
| Keyword | Vol | KD | CPC | Comp | Source / report / DB |
|---|---|---|---|---|---|
| video production rfp | keine Daten | keine Daten | keine Daten | keine Daten | – |
| government rfp alerts | keine Daten | keine Daten | keine Daten | keine Daten | – |
| rfp finder | keine Daten | keine Daten | keine Daten | keine Daten | – |
| bid alerts | keine Daten | keine Daten | keine Daten | keine Daten | – |
| government contracts for video production | keine Daten | keine Daten | keine Daten | keine Daten | – |

#### Niche 7: Contract renewal tracker (DB us)
| Keyword | Vol | KD | CPC | Comp | Source / report / DB |
|---|---|---|---|---|---|
| contract renewal tracking | keine Daten | keine Daten | keine Daten | keine Daten | – |
| contract management software small business | keine Daten | keine Daten | keine Daten | keine Daten | – |
| saas renewal tracker | keine Daten | keine Daten | keine Daten | keine Daten | – |
| contract expiration tracking | keine Daten | keine Daten | keine Daten | keine Daten | – |

#### Niche 8: UK landlord compliance (DB uk)
| Keyword | Vol | KD | CPC | Comp | Source / report / DB |
|---|---|---|---|---|---|
| landlord compliance software | keine Daten | keine Daten | keine Daten | keine Daten | – |
| gas safety certificate reminder | keine Daten | keine Daten | keine Daten | keine Daten | – |
| eicr for landlords | keine Daten | keine Daten | keine Daten | keine Daten | – |
| landlord app | keine Daten | keine Daten | keine Daten | keine Daten | – |
| renters rights act landlord | keine Daten | keine Daten | keine Daten | keine Daten | – |

### Inferences
- COI tracking is the only niche with any CPC signal. About $9–11 CPC on small-volume terms (~30–210/month) [Schätzung] fits a B2B buyer with budget and a narrow, high-intent search pool. Because the source is undated and unverified, treat it as directional only.
- In niche 1, the Frame.io brand term is large (~110K [Schätzung]), so "frame.io alternative" plausibly has real volume. The size is unknown.
- In niche 2, demand is driven by the regulatory deadline rather than shown by keyword data. If the April 2027 tier stands, small municipalities and special districts (the likely micro-SaaS buyers) are now about 6 months from their deadline. The CivicPlus date of 2028 may reflect a later extension or may be an error. This is not verified, and the report writer must check it against DOJ/ada.gov before relying on any date.

### Gaps
- No Semrush data at all (US or UK) for any seed or related term. Every 10–15-term related/phrase-match list was never generated, because `phrase_related`/`phrase_fullsearch`-type reports were never reachable.
- Google autocomplete could not be queried (WebFetch DNS failure), so not even query-existence proxies exist.
- Niches 2, 4, 5, 6, 7 and 8: no public volume or CPC proxy found in the searches made before the search budget ran out.
- The iSpionage and Exploding Topics figures could not be opened to check date, region or methodology.

## Q3: Organic/total traffic of the top competitors

### Takeaway
No Semrush traffic data (`traffic_overview` returned `no_subscription`; `domain_overview` was not called). Public proxies gave one figure: frame.io at 11.67M visits in a March of an unstated year [Schätzung]. All other domains are "keine Daten". For UK landlord tools, Capterra review counts are the only adoption signal.

### Cited Findings
| Domain | Visits / organic traffic | Source / report / DB | Note |
|---|---|---|---|
| frame.io | 11.67M visits "in March" (year not stated), avg. session duration 10:23 [Schätzung] | Semrush **public website page** (not the MCP; seen only as a search snippet) — [semrush.com/website/frame.io](https://semrush.com/website/frame.io/overview) | Similarweb's company page did not show a number in the snippet — [Similarweb](https://www.similarweb.com/company/frame.io) |
| pic-time.com | keine Daten | – | Product: online galleries, print store and marketing automation for pro photographers. Partnership with HoneyBook — [Pic-Time help](https://help.pic-time.com/en/articles/8531313-pic-time-and-honeybook-partnership) |
| rev.com | keine Daten | – | search budget ran out before this domain was searched |
| 3playmedia.com | keine Daten | – | same |
| mycoi.com | keine Daten | – | the search returned myco.io, an unrelated domain, instead — [Ahrefs](https://ahrefs.com/websites/myco.io) (not used) |
| trustlayer.io | keine Daten | – | – |
| getbcs.com | keine Daten | – | Similarweb shows "no data" only for bcsllc.com, which may be a different domain — [Similarweb](https://www.similarweb.com/company/bcsllc.com) |
| passionfroot.me | keine Daten | – | no results mention Passionfroot |
| rightstrack.com | keine Daten | – | no results mention RightsTrack |
| rfpmart.com | keine Daten | – | search budget ran out |
| bidprime.com | keine Daten | – | search budget ran out |
| contractsafe.com | keine Daten | – | search budget ran out |
| landlordvision.co.uk | keine Daten | – | Capterra: 5.0/5 from only 2 reviews — [Capterra UK](https://www.capterra.co.uk/software/156512/landlord-vision) |
| landlordstudio.com | keine Daten | – | Capterra: 147 reviews, 4.9/5, has a free version — [Capterra comparison](https://www.capterra.co.il/compare/145260/182473/arthur-online/vs/landlord-studio). Positions itself as the "Arthur Online alternative" for self-managing landlords — [Landlord Studio](https://www.landlordstudio.com/uk/comparison/arthur-online) |
| arthuronline.co.uk | keine Daten | – | Capterra: 16 reviews, 3.9/5, aimed at portfolios of 25–300 units — [Capterra comparison](https://www.capterra.co.il/compare/145260/182473/arthur-online/vs/landlord-studio) |

### Inferences
- frame.io's ~11.67M monthly visits [Schätzung] put it orders of magnitude above every other domain on the list. A niche "delivery paywall for freelancers" would be competing on long-tail "alternative" terms, not on Frame.io's core terms.
- UK landlord tools: Landlord Studio's ~9x more Capterra reviews than Arthur Online (147 vs 16) suggests stronger traction among small, self-managing landlords. Arthur targets larger portfolios (25–300 units). Review counts are a weak proxy for users.

### Gaps
- No traffic, organic traffic or organic keyword counts for 14 of 15 domains. None of the 15 domains is confirmed as non-existent; the data is simply missing.
- No customer counts found for myCOI, TrustLayer (only an unverified third-party "298,000+ companies" claim), BCS, Pic-Time, Passionfroot, RightsTrack, RFPMart, BidPrime, ContractSafe, Rev, 3Play, Landlord Vision, Landlord Studio or Arthur.
- To close these gaps: add Semrush API units and a Traffic Analytics plan (URLs in the status box), or run a follow-up turn with fresh web-search budget and working WebFetch.
