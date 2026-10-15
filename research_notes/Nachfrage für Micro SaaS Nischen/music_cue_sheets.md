# Music Cue Sheet Generator from Timeline Exports (EDL / FCPXML / Premiere XML / AAF / Resolve): Market Research Notes

*Research date: 2026-10-15. How these notes were made: WebFetch could not resolve any host in this session (`getaddrinfo ENOTFOUND` for editingtools.io, ascap.com, digitalmusicnews.com, filmink.com.au), and the egress proxy refused direct curl. Reddit was also blocked for search ("domains are not accessible to our user agent"). The shared web-search budget ran out (200 per turn) partway through. So every finding below comes from **search-result snippets and summaries, not full page reads**. Prices and quotes should be re-checked on the live page before anyone relies on them. The GitHub findings come from the GitHub API and are verified. Semrush was not available (see `semrush_keyword_metrics.md`: `no_api_units` / `no_subscription`).*

---

## 1. What a cue sheet is, who must file it, which deliverables require it, and what happens when it is missing or wrong

### Takeaway
A music cue sheet lists every music use in a production: title, composer/publisher, PRO affiliation, timing/duration and usage type. The **production company** (in practice the music supervisor, post coordinator or clearance coordinator) is expected to file it with the PROs. Broadcasters such as PBS and the BBC, streamers such as Netflix, distributors and E&O insurers all treat it as a delivery item. When it is missing or wrong, composers mainly lose royalties, and late fixes run into limited retroactive windows. Delivery can also be held up.

