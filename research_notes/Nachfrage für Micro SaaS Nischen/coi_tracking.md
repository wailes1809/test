# COI (Certificate of Insurance) Tracking Software for Small GCs, Specialty Contractors and Small Property Managers — Market Research Notes (as of 2026-10-15)

> **Method caveat (applies to all sections):** WebFetch failed with DNS errors for every domain tried (getbcs.com, subdoc.io, coisoftware.com, trackmyvendor.com, census.gov). The search tool also blocks reddit.com, and the shared web-search budget ran out before I finished. So every finding below comes from search-engine result summaries of the cited pages; I did not read any page in full. Most pricing figures come from **vendor-written comparison blogs** (SubDoc, COI File, TrackMyVendor, COISoftware, bcs, Certificial, Billy), which have a commercial bias. Re-check every price on the vendor's own pricing page before relying on it. Where a source's date was not visible, it says "date n/a".

## 1. Demand signals: do small contractors and property managers complain about COI tracking and pay to solve it?

### Takeaway
The pain shows up repeatedly in forums: spreadsheets, file folders, renewals slipping through the cracks, and whole days spent chasing subs for new COIs. But I could not collect direct Reddit quotes because the tool blocks Reddit. The strongest "paying demand" signal is indirect: in 2025–2026 at least 10 small self-serve COI tools appeared, all pricing at $12–$199/mo, and funded players added free tiers to defend the low end.