### Cited Findings
**Definition and fields**
- A cue sheet is "a detailed document that lists all the music and how it was used in a production, such as a film, TV show, video game, podcast, or commercial" — [Orfium, "Cue sheets: the essential guide part 1" (undated)](https://www.orfium.com/cue-sheets/cue-sheets-the-essential-guide-part-1/)
- A guide lists each cue's title, duration, composer and publisher, recording owner, timecodes and license reference as cue sheet contents. ASCAP, BMI and SESAC use cue sheets to route royalty payments — [Thoolie, Indie Film Delivery Checklist (undated, 2026 site)](https://thoolie.com/creator_resource/indie-film-delivery-checklist/)
- Netflix job postings name "synchronization licenses, publishing splits, IPI numbers, and PRO information" as key cue sheet knowledge — [Showbizjobs: Netflix Cue Sheets Coordinator (undated)](https://www.showbizjobs.com/jobs/netflix-cue-sheets-coordinator-in-los-angeles/jid-74e0oq); [Mediabistro: Music Cue Sheets Coordinator, Netflix](https://www.mediabistro.com/jobs/3541382433-music-cue-sheets-coordinator-netflix)
- BMI and ASCAP published a standardized cue sheet template (publication date not captured) — [MusicRow: "BMI, ASCAP Reveal Standardized Cue Sheet Template"](https://musicrow.com/?p=228473)

**Who files**
- PremiumBeat tells customers to "make sure you or your production company submits it electronically to every PRO listed in the sheet" — [PremiumBeat: Reporting Music Used In Your Projects (undated)](https://www.premiumbeat.com/royalty-free/cuesheet)
- SOCAN: a cue sheet "completed by the producer of a film, television show, or digital production has typically been considered the authoritative source." Broadcasters, distributors, international PROs and SOCAN members may also submit. SOCAN advises members to tell production companies to file their cue sheets — [SOCAN Magazine (undated)](https://www.socanmagazine.ca/?p=51818)
- A 2026 vendor guide says the production company files, "usually through a music supervisor, post-production coordinator, or clearance coordinator." The composer does not file but should check the sheet. Its slogan is "No cue sheet, no royalty" — [DropCue blog: How PROs Pay Composers (2026)](https://dropcue.app/blog/how-pros-pay-composers); [DropCue: Music Cue Sheet Guide 2026](https://dropcue.app/blog/music-cue-sheet-guide). This is a secondary vendor source.
- ASCAP and BMI run **RapidCue**, a joint web portal "to enter, manage and electronically submit music cue sheet data for television, cable and film productions" (launch announcement 2007) — [BMI press release, Aug 14 2007](https://bmi.com/news/entry/bmi_ascap_announce_launch_of_rapidcue_online_cue_sheet_technology); [NextTV: ASCAP, BMI Roll Out RapidCue (2007)](https://www.nexttv.com/news/ascap-bmi-roll-out-rapidcue-30502)
- Netflix has an in-house "Cue Sheets and Music Administration" team inside Music Business & Legal. It "partner[s] closely with productions, internal stakeholders, and our publishing administrator to support cue sheet creation and delivery" — [Showbizjobs Netflix posting](https://www.showbizjobs.com/jobs/netflix-cue-sheets-coordinator-in-los-angeles/jid-74e0oq); [Music Connection: Netflix needs a Music Cue Sheets Coordinator](https://www.musicconnection.com/netflix-needs-a-music-cue-sheets-coordinator/). Netflix's public Backlot partner-help pages turned up no producer-facing cue sheet spec ([Backlot fulfillment-partner delivery page](https://backlothelp.netflix.com/hc/en-us/articles/223351987) covers audio, subtitles and metadata only).

**Deliverables lists that require it**
- **PBS:** music cue sheets are due from the producer or presenter before the initial broadcast. The Red Book deliverables page lists "6 weeks prior to the air date." Sheets must be submitted through **RapidCue** and must list all music: commissioned, library, popular, compulsory-license, fair use and public domain. Producers can use PBS's statutory/compulsory sync licenses "only if they timely submit a cue sheet." These documents are dated 2018/2019, so verify they are current — [PBS Red Book Deliverables (rev. 5/2018)](https://bento.cdn.pbs.org/hostedbento-prod/filer_public/PBS_About/Producing/Red%20Book/Deliverables%205.2018.pdf); [PBS Producer's Handbook (Dec 2019)](https://bento.cdn.pbs.org/hostedbento-prod/filer_public/Producing%20for%20PBS/Handbook%20Drafts/PBS%20Producer's%20Handbook%20(December%202019).pdf); [PBS Rights Requirements (rev. 5/2018)](https://bento.cdn.pbs.org/hostedbento-prod/filer_public/PBS_About/Producing/Red%20Book/Rights%205.2018.pdf); [NETA: PBS Music Licensing overview](https://www.netaonline.org/sites/default/files/uploads/documents/pbs-music-licensing-overview.pdf)
- **BBC (UK):** BBC producers use Soundmouse to search and download music, and "use our audio recognition technology to create a cue sheet." "For certain programmes, the production company will be required to review and verify the cue sheet before it is submitted to the BBC"; "BBC Productions will be responsible for cue sheet approvals." PRS Tunecode is a recommended metadata field. This is an undated Soundmouse/BBC deck — [Soundmouse and the BBC Music Portal (PDF)](https://www.soundmouse.com/bbc/BBC_Music_Portal_Presentation_Template_standard_v1.1.pdf). PRS lists Soundmouse as the platform that helps it track music use in UK TV and radio — [PRS for Music: Soundmouse](https://www.prsformusic.com/what-we-do/soundmouse)
- **Distributors / streamers (indie film):** a quick-answer delivery list includes "music licenses and cue sheet" next to E&O, chain of title and clearance log. "an incomplete or inaccurate cue sheet will delay distribution and can trigger claims from publishers and labels" — [Thoolie: Indie Film Delivery Checklist](https://thoolie.com/creator_resource/indie-film-delivery-checklist/); see also [Agnès Films: The Big "D" of Distribution: Deliverables](https://agnesfilms.com/filmmaking-advice/the-big-d-of-distribution-deliverables/); [Carbon Arc Media: Film Legal Delivery Services](https://carbonarcmedia.com/delivery.html)
- **E&O insurers:** underwriters ask for the cue sheet and chain-of-title paperwork. Underwriting takes about 1–4 days for a clean narrative feature and 4–8+ weeks for documentaries with more clearance questions. Typical distributor-set limits are $1M per occurrence / $3M aggregate with a deductible around $10,000 — [Thoolie: Documentary Release Requirements](https://thoolie.com/creator_resource/documentary-film-release-checklist/); [Akker Insurance: Film E&O guide](https://www.akkerins.com/new-blog/film-eo-insurance-guide-clearance-music-distribution). These are secondary vendor and broker blogs.
- Festivals: **no source found** (see Gaps).

**What happens when a cue sheet is missing or wrong (composer side)**
- One composer was told ASCAP would not process proof of usage without official cue sheets from the network. They got final cue sheets from the music supervisor and submitted them more than a year after air, then had to wait 6 months after the final air date before ASCAP would investigate. Another poster reported about 200 unpaid Telemundo shows despite filed cue sheets, because the performances didn't appear in ASCAP's survey. A third said BMI "only pay so many quarters retroactively" — [MusicLibraryReport forum threads (undated; one titled "these shows still unpaid from 2013")](https://musiclibraryreport.com/forums/topic/these-shows-still-unpaid-from-2013/page/2); [MLR: "Cue Sheets were filed incorrectly, what should I do?"](https://musiclibraryreport.com/forums/topic/cue-sheets-were-filed-incorrectly-what-should-i-do); [MLR: not getting paid on submitted cue sheets](https://musiclibraryreport.com/forums/topic/not-getting-paid-on-submitted-cue-sheets)
- A VI-Control poster: "I think ASCAP has a cutoff of something like one year to notify them if an expected royalty isn't showing up, and I've gotten a couple concessions by calling" — [VI-Control: "cue sheet sent late" (undated)](https://vi-control.net/community/threads/cue-sheet-sent-late.163303/)
- A 2026 guide: ASCAP can retroactively credit royalties missed because of a late cue sheet only if the member notifies ASCAP by January 31 (December 31 for publishers) — [DropCue: Music Cue Sheet Guide 2026](https://dropcue.app/blog/music-cue-sheet-guide). This is secondary; confirm against ASCAP.

### Inferences
- Legally, filing is mostly a **contractual and delivery obligation**, not a statutory one: the composer agreement, the broadcaster deliverables and the distributor delivery schedule. The practical "must" comes from delivery acceptance (PBS, BBC, distributors) and from composers and libraries chasing royalties.
- Big studios and streamers have in-house teams (Netflix) or enterprise vendors (Soundmouse for the BBC). The **underserved segment is small producers**: indie docs, unscripted and corporate/branded series, and small post houses. They get a deliverables list that says "music cue sheet" and have no staff for it.
- Composers and libraries are **motivated secondary stakeholders**. Their royalties depend on someone else's paperwork, which makes them a natural referral channel (see section 6).

### Gaps
- Could not read ASCAP, BMI, SESAC, SOCAN, PRS or APRA AMCOS primary pages (WebFetch DNS failure), so current official submission rules, deadlines and formats are unconfirmed. APRA AMCOS and SESAC requirements were not found at all.
- No current (2024–2026) Netflix, BBC, CBC, ABC (AU), Channel 4 or ITV producer-facing cue sheet spec found. PBS documents are from 2018/2019.
- No source found on **festival** cue sheet requirements. Festivals are generally not expected to require one [Schätzung].
- No quantified estimate of royalties lost to missing cue sheets.

---

## 2. Current workflow and pain: demand signals

### Takeaway
The standard workflow has been the same since at least 2010: export a music-only EDL or XML from Avid, Premiere or Resolve, then clean it by hand in a spreadsheet. That means merging duplicate and overlapping uses, removing invisible cuts, converting timecode to durations at the right frame rate, assigning usage codes and looking up composer/publisher/PRO metadata. People describe the work as a "hellish spreadsheet" and a "multi-day spreadsheet nightmare." Composer forums are full of cases of cue sheets that are missing, late or wrong. Reddit, LiftGammaGain and Avid community threads **could not be reached** in this session.

### Cited Findings
**Workflow evidence**
- Creative COW, Final Cut Pro Legacy forum, thread "Outputting a Music Cue Sheet": "Export an EDL of only the tracks that contain music. CMX3600." (Shane Ross, **April 10, 2010**) — [Creative COW](https://creativecow.net/forums/thread/outputting-a-music-cue-sheet/)
- Creative COW, Avid Media Composer forum, thread "Exporting EDLs for Cue Sheets" (**2012**). A user asked for an efficient way to get cue data out of Avid when overlapping copies of the same cue must count as one use. The suggested workaround was to decompose the audio tracks with zero handles; "The process takes fades and dissolves into consideration and only will make one clip, even if used several times. Sort results and export as TAB" — [Creative COW](https://creativecow.net/forums/thread/exporting-edls-for-cue-sheets/)
- A library cue sheet service asks for a music-only EDL and "please be sure to share the frame rate so we can properly calculate durations from timecode" — [Slipstream Music Cue Sheet Generator](https://slipstreammusic.com/cuesheet) (attribution from the search summary)
- Edge cases editors run into: a VI-Control poster asks how to code diegetic TV-show-theme music because "none of the 'Usage Codes', BI, BV, VI, VV, MT, ET, or Logo seem to address this" — [VI-Control: "cue sheet questions" (undated)](https://vi-control.net/community/threads/cue-sheet-questions.150717/)
- The work also appears as job duties. ESPN's music assistant role includes "organizing and inputting audio assets and music cue metadata into the cue sheet management system" — [The Muse: Disney/ESPN Music Assistant](https://www.themuse.com/jobs/disney/music-assistant-380af5). An NFL Films seasonal music editor must "track music usage and create corresponding cue sheets" — [Greenhouse: NFL Films](https://job-boards.greenhouse.io/nflprivateposting/jobs/4756569008)

**Pain quotes and demand signals (URL, date where known)**
1. "hellish spreadsheet used to log every single second of music used in every single episode / programme of broadcast television" — [FilmInk, article on Melodie's Cue Sheet Tool (~Aug 2024)](https://www.filmink.com.au/?p=99565)
2. "It's a multi-day spreadsheet nightmare... please save me." This is an answer option in the early-access survey of **Cuedio**, a pre-launch cue sheet startup. The survey asks editors their role, team type, music libraries, main NLE and time spent on cue sheets. It is a vendor-written option, not a user quote, but it shows someone else is validating the same idea — [Cuedio early access form (Tally, undated, likely 2026)](https://tally.so/r/A782rl)
3. A blog post titled "Cue Sheets Explained: The Invisible Paperwork That Gets You Paid (And Why Music Coordinators Low-Key Hate Them)" (title only, undated) — [Young Coconut Music](https://youngcoconutmusic.com/cue-sheets-explained-the-invisible-paperwork-that-gets-you-paid-and-why-music-coordinators-low-key-hate-them/)
4. Composer chasing missing sheets: thread "ASCAP missing cue sheets for several shows. Missed royalty payment date. Next steps?" (title only, undated) — [VI-Control](https://vi-control.net/community/threads/ascap-missing-cue-sheets-for-several-shows-missed-royalty-payment-date-next-steps.128281/)
5. Composer: "Cue Sheets were filed incorrectly, what should I do?" (undated) — [MusicLibraryReport](https://musiclibraryreport.com/forums/topic/cue-sheets-were-filed-incorrectly-what-should-i-do). A related thread asks "Anyone have the cue sheets for these shows?" — [MLR "these shows still unpaid from 2013"](https://musiclibraryreport.com/forums/topic/these-shows-still-unpaid-from-2013/page/2). Others: [MLR "how long for a cue sheet to show up"](https://musiclibraryreport.com/forums/topic/how-long-for-a-cue-sheet-to-show-up); [MLR "Cue Sheet Timeline: From Placement to Payment"](https://musiclibraryreport.com/forums/topic/cue-sheet-timeline-from-placemenrt-to-payment/)
6. MLR members say ASCAP "is there to pay you but not to investigate the uses and cue sheet errors," and suggest going back through the library, music supervisor or production company — [MLR: ASCAP and their inadequate survey system](https://musiclibraryreport.com/forums/topic/ascap-and-their-inadequate-survey-system/page/6/)
7. Stage 32 Post-Production Lounge thread "Music cue sheet," tagged "Now Trending!" (title only) — [Stage 32](https://www.stage32.com/lounge/post_production/Music-cue-sheet)
8. Gearspace: "publisher on cue sheets?" (title only) — [Gearspace](https://gearspace.com/threads/publisher-on-cue-sheets.1374444/). Skool community post "Story Time (missing cue sheets)" — [Skool: Hit Record Academy](https://www.skool.com/hit-record-academy-7764/story-time-missing-cue-sheets)
9. **Builder signal (verified through the GitHub API):** at least 8 new public GitHub repos created **Apr–Oct 2026** target exactly this job. Examples:
   - [Obrais-cloud/cuesheet](https://github.com/Obrais-cloud/cuesheet) (created 2026-09-27): "Edit timeline (EDL/FCPXML) → music cue sheet + archive/stock usage report with rights-gap check. Stdlib Python, no cloud."
   - [buildwithtolu/cueclear](https://github.com/buildwithtolu/cueclear) (2026-08-21): "EDL/XML in, … cue sheet out"
   - [geckon1film/gema-gelileo-codexskill](https://github.com/geckon1film/gema-gelileo-codexskill) (2026-07-29): "overlap-safe GEMA music cue sheets from Final Cut Pro and DaVinci Resolve XMEML timelines"
   - [Adarsh54/cuestamp](https://github.com/Adarsh54/cuestamp) (2026-09-15)
   - [danielharrington-WTV/WTV-Audio-Wizard](https://github.com/danielharrington-WTV/WTV-Audio-Wizard) (2026-09-24)
   - [paulreevessound/music-cue-sheet](https://github.com/paulreevessound/music-cue-sheet) (2026-04-28)
   - [Manas103/music-cue-sheet-clearance-gate](https://github.com/Manas103/music-cue-sheet-clearance-gate) (2026-10-02)
   - [miwco/ArchiveCheck](https://github.com/miwco/ArchiveCheck) (2026-06-14, recognition plus credits OCR)
   - All have 0–1 stars.

### Inferences
- The pain is real and old (2010–2012 forum workarounds are still the same steps tools automate in 2026), but **the merging and formatting part is largely solved** by existing tools (section 3). The pain that remains is **metadata**: composer, publisher, PRO, IPI and splits for tracks not in a partner library. A second remaining pain is **PRO/broadcaster-specific output formats**.
- The 2026 wave of hobby/AI-built GitHub tools and the Cuedio pre-launch both suggest **low barriers to entry and a crowded idea space**. An editor using Claude Code can build the parser, but so can many others.
- Two buyer emotions: **post-side** ("get this deliverable off my desk") and **composer-side** ("make sure I get paid"). Composer pain is louder online, but composers are not the ones who file.

### Gaps
- **No Reddit quotes** (r/editors, r/postproduction, r/Filmmakers, r/WeAreTheMusicMakers). Reddit is blocked for this agent's search and fetch. **No LiftGammaGain or Avid Community threads** were found before the search budget ran out. The user should search these manually: `site:reddit.com/r/editors "cue sheet"`.
- Most forum threads have no visible date in the snippets. Only the Creative COW threads are dated (2010, 2012). The quote requirement (5+ dated 2024–2026 quotes) is **not fully met**.
- No survey data on time spent per cue sheet. Cuedio's "multi-day" option is the only hint, and it is vendor-written.

---

## 3. Existing tools and prices: who already does EDL → cue sheet

### Takeaway
**Yes, the exact job is already done.** EditingTools.io (a German post-tools company) runs a **Music Cue Sheet** generator and a **Music Cue Sheet Manager**. They take EDL, FCP7 XML, FCPXML and Pro Tools text from Avid, Premiere, Resolve and FCP. They merge duplicates and invisible cuts, auto-fill metadata from **20+ partner libraries (10–15M tracks)**, and export CSV, Excel, PDF, **CISAC and APRA formats**. A free Premiere panel and a REST API are included. Pricing runs from a Free tier to PRO subscription, Day-Pass and project-based plans; exact dollar amounts could not be retrieved. Music libraries (Melodie, Slipstream) give away free EDL/XML → cue sheet tools for their own catalogs. Enterprise players (Soundmouse/Orfium, Cuetrak/Music Reports, Qwire, RapidCue) serve broadcasters and studios with quote-only pricing.

### Cited Findings
**Direct EDL/XML → cue sheet tools**

*EditingTools.io: Music Cue Sheet and Music Cue Sheet Manager*
- Reads sequences from Media Composer, Premiere Pro, Resolve and Final Cut Pro. For Premiere or Resolve it recommends exporting **Final Cut 7 XML**. Inputs: EDL, XML, FCPXML, TXT, CSV. Exports to CSV, XLSX, PDF via presets. "Merge multiple tracks and remove invisible cuts to have a clean list" — [EditingTools.io Music Cue Sheet](https://editingtools.io/cuesheet/)
- The Manager also reads Pro Tools session info and offers CSV, Excel, **CISAC and APRA** exports. Metadata comes from "10M+ tracks from 20+ partner libraries" (the cuesheet page says 15M+, an inconsistency). No limit on sheets or entries — [EditingTools.io Music Cue Sheet Manager](https://editingtools.io/cuesheetmanager/)
- A **free** Premiere Pro panel, "Music Cue Sheet Uploader" (Premiere CC 2022+, Win/Mac), is described as "a free, light version of our Listify plugin." It needs an API key from a free account — [EditingTools.io Cue Sheet Uploader](https://editingtools.io/plugins/cuesheetuploader/); [Adobe Exchange listing](https://exchange.adobe.com/publisher/cc/8b1d028e-33e1-4589-b9e6-39f67d77553a/editingtoolsio). The Adobe Exchange listing shows other EditingTools plugins at **$15.99, $29.99 and $49.99**. Which price belongs to which plugin (e.g. Listify) could not be confirmed.
- REST API for cue sheet conversion (recommended max file size 10 MB) — [EditingTools.io API v2 cuesheets](https://editingtools.io/api/v2/cuesheets/)
- Pricing structure: Free tier; **PRO** (monthly or annual; "unlimited projects, priority processing, batch operations"); **Day-Pass** (24 h of PRO, one-time); **Project-Based** (per week, 8–90 weeks, no recurring billing); Educational (6-month fixed term); Team subscriptions; plus extra AI credits. **Exact amounts were not retrieved** — [EditingTools.io Pricing](https://editingtools.io/pricing/); [EditingTools.io Support](https://editingtools.io/support/)
- Company profile: a Digital Production interview dated **11 Sep 2026** describes a toolbox of "small utilities, strict metadata, offline workflows, human support" across Premiere, Avid, Resolve, FCP and Pro Tools — [Digital Production, 2026-09-11](https://digitalproduction.com/2026/09/11/editingtools-io-the-post-production-toolbox/). Exhibited at IBC's German Pavilion — [IBC German Pavilion listing](https://ibc.german-pavilion.com/en/sites/products-services/197864)

*Free library tools (single catalog only)*
- **Melodie (AU), Cue Sheet Tool**, launched Aug 2024. Upload an XML or EDL and get CSV/XLS/XLSX/TXT with timecodes, durations and "full track metadata for all Melodie tracks, compatible with major PRO formats," plus a Cue Sheet History. Described as "quick, easy and free" — [Señal News, 27 Aug 2024](https://senalnews.com/en/digital/melodie-unveiled-a-new-music-development-cue-sheet-tool); [FilmInk (~Aug 2024)](https://www.filmink.com.au/?p=99565). A Melodie blog post titled "No More Music Cue Sheets. (You're Welcome)." is dated 22 Feb 2024 (content not retrieved) — [Melodie blog](https://blog.melod.ie/2024/02/22/no-more-music-cue-sheets/)
- **Slipstream, Cue Sheet Generator (Beta)**: upload an EDL and get a cue sheet with rights metadata for Slipstream tracks. "Unmatched events are still included with their timecodes, with rights columns left blank" — [Slipstream support article](https://support.slipstreammusic.com/en/articles/15313476-cue-sheet-generator-beta); [slipstreammusic.com/cuesheet](https://slipstreammusic.com/cuesheet)
- PremiumBeat (Shutterstock) has a cue sheet reporting page for its library — [PremiumBeat cuesheet](https://www.premiumbeat.com/royalty-free/cuesheet). SourceAudio (a library-hosting platform) has a cue sheet admin module — [SourceAudio docs: Cue Sheets](https://docs.sourceaudio.com/administration/cue_sheets.html)

*Other small or desktop tools*
- **Brewer** (macOS): reads EDLs from FCP or Avid and builds clip lists and cue sheets with spreadsheet export. The demo loads only 50% of an EDL. Price not captured — [Softpedia Mac: Brewer](https://mac.softpedia.com/get/Utilities/Brewer.shtml)
- **Q-Cuts**: "music cue sheet generation software" with CSV filter templates published on GitHub in 2020 — [dheidelberger/Q-Cuts-CSV-Templates](https://github.com/dheidelberger/Q-Cuts-CSV-Templates). Vendor page and price not found.
- **Screenweaver.ai**: page title "Music Cue Sheet Generator: Free PDF and CSV" (content not retrieved) — [screenweaver.ai](https://www.screenweaver.ai/tools/cue-sheet-generator)
- **BookWriter "Music cue sheet builder"**: form-based builder that defines the BI/BV/VI/VV/MT/ET codes — [bookwriter.vip](https://www.bookwriter.vip/music-cue-sheet-builder)
- **Cuedio**: pre-launch, early-access form only — [Tally](https://tally.so/r/A782rl)
- **CueReady (Radio Ready Ware)**: radio-syndication cue sheets, **$29.99 one-time**, no subscription, one license per show — [Payhip](https://payhip.com/b/KHBjT). This is the radio segment, not film/TV.
- Free Word/Excel templates: [Business-in-a-Box cue sheet template](https://www.business-in-a-box.com/template/cue-sheet-D14094); [Loughborough template](https://lbas.lboro.ac.uk/template/music-cue-sheet-template.html); [Music Gateway how-to](https://musicgateway.com/blog/music-industry/what-is-a-cue-sheet-and-how-to-create-one)

**Enterprise and PRO-side platforms**
- **Soundmouse (Orfium)**: web cue sheet and music reporting with audio recognition that creates draft cue sheets. Used by the BBC and PRS. Pricing is a **one-time setup fee plus a monthly service fee**, depending on production volume, distribution channels, societies and users. **No amounts are published** — [Orfium FAQ](https://www.orfium.com/frequently-asked-questions/); [Orfium: What is Soundmouse](https://www.orfium.com/what-is-soundmouse-by-orfium/); [Soundmouse for broadcasters](https://pages.orfium.com/soundmouse-for-broadcasters). A related price point: Harvest Media charges **AUD 10 per catalogue per month** for its Soundmouse metadata delivery integration. That is library-side, not a cue sheet price — [Harvest Media: Soundmouse](https://wwwcforigin.harvestmedia.net/soundmouse/)
- **Cuetrak (Music Reports)**: "the world's leading cue sheet and analytics solution." Price not published — [Music Reports Cuetrak](https://www.musicreports.com/cuetrak). Explainer article dated **17 Apr 2026** (content not retrieved) — [Digital Music News](https://www.digitalmusicnews.com/2026/04/17/cue-sheets-cuetrak-service-how-it-works/)
- **Qwire**: cue sheet and music reporting software for productions. Price not found — [Qwire press clipping](https://qwire.rockpaperscissors.biz/artist/14017/press_clips/17828/white)
- **RapidCue (ASCAP/BMI)**: PRO submission portal (2007). Cost not found — [BMI](https://bmi.com/news/entry/bmi_ascap_announce_launch_of_rapidcue_online_cue_sheet_technology)

**Prior art / IP**
- US patent **US7925671B2**, "Method and system for automatic cue sheet generation": "The computer parses the EDL file to extract track file names, a duration of use, and a time code… searches a database for the track file name to retrieve a composer, publisher, and PRS" — [Google Patents US7925671](https://patents.google.com/patent/US7925671); related application [US20060044957](https://patents.justia.com/patent/20060044957); [US20090202220](https://patents.justia.com/patent/20090202220)

### Inferences
- **The core EDL → cue sheet job is commoditized.** EditingTools.io does it across all major NLEs with library metadata and PRO formats. Libraries give away catalog-specific versions for free. A plain "upload EDL, get spreadsheet" MVP would compete with free tools.
- Possible gaps for a newcomer [Schätzung]:
  - a **library-agnostic metadata layer**: auto-lookup of composer/publisher/PRO for tracks from Artlist, Musicbed, Epidemic, APM, Extreme and similar, which may or may not be among EditingTools' 20+ partners
  - **ready-to-submit output per destination**: RapidCue/ASCAP/BMI, SOCAN, PRS/Soundmouse, APRA, PBS, distributor templates
  - a **composer verification loop**: share link, composer confirms splits and IPI
  - a **rights-gap check** that flags uncleared cues before delivery
- **Patent risk:** US7925671 claims EDL parsing plus DB lookup for cue sheets. Its family dates from about 2005–2006 (publication 2006), so it **may have expired around 2025–2026** [Schätzung]. This needs a legal or Google Patents status check.
- Pricing ladder observed: free (library tools, EditingTools free tier) → day-pass or project-based (EditingTools) → $15.99–$49.99 plugin prices (Adobe Exchange, mapping unclear) → enterprise setup plus monthly (Soundmouse).

### Gaps
- **Not found because the search budget ran out:** RightsTrack, "Cue Sheet Pro," Silvermouse, TuneSat and BMAT pricing or product pages. The cue sheet features of APM, Extreme Music, Musicbed, Artlist and Epidemic Sound were also not found. Whether these exist as described was not checked; nothing is invented here.
- Exact EditingTools.io PRO, Day-Pass and Project-Based dollar or euro prices: the page was found but could not be fetched. Top priority to check manually at https://editingtools.io/pricing/
- Which libraries are among EditingTools' "20+ partners": not retrieved.
- No usage or traction numbers for any tool.

---

## 4. Volume of productions, who pays, pricing norms and willingness to pay

### Takeaway
No sourced production counts could be gathered in this session; the search budget was exhausted. What the evidence does show: in the enterprise tier, payers are broadcasters and studios (Soundmouse, Cuetrak, in-house Netflix team). For independent productions, **the production company pays**, through the music supervisor, post coordinator or clearance coordinator. Current pricing norms are **per-project or time-boxed** (Day-Pass, project weeks) at the low end and **setup plus monthly** at the enterprise end.

### Cited Findings
- Responsible roles: the production company, "usually through a music supervisor, post-production coordinator, or clearance coordinator" — [DropCue guide (2026)](https://dropcue.app/blog/how-pros-pay-composers)
- Dedicated paid roles exist at scale. Netflix hires a "Music Cue Sheets Coordinator" — [Music Connection](https://www.musicconnection.com/netflix-needs-a-music-cue-sheets-coordinator/). ESPN and NFL Films music assistants and editors list cue sheets as a core duty — [The Muse/ESPN](https://www.themuse.com/jobs/disney/music-assistant-380af5); [NFL Films/Greenhouse](https://job-boards.greenhouse.io/nflprivateposting/jobs/4756569008)
- Per-project pricing exists in the closest competitor: EditingTools.io sells a **Day-Pass** (24 h) and **Project-Based** plans billed per week for 8–90 weeks with no recurring billing, alongside monthly and annual PRO — [EditingTools.io Pricing](https://editingtools.io/pricing/)
- Enterprise: Soundmouse charges a setup fee plus a monthly fee, scaled by production volume, channels, societies and users — [Orfium FAQ](https://www.orfium.com/frequently-asked-questions/)
- One-time pricing in an adjacent niche: CueReady $29.99 per show license — [Payhip](https://payhip.com/b/KHBjT)
- Composer/sync SaaS price points (adjacent buyer: composers and libraries): DropCue Artist **$8/mo**, Pro **$15/mo**, Studio "starting at **$33/month**." The About page lists Starter at $5/mo annual or $7/mo monthly — [dropcue.app](https://dropcue.app/); [DropCue About](https://dropcue.app/about). Capterra shows different, likely outdated figures — [Capterra: Dropcue](https://www.capterra.com/p/10037930/Dropcue/)
- Willingness-to-pay evidence from free competitors: Melodie's tool is free — [FilmInk](https://www.filmink.com.au/?p=99565); Slipstream's is free beta — [Slipstream](https://support.slipstreammusic.com/en/articles/15313476-cue-sheet-generator-beta)

### Inferences
- **[Schätzung] Volume (unverified, no source retrieved this session):**
  - English-language scripted TV runs to several hundred series a year. FX's "Peak TV" counts were roughly 500–600 US scripted series a year in 2022–2023, from memory and **not verified here**. That would mean many thousands of scripted episodes a year.
  - Unscripted, documentary, factual, sports and branded series probably add several times more episodes.
  - Each broadcast episode in the US, UK, Canada and Australia needs a cue sheet.
  - Feature films (studio plus indie with distribution) add low thousands a year across English markets.
  - Ads mostly don't need PRO cue sheets in the US but may in UK and AU (unverified).
  - The realistic SAM for a solo founder is small production companies and post houses delivering docs and unscripted series. Plausibly thousands of companies, but this is not quantified.
- **[Schätzung] Payer mismatch:** indie filmmakers need about 1 cue sheet per film, which suits per-project payment ($19–$49 one-off is plausible, matching the plugin price band). Recurring revenue fits **post houses, unscripted/doc production companies, music libraries (white-label) and composers/publishers** (verification and tracking). The founder's preference for recurring revenue points to series producers and post houses as the ICP, not indie features.
- With free library tools and EditingTools' free tier, **WTP for plain conversion is low**. WTP plausibly exists for saved time on metadata completion and for "delivery-accepted" formatted output; this is untested.

### Gaps
- **No sourced numbers** for productions per year (US, UK, CA, AU features, TV episodes, docs, ads). Suggested sources for a follow-up: FX Networks Research scripted-series count; Ampere Analysis; BFI Statistical Yearbook; CMPA Profile (Canada); Screen Australia Drama Report; Ofcom/Pact UK TV production census; MPA THEME report.
- No sourced fees for outsourced cue sheet preparation (music clearance houses, freelance music coordinators), which is the most direct WTP benchmark.
- No customer interviews or surveys on WTP.

---

## 5. Technical feasibility

### Takeaway
Feasible for a solo editor building with Claude Code. Open-source **OpenTimelineIO** (Academy Software Foundation, actively maintained as of 2026-10) plus its AAF adapter covers the timeline formats. Several hobby repos already do EDL/FCPXML/XMEML → cue sheet in stdlib Python. The hard part is **not parsing** but (a) correct cue logic: merging, overlaps, invisible cuts, frame rate, usage codes; and (b) **rights metadata** (composer, publisher, PRO, IPI, splits). That metadata is not in the timeline and must come from library databases, filename matching or manual entry.

### Cited Findings
**Input formats**
- CMX3600 EDL with music tracks only is the long-standing input — [Creative COW, 2010](https://creativecow.net/forums/thread/outputting-a-music-cue-sheet/)
- Premiere writes XML "according to Apple's retired spec, from around version 7.0.3 of Final Cut Pro," i.e. FCP7 XML/XMEML — [Adobe Community thread](https://community.adobe.com/questions-729/regarding-xml-file-of-premiere-pro-1407312) (attribution from the search summary)
- EditingTools recommends FCP7 XML over EDL for Premiere and Resolve — [EditingTools.io](https://editingtools.io/cuesheet/)
- A Codex skill on GitHub targets "Final Cut Pro and DaVinci Resolve XMEML timelines" — [gema-gelileo-codexskill](https://github.com/geckon1film/gema-gelileo-codexskill)
- **OpenTimelineIO**: "Open Source API and interchange format for editorial timeline information"; 2,020 stars, last updated 2026-10-14 — [AcademySoftwareFoundation/OpenTimelineIO](https://github.com/AcademySoftwareFoundation/OpenTimelineIO). AAF adapter: [OpenTimelineIO/otio-aaf-adapter](https://github.com/OpenTimelineIO/otio-aaf-adapter) (updated 2026-09-22)
- A stdlib Python EDL/FCPXML → cue sheet tool exists: [Obrais-cloud/cuesheet](https://github.com/Obrais-cloud/cuesheet)

**Cue logic**
- Overlapping copies of the same cue must be counted as one use. Fades and dissolves must not split a cue — [Creative COW, 2012](https://creativecow.net/forums/thread/exporting-edls-for-cue-sheets/)
- Commercial tools "merge multiple tracks and remove invisible cuts" — [EditingTools.io](https://editingtools.io/cuesheet/)
- The frame rate is needed to compute durations from timecode — [Slipstream](https://slipstreammusic.com/cuesheet)

**Usage codes**
- BI = background instrumental, BV = background vocal, VI = visual instrumental (performed on screen), VV = visual vocal (sung on screen), MT = main title, ET = end title — [BookWriter cue sheet builder](https://www.bookwriter.vip/music-cue-sheet-builder)
- Real 2025–2026 broadcast cue sheets also use SRC (visual source) and T (theme) — [PGA Tour 2025 Players preview cue sheet](https://internationalmedia.pgatour.com/uploads/special_programs/2025_the_players_preview_show/25intppv-music-cue-sheet.pdf); [PGA Tour 2026 cue sheet](https://internationalmedia.pgatour.com/uploads/the_cut/2026/2026-api-cue-sheet.pdf)
- Codes are not uniform across sheets, and diegetic edge cases are ambiguous — [VI-Control](https://vi-control.net/community/threads/cue-sheet-questions.150717/)
- **Usage type is not encoded in timelines.** It must be set by the user or inferred, e.g. from track names such as "SOURCE" or "SCORE" [Schätzung].

**Metadata sources**
- Partner-library lookup by file name: EditingTools (20+ libraries) — [EditingTools Manager](https://editingtools.io/cuesheetmanager/); Melodie (own catalog) — [Señal News 2024](https://senalnews.com/en/digital/melodie-unveiled-a-new-music-development-cue-sheet-tool); Slipstream (own catalog, unmatched cues left blank) — [Slipstream](https://support.slipstreammusic.com/en/articles/15313476-cue-sheet-generator-beta); patent DB lookup by track file name — [US7925671](https://patents.google.com/patent/US7925671)
- Required identifiers: IPI, publishing splits, PRO — [Netflix posting](https://www.showbizjobs.com/jobs/netflix-cue-sheets-coordinator-in-los-angeles/jid-74e0oq); PRS Tunecode recommended — [Soundmouse/BBC deck](https://www.soundmouse.com/bbc/BBC_Music_Portal_Presentation_Template_standard_v1.1.pdf)
- Alternative to timeline parsing: **audio recognition** on the final mix (Soundmouse) — [Soundmouse/BBC](https://www.soundmouse.com/bbc/BBC_Music_Portal_Presentation_Template_standard_v1.1.pdf); hobby example [miwco/ArchiveCheck](https://github.com/miwco/ArchiveCheck)

### Inferences
- **[Schätzung] 14-day MVP is realistic** for: upload EDL/FCP7 XML/FCPXML → parse audio clips (OTIO or stdlib) → merge or dedupe per source file → durations at the user's frame rate → editable grid with usage-code dropdown and composer/publisher/PRO fields → CSV/XLSX/PDF export. AAF and Resolve .drp are harder; ask users to export FCP7 XML or FCPXML from Resolve first, as EditingTools also recommends.
- **[Schätzung] The metadata moat is the hard part.** Options:
  - read embedded ID3/BWF metadata from library WAV/MP3 files. Many libraries embed composer and publisher, but this was not verified in this session
  - build a user-contributed lookup table (track file name → rights) per workspace, so series reuse it episode to episode
  - partner with libraries for metadata feeds, the way EditingTools does
- A non-coder relying on Claude Code should constrain scope to 2–3 formats and test against real exports from his own Premiere and Resolve projects. EDL clip-name handling (comment lines) and nested sequences are classic edge cases [Schätzung].

### Gaps
- ID3/BWF/iXML metadata conventions at specific libraries (APM, Extreme, Musicbed, Artlist, Epidemic) were not researched.
- RapidCue, Soundmouse, SOCAN and APRA import file formats and specs were not found. These are needed for "submission-ready" exports.
- Which OTIO adapters support FCP7 XML, FCPXML and CMX3600 in 2026 was not confirmed from documentation, only that the core repo and AAF adapter are active.

---

## 6. Channels to the first 10 paying customers

### Takeaway
Few channel-specific sources were gathered (search budget exhausted). The evidence points to:
1. communities where cue sheets come up: Creative COW, Stage 32 Post-Production Lounge, VI-Control, MusicLibraryReport, composer Skool groups
2. **music libraries and library platforms** that already invest in cue sheet tooling (Melodie, Slipstream, SourceAudio, Harvest Media, EditingTools' 20+ partners)
3. the **Adobe Exchange** plugin marketplace, where the main competitor already distributes a free Premiere panel.

Facebook groups, newsletters and podcasts could not be researched.

### Cited Findings
- Post-production forums with cue sheet threads: [Creative COW (FCP and Avid forums)](https://creativecow.net/forums/thread/exporting-edls-for-cue-sheets/); [Stage 32 Post-Production Lounge, "Music cue sheet" (trending)](https://www.stage32.com/lounge/post_production/Music-cue-sheet)
- Composer and library communities where missing cue sheets are discussed: [VI-Control](https://vi-control.net/community/threads/ascap-missing-cue-sheets-for-several-shows-missed-royalty-payment-date-next-steps.128281/); [MusicLibraryReport forums](https://musiclibraryreport.com/forums/topic/cue-sheets-were-filed-incorrectly-what-should-i-do); [Gearspace](https://gearspace.com/threads/publisher-on-cue-sheets.1374444/); [Skool: Hit Record Academy](https://www.skool.com/hit-record-academy-7764/story-time-missing-cue-sheets)
- Libraries invest in cue sheet tools as a customer-service feature: Melodie ([Señal News 2024](https://senalnews.com/en/digital/melodie-unveiled-a-new-music-development-cue-sheet-tool)); Slipstream ([support](https://support.slipstreammusic.com/en/articles/15313476-cue-sheet-generator-beta)); PremiumBeat ([cuesheet page](https://www.premiumbeat.com/royalty-free/cuesheet)). EditingTools partners with 20+ libraries for metadata ([Manager](https://editingtools.io/cuesheetmanager/)).
- Library infrastructure platforms with cue sheet and metadata hooks: [SourceAudio cue sheets](https://docs.sourceaudio.com/administration/cue_sheets.html); [Harvest Media to Soundmouse integration (AUD 10/catalogue/month)](https://wwwcforigin.harvestmedia.net/soundmouse/)
- Plugin marketplace: EditingTools distributes its free Cue Sheet Uploader through [Adobe Exchange](https://exchange.adobe.com/publisher/cc/8b1d028e-33e1-4589-b9e6-39f67d77553a/editingtoolsio)
- Composer-facing SaaS publishes cue sheet SEO content in 2026, which suggests composers search for this — [DropCue Music Cue Sheet Guide 2026](https://dropcue.app/blog/music-cue-sheet-guide); [SyncPlacement: What Is a Cue Sheet (2026)](https://syncplacement.com/blog/what-is-a-cue-sheet/)

### Inferences
- **[Schätzung] Fastest path to 10 paying customers with $0 ads:**
  - (a) the founder's own editor network: AEs and post supervisors on doc and unscripted series, who face cue sheets every episode
  - (b) posts in Creative COW, Stage 32 and post Facebook groups offering a free first cue sheet in exchange for feedback
  - (c) **composers as referral agents**: a "send this link to your production's post team" landing page, since composers are the ones chasing (VI-Control, MLR)
  - (d) small and indie music libraries without their own cue sheet tool, as white-label or affiliate partners
- A done-for-you concierge service (upload EDL, receive a verified sheet within 24 h) could get first revenue within 30 days before the self-serve product is polished [Schätzung].
- Differentiation is required. EditingTools already sits in Adobe Exchange and holds library partnerships, and libraries give away single-catalog tools.

### Gaps
- No data on Facebook groups (e.g. "Assistant Editors", post-production groups) or their member counts. No post-production newsletters or podcasts (e.g. The Rough Cut, Art of the Cut, Frame.io Insider) were checked. No LiftGammaGain or Avid community channels checked.
- No evidence on library partnership terms or affiliate rates.
- Reddit communities (r/editors, r/postproduction, r/Filmmakers, r/WeAreTheMusicMakers) could not be accessed. Size and rules for self-promotion are unknown.