### Cited Findings
**Forum and community complaints (secondhand, from search summaries):**
- ContractorTalk thread "Software for managing Subcontractor Certs of Insurance & associated sub data" (date n/a). The original poster manages about 40–50 active subs with "a spreadsheet and file folders and it is becoming quite burdensome and we are having issues with details falling through the cracks". They want to enter expiration dates and have the software flag them. — [ContractorTalk](https://www.contractortalk.com/threads/software-for-managing-subcontractor-certs-of-insurance-associated-sub-data.264865/)
- QuickBooks Community thread "Is there a way to track when Certificates of insurance expires for vendors that are subcontractors?" (date n/a). A reply suggests the workaround: "you can add the expiration date in the Notes section of the vendor's profile". QuickBooks Desktop has WC/GL expiration-date fields on the vendor record. — [QuickBooks Community](https://quickbooks.intuit.com/community/reports-and-accounting-5/is-there-a-way-to-track-when-certificates-of-insurance-expires-for-vendors-that-are-subcontractors-40576)
- Reddit anecdote, retold secondhand by a vendor blog: a project coordinator who inherited a sub-insurance spreadsheet says they "spend their entire day chasing subs over email to get new COIs before one expires". The blog says experienced construction managers replied that this is how most companies do it. The source is promotional (imagetotable.ai sells COI-to-Excel extraction), date n/a. — [imagetotable.ai blog](https://imagetotable.ai/blog/batch-subcontractor-coi-tracking-general-contractor)
- The same vendor blog describes the spreadsheet as "free and adequate with eight subs, but a bottleneck at thirty and a liability at fifty". Opinion, vendor-authored. — [imagetotable.ai](https://imagetotable.ai/blog/batch-subcontractor-coi-tracking-general-contractor); see also [imagetotable.ai COI→Excel](https://imagetotable.ai/blog/certificate-of-insurance-data-extraction-excel)
- BiggerPockets thread "How do you handle insurance for your contractors?" is about 14 years old (~2012) and thin. Advice given: "Ask for liability insurance, as the contractor for a copy of theirs and look at the expiration date." — [BiggerPockets](https://www.biggerpockets.com/forums/52/topics/77235-how-do-you-handle-insurance-for-your-contractors)
- BiggerPockets thread "Best way to track tenant renters insurance at scale? (AppFolio)" (date n/a) shows an adjacent pain: tenant insurance tracking rather than vendor COIs. — [BiggerPockets](https://www.biggerpockets.com/forums/52/topics/1276812-best-way-to-track-tenant-renters-insurance-at-scale-appfolio)
- Vendor guides claim "60% of small GCs" use spreadsheets and that "fewer than half have a system that tells them when that certificate expires". These figures are unsourced vendor claims; do not treat them as data. — [TrackMyVendor guide](https://trackmyvendor.com/resources/how-to-track-subcontractor-insurance); [Workhand blog](https://workhand.app/blog/track-subcontractor-insurance-certificates/)
- Property-management guides note that vendors and tenants sometimes resubmit old certificates when chased for renewals, so the issue date matters as well as the expiry date. — [Rioo blog](https://riooapp.com/blog/coi-tracking-vendor-insurance-property-managers); [Vantage Point Risk](https://vantagepointrisk.com/learning-center/coi-tracking-for-property-managers/) (the summary did not say which of the two made this point)

**Supply-side signals (others are building and selling this):**
- Many small, self-serve COI tools publish prices and comparison blogs dated 2026: SubDoc, TrackMyVendor, COI File, COISoftware, COIPulse, CertShield, VendorProof, VendorJot, Workhand, Rioo, ExpirationReminder, imagetotable.ai, ConCoi. — [SubDoc list](https://subdoc.io/blog/affordable-coi-tracking-software); [COI File](https://coifile.com/coi-tracking/best-software/); [TrackMyVendor](https://trackmyvendor.com/compare-coi-tracking-software); [ConCoi](https://concoi.com/certificate-of-insurance-tracking-software/); [ExpirationReminder](https://www.expirationreminder.com/blog/how-expired-cois-put-your-company-at-financial-risk)
- An Indie Hackers post titled "Best COI Tracking Software 2026: I Compared 10 Platforms and Ranked Every Option for Vendor Insurance Compliance" suggests indie founders are already marketing in this niche. — [Indie Hackers](https://www.indiehackers.com/post/best-coi-tracking-software-2026-i-compared-10-platforms-and-ranked-every-option-for-vendor-insurance-compliance-0c694b2679)
- An Apify actor, "COI Tracking – Certificate Expiry Alerts" by armourylabs, exists as a micro-tool. — [Apify](https://apify.com/armourylabs/subcontractor-certificate-expiry-checker)
- A £4.99 Gumroad Excel "Construction Insurance Tracker" exists, though it tracks the buyer's own policies rather than subs' COIs. — [Gumroad siteready](https://siteready.gumroad.com/l/wsbhkx)
- TrustLayer launched a free "Starter" tier for up to 50 vendors in August 2025 (per a competitor's comparison page). — [COI File vs TrustLayer](https://coifile.com/compare/trustlayer-alternative/)

### Inferences
- The pain is real and recurring: expiry dates, chasing renewals, and audit exposure. The problem is not demand but **saturation at the low end**. In 2026 a newcomer competes with free tiers (TrustLayer 50 vendors, bcs 25, TrackMyVendor 25) and a $20/mo floor (SubDoc). [Schätzung]
- The buyer with the most pain is the firm with roughly 20–100 active subs or vendors. Below about 10, a spreadsheet works; above about 100, buyers move to managed or enterprise tools. [Schätzung, based on the ContractorTalk OP's 40–50 subs and the vendor blog's 8/30/50 thresholds]
- Forum threads are mostly old (BiggerPockets ~2012), and the "Reddit" evidence is secondhand. Direct 2024–2026 Reddit validation is still open.

### Gaps
- **Direct Reddit quotes (r/Construction, r/Contractor, r/PropertyManagement, r/smallbusiness, r/Insurance):** not collected, because reddit.com is blocked for this search tool. Target of 5+ dated quotes not met: I found 4 forum/community signals plus 1 secondhand Reddit anecdote, mostly undated or old.
- No dated 2024–2026 forum posts found that mention a willingness-to-pay figure.
- Reply content of the ContractorTalk and QuickBooks threads (which tools people recommend) was not visible.

## 2. Competitors and their (lowest) prices; who is the cheapest self-serve option?

### Takeaway
Self-serve prices cluster between free and about $199/mo. Based on published 2026 figures (mostly self-reported by vendors), the cheapest options are **SubDoc ($20/mo for up to 100 vendors)**, **VendorProof (from $12/mo, 10 vendors free)** and **bcs ($0.95/active vendor/mo, 25 free)**. Free tiers go up to **50 vendors (TrustLayer Starter)**. Enterprise players (myCOI/illumend, Jones, Billy, SmartCompliance, PINS, TrustLayer paid) don't publish prices and need a demo or sales call. Procore and Buildium already include basic expiry tracking.

### Cited Findings
**Cheap, self-serve tools (published prices, mostly from vendor blogs):**
- **SubDoc:** free for up to 3 vendors, then **$20/month for up to 100 vendors**, with no setup fee and no annual minimum. It claims to be "the cheapest verified option" based on published pricing as of September 2026 (self-claim). — [SubDoc](https://subdoc.io/blog/affordable-coi-tracking-software); [SubDoc chooser](https://subdoc.io/blog/which-coi-tracking-software-should-you-choose)
- **VendorProof:** free tier for 10 vendors with all features, paid from **$12/month** (paid-tier vendor limit not found). Directory listing, date n/a. — [AlternativeTo VendorProof](https://alternativeto.net/software/vendorproof/about)
- **bcs (getbcs.com):** free up to 25 vendors. Self-service is **$0.95 per active vendor per month** ($11.40/vendor/yr). Full-service is $17.80/vendor/yr with a **$10K annual minimum** (the minimum comes from a third-party comparison). — [bcs pricing page](https://www.getbcs.com/pricing-and-plans) (seen only in search results); [Docsumo comparison 2026](https://www.docsumo.com/blog/best-coi-tracking-software); [bcs alternatives](https://www.getbcs.com/alternatives)
- **TrackMyVendor:** free for 25 subs; **$39/mo** for unlimited subs with 2 users; **$59/mo** for unlimited subs and unlimited team members. — [TrackMyVendor comparison 2026](https://trackmyvendor.com/compare-coi-tracking-software)
- **COI File:** Base **$39/mo** (up to 10 vendors), Growth $89/mo (up to 50), Pro $199/mo (unlimited). — [COI File 2026](https://coifile.com/coi-tracking/best-software/); [COI File free tools](https://coifile.com/blog/best-free-coi-tracking-tools/)
- **COISoftware:** Starter $49/mo and Plus $149/mo, or $24 and $74/mo billed yearly. — [COISoftware pricing 2026](https://coisoftware.com/coi-tracking-software-pricing)
- **COIPulse:** paid plan $49/month. **CertShield:** paid plans from $99/month. These come from the same search result set; the summary did not say which comparison page listed them, most likely [SubDoc list](https://subdoc.io/blog/affordable-coi-tracking-software) or [COISoftware pricing](https://coisoftware.com/coi-tracking-software-pricing).
- **Certificial:** free for up to 5 vendors (suppliers); "Professional from $99 per month" with unlimited suppliers. Some sources describe the paid tier as custom-priced instead. — [Certificial blog 2026](https://www.certificial.com/blog-post/we-compared-7-best-coi-tracking-software-in-depth-feedback-and-review); [Indie Hackers comparison](https://www.indiehackers.com/post/best-coi-tracking-software-2026-i-compared-10-platforms-and-ranked-every-option-for-vendor-insurance-compliance-0c694b2679)
- **COI Pro** is listed on Capterra (price not captured). — [Capterra COI Pro](https://www.capterra.com/p/208128/COI-Pro/)

**Enterprise / sales-led (no public price):**
- **TrustLayer:** free Starter tier up to 50 vendors since August 2025; upgrade pricing not public and requires a sales call (per competitor COI File). Directory listings conflict: Capterra shows "$29 Flat Rate, Per Month", Software Advice shows "Starting at $25000.00 per year", SelectHub estimates $1,000+. — [COI File vs TrustLayer](https://coifile.com/compare/trustlayer-alternative/); [Capterra](https://www.capterra.com/p/198486/TrustLayer/); [Software Advice](https://www.softwareadvice.com/compliance/trustlayer-profile/); [SelectHub](https://www.selecthub.com/p/risk-management-software/trustlayer/); [G2 says pricing n/a](https://www.g2.com/products/trustlayer/reviews)
- **myCOI (now illumend):** pricing not published. One review mentions a 60-day risk-free trial; another claims tiers "starting around $200–400/month" (unverified). — [COISoftware: myCOI pricing](https://coisoftware.com/blog/mycoi-pricing); [Certificial: myCOI alternatives 2026](https://www.certificial.com/blog-post/best-mycoi-alternatives-2026)
- **Jones (getjones.com):** custom enterprise pricing based on user count and integrations; one review says you need a sales conversation before you can access the platform. Per-certificate price not found. — [Docsumo 2026](https://www.docsumo.com/blog/best-coi-tracking-software); [bcs: top COI companies](https://www.getbcs.com/blog/top-certificate-of-insurance-tracking-companies)
- **Billy (billyforinsurance.com):** pricing is "consultative", not a public list, and depends on vendor volume, service level, integrations and feature tier; you request a demo for custom pricing. Software Advice lists "starting at $500.00 per year" but also "available upon request" (unverified). Integrates with Procore, Autodesk, Viewpoint Vista, CMiC, DocuSign and Sage 300. — [Billy FAQ](https://billyforinsurance.com/resources/faq/); [Software Advice Billy](https://www.softwareadvice.com/insurance/billy-profile/); [CB Insights Billy vs myCOI](https://www.cbinsights.com/compare/billy-4-vs-mycoi)
- **SmartCompliance:** pricing not published. Capterra lists a $1,000/year starting price; SubDoc estimates about $1,800+/yr. — [Capterra SmartCompliance](https://www.capterra.com/p/189672/SmartCompliance/); [SubDoc](https://subdoc.io/blog/affordable-coi-tracking-software)
- **PINS Advantage:** volume tiers tied to annual COI count; SelectHub estimates $1,000+/yr. Slashdot lists $85/$115/$150 per user per month, which conflicts with sources saying all plans include unlimited users. — [Billy: PINS pricing](https://billyforinsurance.com/resources/resources-pins-advantage-pricing-reviews-alternatives/); [Slashdot](https://slashdot.org/software/comparison/Certificial-vs-Pins-Advantage/)
- **CertFocus (Vertikal RMS):** one comparison says it publishes $6–8 per vendor with a **$7,500 minimum**; a Vertikal RMS estimate of $40–80 per vendor also appears. — From the "COI tracking software pricing" search set ([COISoftware pricing](https://coisoftware.com/coi-tracking-software-pricing) / [SubDoc list](https://subdoc.io/blog/affordable-coi-tracking-software)); [Vertikal RMS 2026](https://www.vertikalrms.com/article/best-coi-tracking-software-2026-top-coi-platforms-for-contractors/)
- Enterprise platforms such as myCOI, Jones and TrustLayer "typically start at $500–2,000+/month with annual contracts". This is a third-party estimate in a vendor blog. — [COISoftware pricing](https://coisoftware.com/coi-tracking-software-pricing) / [SubDoc list](https://subdoc.io/blog/affordable-coi-tracking-software) (search summary)
- **Constrafor:** offers a free universal prequalification form, free for subs. A competitor (Billy) says it is a prequal intake tool attached to a finance product, not a pure COI tracker. Constrafor does have a COI page. — [Billy vs Constrafor](https://billyforinsurance.com/resources/billy-vs-constrafor-prequalification/); [Constrafor COI page](https://www.constrafor.com/coi-certificates-of-insurance)
- **Others seen:** Docutrax (outsourced programs; selected by ProSight Specialty Insurance for its sub-compliance program, date n/a), HoundDog, TradeGuard, ConCoi. — [BioSpace/Docutrax](https://www.biospace.com/docutrax-selected-to-oversee-new-subcontractor-compliance-program-of-prosight-specialty-insurance); [SourceForge AU list](https://sourceforge.net/software/certificate-of-insurance-coi-tracking/australia/)

**Built-in features of PM and construction suites:**
- **Procore:** insurance data lives in the Company Directory. Automated emails go to the company's insurance manager starting two weeks before expiry and continue daily for up to 60 days after expiry or until the date is updated. Critics who sell add-ons say: "Procore stores it; it does not check it." — [Procore support FAQ](https://support.procore.com/faq/who-receives-notification-emails-when-a-vendors-insurance-expires); [Procore tutorial](https://support.procore.com/products/online/user-guide/company-level/directory/tutorials/update-expiring-insurance-for-a-vendor-in-the-company-directory); [Billy on Procore](https://billyforinsurance.com/resources/how-to-track-cois-in-procore/); [PINS on Procore](https://www.pinsadvantage.com/resources/blog/coi-tracking-in-procore); [COISoftware on Procore](https://coisoftware.com/blog/can-you-track-certificates-of-insurance-in-procore)
- **Buildium:** vendor records hold the insurance provider, policy number and expiry date. When notifications are on, it flags vendors with missing or expired insurance, and an expiry notice appears on the Vendor page starting 90 days before expiry. — [Buildium Help](https://help.buildium.com/hc/s/article/Tracking-Vendor-Insurance-1557495330433)
- **QuickBooks Desktop:** WC and GL expiration-date fields on the vendor record (per a community reply). — [QuickBooks Community](https://quickbooks.intuit.com/community/reports-and-accounting-5/is-there-a-way-to-track-when-certificates-of-insurance-expires-for-vendors-that-are-subcontractors-40576)
- **AppFolio, Yardi, Buildertrend:** no official source found on vendor-COI features. One third-party mention says Buildertrend receives "sub and vendor documents, expiry alerts" (weak). — [Exotica IT blog](https://ai.exoticaitsolutions.com/blog/construction-compliance-automation)

### Inferences
- **Price floor:** about $0–20/mo for up to 100 vendors. A new entrant cannot win on price alone. [Schätzung]
- **Cost comparison (my arithmetic):** for 40 subs, bcs self-serve costs 40 × $0.95 = $38/mo, compared with SubDoc $20, TrackMyVendor $39 and COI File Growth $89. For 100 subs, bcs costs $95/mo. [Rechnung]
- **Possible gaps:**
  - A "done-for-you" service at small-business prices. bcs full-service has a $10K minimum, so a small firm cannot buy it.
  - Vertical focus, for example property managers on AppFolio, or one trade.
  - A non-English-US market such as AU "certificates of currency".
  - Deeper checks, for example additional-insured endorsement review.

  [Schätzung]
- Procore and Buildium users already get basic expiry reminders, so the pitch to them has to go beyond dates. Firms on QuickBooks and spreadsheets are the more natural target. [Schätzung]

### Gaps
- **Evident:** no pricing or details found.
- **Yardi and AppFolio vendor-COI features:** no official source found.
- **Jones:** per-certificate pricing not found.
- **Exact contract terms** (monthly vs annual) for SubDoc, TrackMyVendor, COI File and VendorProof were not visible. Only SubDoc's "no annual minimum" claim was captured.
- **G2/Capterra review texts with price mentions** were not retrieved (WebFetch failed).
- **Verification:** no price was checked on the live pricing page itself (WebFetch DNS failure).

## 3. Cost of non-compliance: premium-audit charges and liability

### Takeaway
At a workers' comp or GL premium audit, carriers commonly treat what you paid a sub with no valid COI as your own payroll and charge premium on it. A vendor's worked example gives **$6,400 extra premium on one $80,000 uninsured drywall sub**. Some states (for example FL, NC, GA) make the GC liable for an uninsured sub's employees' workers' comp benefits.

### Cited Findings
- **Travelers:** a carrier may charge premium for a sub's work when no valid workers' comp certificate exists. A valid certificate shows policy type, carrier, policy number, term and insured sub, with your company as certificate holder. — [Travelers Premium Audit](https://www.travelers.com/business-insurance/services/premium-audit/workers-compensation-premium-audit)
- **State Farm:** if no certificate is available at audit, the sub's total cost may be added to your payroll. — [State Farm Premium Audits](https://www.statefarm.com/small-business-solutions/insurance/premium-audit)
- **Builders Mutual:** under an ISO payroll-inclusion rule, certain sub types such as temp agencies and leased employees are treated as uninsured on GL audits even when they carry coverage. — [Builders Mutual blog](https://blog.buildersmutual.com/questions-about-your-workers-comp-audit-we-have-answers)
- **Contractors Insured (2026 guide):** a certificate you cannot locate at audit counts the same as one you never collected. — [Contractors Insured](https://contractorsinsured.net/blog/subcontractor-insurance-requirements/)
- **Worked example (vendor blog):** an $80,000 uninsured drywall sub at $8 per $100 of payroll means a **$6,400** charge. Rules vary by insurer, policy and state. — [VendorJot](https://www.vendorjot.com/blog/insurance-audit-subcontractors-workers-comp-general-liability)
- **TrackMyVendor:** common audit problems are expired certificates, payee names that don't match, and limits below what the policy requires. Workers' comp is often the bigger charge. — [TrackMyVendor GL audit](https://trackmyvendor.com/resources/general-liability-premium-audit-subcontractors)
- **Other carrier and agency pages on the same topic** (content not extracted): [Midwestern Insurance Alliance](https://midwesterninsurance.com/policyholders/wc/premiumaudit/); [State Fund CA](https://www.statefundca.com/policyholder/independent-contractor/employment-status-and-your-audit/); [Sadler & Co.](https://www.sadlerco.com/industries/builders-contractor-insurance/not-collecting-coi-from-insured-subs/)
- **Florida:** Statute §440.10 can make a contractor liable for workers' comp benefits for employees of a sub that has not secured coverage. — via search summary of [Grit Insurance](https://gritinsurance.com/blog/subcontractor-insurance-gaps-general-contractor) / [MKPA Law, 2026-04](https://www.mkpalaw.com/blog/2026/04/can-you-be-liable-for-an-uninsured-subcontractor/)
- **North Carolina:** the GC must obtain a certificate from the sub; if the sub can't provide one, the GC must secure workers' comp benefits for the sub's employees. — [Wilder Law Group](https://www.wilderlawgroup.com/nc-sc-injured-workers/independent-contractors/)
- **Statutory-employer rules:** "most states" have such laws making the GC responsible for workers' comp when an uninsured sub's employee is hurt. In Georgia, the GC is liable to the same extent as the sub. Some states also allow tort suits against the GC. — [illumend guide](https://www.illumend.ai/post/a-guide-to-handling-subcontractors-that-do-not-have-insurance); [illumend 2026 requirements guide](https://www.illumend.ai/insurance-knowledge/subcontractor-insurance-requirements-guide) (search summary; exact attribution between these and MKPA uncertain)
- **Third-party injury claims:** plaintiffs "name everyone they can — the sub, your company, and possibly the property owner." — [Grit Insurance](https://gritinsurance.com/blog/subcontractor-insurance-gaps-general-contractor)
- **Policy cancellation:** a community post says carriers may cancel a policy over use of uninsured subs. — [Patch NJ](https://patch.com/new-jersey/springfield/bp--uninsured-subcontractors)
- **Other sources on the topic:** the South Carolina Workers' Compensation Commission has a "Lapse in Insurance" document (2020); content not extracted. — [SC WCC PDF](https://wcc.sc.gov/sites/wcc/files/Documents/Header/Verify_Coverage/Lapse_In_Insurance%20Updated%20REV.%204.16..20.pdf). See also [Next Insurance](https://www.nextinsurance.com/blog/subcontractor-insurance/); [Westfield](https://www.westfieldinsurance.com/about-us/articles/subcontractor-insurance-what-contractors-need-to-know-about-coverage-and-liability)

### Inferences
- **ROI pitch:** one missed COI on a mid-size sub (about $6,400 in the vendor example) costs more than 10–25 years of a $20–49/mo tool. That is a strong one-line sales argument, but the example comes from a vendor. [Schätzung]
- **Product requirements implied:**
  - Keep a historical record of the COI valid on each payment date, not just the current one, because what counts is what you can show at audit.
  - Match payee names to named insureds.
  - Check limits against requirements.

  [Schätzung]

### Gaps
- No independent statistic found for average premium-audit charges caused by missing COIs (only the vendor example).
- No named court case found in which a GC was held liable because a sub's COI was missing or expired.
- State-by-state statutory-employer rules beyond FL, NC and GA were not checked.

## 4. Market size: US (NAICS 236/238/531311) and Canada/UK/Australia

### Takeaway
US specialty trade contractors (NAICS 238) have about **591,000–595,000 private establishments** (BLS QCEW, Q4 2024–Q2 2025), and about **90% of them have fewer than 20 employees** (CPWR, CBP-based). Residential property managers (NAICS 531311) have about **60,800 establishments** (CBP 2023, via a third-party aggregator). I could not retrieve a NAICS 236 total or exact size-class tables. Australia has the same need under the name "certificate of currency". Direct UK and Canada evidence was not found.

### Cited Findings
- **BLS NAICS 238 private establishments:** 590,917 (Q3 2024), 591,663 (Q4 2024), 591,154 (Q1 2025, preliminary), 595,488 (Q2 2025, preliminary). — [BLS Industries at a Glance 238](https://www.bls.gov/iag/tgs/iag238.htm)
- **CPWR Data Bulletin, April 2026 (Census CBP-based):** 91.0% of construction payroll establishments were small (2014–2023). NAICS 238 specialty trade contractors: **90.2% had fewer than 20 employees**. The snippet does not make clear whether that figure is for 2023 or 2014–2023. Specialty trade contractors were 66.1% of nonemployer construction establishments. — [CPWR Data Bulletin Apr 2026](https://www.cpwr.com/wp-content/uploads/DataBulletin-April2026.pdf); mirror [CDC Stacks](https://stacks.cdc.gov/view/cdc/260010/cdc_260010_DS1.pdf)
- **CPWR Construction Chart Book, 7th ed. (2025):**
  - 81.7% of construction establishments employed 1–9 employees, accounting for 1.5M workers (2014–2023 average).
  - In 2023, establishments with 1–9 employees accounted for 16.6% of construction payroll ($96.6B).
  - Nonemployer establishments made up 78.1% of all construction establishments (2021).

  — [CPWR Chart Book 7th ed.](https://www.cpwr.com/wp-content/uploads/CPWR_Construction_Chart_Book-7th.pdf)
- **CBP 2023, NAICS 236210 (industrial building construction, one sub-industry only):** 3,380 establishments, of which 1,668 have fewer than 5 employees and 583 have 5–9. — [data.census.gov](https://data.census.gov/table?q=236210%3A+Industrial+building+construction)
- **2023 County Business Patterns** was released June 26, 2025 and uses 2017 NAICS. — [Census press release](https://www.census.gov/newsroom/press-releases/2025/2023-county-business-patterns.html)
- **2022 Economic Census:** the "Location of Construction Establishments by Employment Size" dataset exists (last updated 2025-03-04); figures not retrieved. — [data.gov catalog](https://catalog.data.gov/dataset/economic-census-construction-location-of-construction-establishments-by-employment-si-2022)
- **2017 Economic Census (via a secondary site, unverified):** about 648,000 specialty trade establishments. — [Contractor Industry News](https://contractorindustrynews.com/contractor-market-size-and-statistics) [2017 data]
- **NAICS 531311 Residential Property Managers:** **60,818 establishments and 536,933 employees (CBP 2023)** per a third-party industry profile. Another site lists "Total Companies 39,462" (companies, not establishments; year n/a). — [Vanta Insights 531311](https://vantainsights.com/industry/531311-residential-property-managers) (search-summary attribution); [NAICS.com 531311](https://www.naics.com/naics-code-description/?code=531311)
- **NARPM:** more than 5,300 members (press kit, about late 2024). A 2026 blog says membership "has hovered just under 6,000 for years". — [NARPM Press Kit](https://www.narpm.org/press-center/press-kit/); [Peter Lohmann blog](https://www.peterlohmann.com/blog/narpm-2-0)
- **Australia:**
  - A "certificate of currency" proves a policy is active on its issue date. Subcontractors usually need one before going on site, accepting a purchase order, renewing a trade licence or submitting an invoice. — [Bokis](https://bokis.com.au/insights/certificate-of-currency-insurance)
  - US "COI" and AU "certificate of currency" tracking are the same job under different names. — [Apify armourylabs](https://apify.com/armourylabs/subcontractor-certificate-expiry-checker)
  - AU subcontractor-management platforms list insurance and licence expiry tracking with reminders and an upload portal as core features. — [Built Simple AU 2026](https://builtsimple.com.au/blog/subcontractor-management-software-australia/); [SourceForge AU list](https://sourceforge.net/software/certificate-of-insurance-coi-tracking/australia/)
- **UK:** no UK-specific results. bcs lists the UK among its service areas. — [bcs construction COI](https://www.getbcs.com/construction-coi-tracking)

### Inferences
- About 533,000 NAICS 238 establishments have fewer than 20 employees (591,663 × 90.2%). This mixes BLS QCEW and CBP shares, so it is rough. [Schätzung]
- Many small specialty contractors are the subs who *send* COIs rather than collect them. The core buyers are GCs (NAICS 236), larger specialty contractors who sub out work, and PM firms (about 60.8k establishments). [Schätzung]
- Even 0.1% of roughly 600k US construction plus PM establishments is about 600 customers. At $30/mo that is about $18k MRR, more than enough for a solo founder; the challenge is distribution, not TAM. [Schätzung]

### Gaps
- **NAICS 236 totals and exact CBP/SUSB size-class tables** (1–4, 5–9, 10–19, 20–49) for 236, 238 and 531311 were not retrieved. The Census API was blocked by the proxy and the search budget ran out. Next step: data.census.gov table CB2300CBP, filtered to NAICS 236/238/531311.
- **Canada:** no data on COI usage, Statistics Canada counts or analogues such as WSIB clearance certificates. I could not search for it, so it is unverified.
- **UK:** no establishment counts and no evidence on whether "COI tracking" is a common practice or what it is called.
- **Australia:** no ABS establishment counts.

## 5. Technical and legal pitfalls: ACORD 25, AI/OCR extraction, liability of a "compliant" flag

### Takeaway
The ACORD 25 is explicitly "informational only". It cannot confer additional-insured (AI) status, which only the policy endorsement can, and courts generally side with the policy over the certificate. AI extraction of dates, limits and carriers is feasible, but layout, checkboxes, scanned faxes and free-text "Description of Operations" are known failure points, so a human-review fallback is needed. A tool that marks a COI "compliant" risks overstating what the certificate proves.

### Cited Findings
- **ACORD 25 disclaimer:** the certificate is informational and "does not affirmatively or negatively amend, extend or alter the coverage afforded by the policies below." Also: "If the certificate holder is an ADDITIONAL INSURED, the policy(ies) must be endorsed. A statement on this certificate does not confer rights to the certificate holder in lieu of such endorsement(s)." — [TDI ACORD 25 PDF](https://www.tdi.texas.gov/certificates/documentcr/s21357a.pdf); [NYC DYCD sample](https://www.nyc.gov/assets/dycd/downloads/pdf/Insurance-Sample-Package25.pdf)
- **Case law:** a law firm says the majority view holds that a certificate disclaiming changes won't alter the policy. It cites a Second Circuit decision that certificate terms are subordinate to the policy: a certificate "will not suffice to create insurance coverage if such coverage is precluded by the terms of the policy." — [Butler Weihmuller Katz Craig LLP](https://www.butler.legal/information-or-indemnity-do-certificates-of-insurance-grant-insured-status/)
- **Blanket AI endorsements:** these carry conditions that never appear on the certificate. ISO automatic-AI endorsement CG 20 34 07 04 grants AI status only "when required by written contract", so an unsigned contract can void the AI status the certificate implies. Advice: ask for the actual endorsement. — search summary of [Insurance Advocate (2011)](https://insurance-advocate.com/2011/11/14/acord-25-certificate-of-liability-insurance-has-changed-for-better-or-worse/) / [Wellesley guide](https://www1.wellesley.edu/sites/default/files/assets/certificates_how_to_read_and_review_with_acord_forms.pdf) (exact attribution between the two uncertain)
- **Disclaimer wording** differs across ACORD 25 editions (2009, 2014 and later). — [FormsBoss ACORD 25 (2014/01)](https://www.formsboss.com/help/acord-25.html); [Hawaii SPO 25S/25](https://spo.hawaii.gov/wp-content/uploads/2013/12/spo150AcordCertofInsurForms25_25s.pdf)
- **Certificate vs endorsement:** a certificate summarizes a policy and grants no rights; the endorsement amends coverage. — [Rioo](https://riooapp.com/blog/coi-tracking-vendor-insurance-property-managers); [Jones PM guide](https://getjones.com/blog/how-property-managers-verify-tenant-vendor-insurance-certificates/)
- **Fields to re-check:** a vendor guide recommends re-checking six fields per sub, including carrier, limits and additional-insured wording, with reminders about 30 and 14 days before expiry. — [Workhand](https://workhand.app/blog/track-subcontractor-insurance-certificates/) / [TrackMyVendor](https://trackmyvendor.com/resources/how-to-track-subcontractor-insurance) (search summary)
- **AI/OCR failure points:**
  - Plain LLM text parsing of ACORD forms can merge adjacent columns and attach a limit to the wrong coverage line. Layout-aware extraction that maps coordinates to ACORD fields avoids this. — [Activepieces](https://www.activepieces.com/blog/extract-data-from-acord-forms-ai-for-insurance-teams) / [Reducto](https://llms.reducto.ai/acord-form-extraction) (search summary)
  - Checkboxes (for example additional insured or subrogation waived, the "ADDL INSD / SUBR WVD" columns) are a known failure point: OCR reads the label but not whether the box is marked. ACORD 25s often arrive as faxes or low-resolution scans with stamps overlapping fields. — [Reducto ACORD extraction](https://llms.reducto.ai/acord-form-extraction)
  - The "Description of Operations" free text often carries AI wording and endorsement numbers, so it must be extracted too. — [Docsumo ACORD 25](https://www.docsumo.com/blog/acord-25-data-extraction); [Docsumo guide](https://www.docsumo.com/blogs/data-extraction/from-acord-25-forms)
  - LLM errors "look right" despite being structurally wrong, so they are harder to catch than OCR errors. — [Vellum 2026](https://www.vellum.ai/blog/document-data-extraction-llms-vs-ocrs)
  - Research result on a non-ACORD dataset (DocILE): routing the lowest-confidence 20% of predictions to human review gives 99.1% automated accuracy, against a 73.3% base. — [arXiv 2606.24420](https://arxiv.org/pdf/2606.24420)
  - Docsumo claims 99% field-level accuracy across 250+ document types. This is marketing and not ACORD-specific; I found no independent ACORD 25 benchmark. — [Docsumo](https://www.docsumo.com/blog/acord-25-data-extraction)
- **Status-only tools exist:** an existing AU/US expiry checker flags certificates as valid, expiring, expired or unknown, but explicitly does not verify coverage or authenticity. — [Apify armourylabs](https://apify.com/armourylabs/subcontractor-certificate-expiry-checker)

### Inferences
- **Safest MVP framing:** "tracking and reminders plus a data-extraction assist", not "compliance verification". Show statuses such as "expired", "expires in 30 days" and "missing AI endorsement upload", not a green "compliant". [Schätzung]
- **Human review:** keep a human review step (founder or customer) for low-confidence extractions and for every checkbox and limit field. Store the original PDF next to the extracted data. [Schätzung]
- **Legal hygiene:** put a disclaimer in the terms ("not insurance advice; certificate is informational; verify endorsements with the carrier or broker") and consider small E&O coverage once revenue exists. Giving advice on coverage adequacy may come close to activity that requires an insurance licence in some states. That last point is unverified and needs legal review. [Schätzung]
- **Low-risk differentiator:** collect the actual AI endorsement PDF and the WC certificate, and keep a dated history for audits. [Schätzung]

### Gaps
- I could not retrieve any COI-tracking vendor's terms of service or liability disclaimer (search budget exhausted), nor any lawsuit against a COI-tracking vendor.
- No independent accuracy benchmark for LLM or vision extraction on ACORD 25.
- ACORD form licensing: whether a tool may render or reproduce ACORD forms (ACORD is a registered mark) was not researched. Reading uploaded forms is likely fine, but this is unverified.

## 6. Channels to win the first 10 paying customers without an ad budget

### Takeaway
I found little verified channel data. The visible landscape shows that SEO "best COI software 2026" listicles are saturated: every competitor publishes them. Reddit self-promotion is widely restricted. Communities with a confirmed audience include NARPM (about 5,300–6,000 members), ContractorTalk, the QuickBooks Community and BiggerPockets, all of which have existing COI threads to answer. Insurance brokers and carriers run outsourced COI programs, which hints at a broker or partner channel.

### Cited Findings
- **Reddit rules:** a third-party database says r/constructionit's written rules take no clear position on promotion, so ask the mods first; on r/constructionmanagers, obvious product pitches tend to get reported. — [ThreadOtter r/constructionit](https://www.threadotter.com/subreddit-rules/constructionit); [ThreadOtter r/constructionmanagers](https://www.threadotter.com/subreddit-rules/constructionmanagers)
- **Reddit in general:** a 2026 study found that 61% of 49 subreddits where founders pitch ban self-promotion. Another database of 64 subreddits reports 34% ban it outright. Rules are in each sidebar or wiki; some allow promotion only in designated threads or on set days. — [OneUp study 2026](https://oneup.today/blogs/reddit-selfpromo-rules-study-2026); [OneUp checker](https://oneup.today/tools/reddit-self-promotion-checker); [Redship guide 2026](https://redship.io/blog/reddit-self-promotion-rules); [Soar database](https://www.soar.sh/blog/self-promotion-rules-by-subreddit-database)
- **NARPM:** more than 5,300 members in the US, Canada and other countries (press kit). A 2026 blog says the association is "reinventing itself" ("NARPM 2.0"). — [NARPM Press Kit](https://www.narpm.org/press-center/press-kit/); [NARPM Join](https://www.narpm.org/join/); [Peter Lohmann](https://www.peterlohmann.com/blog/narpm-2-0)
- **Existing COI threads to answer:**
  - [ContractorTalk](https://www.contractortalk.com/threads/software-for-managing-subcontractor-certs-of-insurance-associated-sub-data.264865/)
  - [QuickBooks Community](https://quickbooks.intuit.com/community/reports-and-accounting-5/is-there-a-way-to-track-when-certificates-of-insurance-expires-for-vendors-that-are-subcontractors-40576)
  - [BiggerPockets (contractor insurance)](https://www.biggerpockets.com/forums/52/topics/77235-how-do-you-handle-insurance-for-your-contractors)
  - [BiggerPockets (AppFolio renters insurance)](https://www.biggerpockets.com/forums/52/topics/1276812-best-way-to-track-tenant-renters-insurance-at-scale-appfolio)
- **SEO and content saturation:** the following vendors all publish "best/affordable COI tracking software 2026" comparisons, ranking for the same queries. — [SubDoc](https://subdoc.io/blog/affordable-coi-tracking-software); [COI File](https://coifile.com/coi-tracking/best-software/); [TrackMyVendor](https://trackmyvendor.com/compare-coi-tracking-software); [COISoftware](https://coisoftware.com/best-coi-tracking-software); [Certificial](https://www.certificial.com/blog-post/we-compared-7-best-coi-tracking-software-in-depth-feedback-and-review); [bcs](https://www.getbcs.com/blog/top-certificate-of-insurance-tracking-companies); [Billy](https://billyforinsurance.com/resources/resources-best-coi-tracking-software-2026/); [Vertikal RMS](https://www.vertikalrms.com/article/best-coi-tracking-software-2026-top-coi-platforms-for-contractors/); [Docsumo](https://www.docsumo.com/blog/best-coi-tracking-software)
- **Broker and insurer channel:** an insurer (ProSight Specialty) selected Docutrax to run a sub-compliance program in which state-licensed account managers collect, track and audit contracts and policies (date n/a). — [BioSpace/Docutrax](https://www.biospace.com/docutrax-selected-to-oversee-new-subcontractor-compliance-program-of-prosight-specialty-insurance)
- **Marketplaces and templates:** COI micro-tools are sold on Apify and Gumroad. — [Apify](https://apify.com/armourylabs/subcontractor-certificate-expiry-checker); [Gumroad](https://siteready.gumroad.com/l/wsbhkx)
- **Context on solo-SaaS outcomes:** a TrustMRR-based analysis (self-selected sample) reports that the median 30-day revenue among 4,987 earning products was $169. — [TechStartups 2026-09-28](https://techstartups.com/2026/09/28/what-percentage-of-indie-hacker-products-make-100k-in-arr/)

### Inferences
These are untested plans, not verified facts.
- **Highest-leverage path with no budget:** direct, manual outreach to about 100–200 small GCs and PM firms. Find them through local AGC/ABC chapter member directories, NARPM chapter directories, and Google Maps listings. Offer a "we'll load your current spreadsheet and COIs for you" concierge onboarding, so the founder does the data entry by hand at first. [Schätzung]
- **Insurance agents and brokers** who write contractor GL/WC policies have a direct interest in clients passing audits and could refer or white-label. Offer them a free branded portal. [Schätzung]
- **Reddit and forums:** answer existing COI threads helpfully (ContractorTalk, QuickBooks Community, BiggerPockets, r/ConstructionManagers) with a disclosed link only where the rules allow. Expect a slow trickle rather than 10 customers. [Schätzung]
- **Free lead magnets:** a free Google Sheets or Excel COI tracker template with expiry formulas, or a free "COI checker" (upload a PDF, get the extracted dates and limits). These collect emails from the exact target audience. [Schätzung]
- Avoid competing on "best COI tracking software" SEO in the first 30 days, since at least 9 vendors already own that content. [Schätzung]

### Gaps
- **Trade associations:** local ABC/AGC chapter vendor-membership costs and rules, AGC/ABC member counts, and NARPM affiliate or vendor membership rules and fees were not found (search budget exhausted).
- **Facebook groups:** no specific contractor or property-manager Facebook groups or member counts found.
- **Newsletters and podcasts:** none identified with audience size.
- **Subreddit rules:** the actual sidebar rules for r/Construction, r/Contractor, r/PropertyManagement, r/smallbusiness and r/Insurance were not verified.
