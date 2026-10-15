# Minimal Tech Stack Costs & Terms for a Solo-Founder Paid Web App (Next.js + DB + Payments), worldwide, $50 start budget — Stand 2026-10-15

> **Method / reliability note (read first):** All accesses dated **2026-10-15**. Direct page fetching (WebFetch) failed for every vendor domain in this session (DNS error `ENOTFOUND`), so vendor facts below come from **search-engine results restricted to the vendors' own domains** (summaries/snippets of the official pages listed), not from a full read of each page. Where only third-party sources were available, this is stated. Anthropic model prices come from Anthropic's own bundled `claude-api` reference (price table marked "cached 2026-10-06"), which points to the official pricing page. The shared web-search budget ran out before video hosting, object storage and domain pricing could be checked — those are documented as **Gaps** (with clearly labelled, unverified prior knowledge only). All own calculations are labelled **[Schätzung]**.

## 1. Hosting: Vercel Hobby vs Pro, Cloudflare Workers/Pages, Netlify, Render, Railway, Fly.io

### Takeaway
Vercel Hobby is officially **non-commercial only** (taking payments = commercial), so a paid app on Vercel needs Pro (~$20/seat/month per third-party sources). The cheapest commercial-capable options are Cloudflare Workers (Free $0 / Paid $5 per month minimum), Netlify Free (300 credits, hard cap), Railway Hobby ($5 incl. $5 usage), Render free (sleeps) or $7 always-on, and Fly.io pay-as-you-go (~$2.19/month for the smallest machine).

### Cited Findings
**Vercel**
- Fair Use Guidelines: Hobby teams may use the platform only for non-commercial personal purposes; any commercial use requires Pro or Enterprise. Commercial usage explicitly includes **taking payments from visitors**, advertising a product/service, being paid to build/host the site, affiliate links as main purpose, and ads (e.g. AdSense). Asking for donations is *not* commercial — [Vercel Fair Use Guidelines](https://vercel.com/docs/limits/fair-use-guidelines); [Vercel Hobby Plan docs](https://vercel.com/docs/plans/hobby)
- Vercel Terms of Service: a hobby plan may be used only for personal or non-commercial purposes — [Vercel Terms](https://examples.vercel.com/legal/terms) (URL as surfaced by search; canonical is vercel.com/legal/terms)
- Commercial use on Hobby is a frequent trigger for a policy-based account/deployment pause — [Vercel KB: Why has my account or deployment been paused?](https://vercel.com/kb/guide/why-is-my-account-deployment-blocked)
- Pro price: $20 per seat per month, including a usage credit (one source: $20/month infrastructure credit, usage beyond billed on demand) — [Schematic: Vercel pricing](https://schematichq.com/blog/vercel-pricing); [Modelence: Vercel pricing 2026](https://modelence.com/compare/vercel-pricing). **Conflict:** one third-party source states $20/user/month billed annually vs $24/user/month billed monthly — [costbench](https://costbench.com/software/developer-tools/vercel/). Not confirmed on vercel.com/pricing in this session (third-party price checks dated Aug–Sep 2026).

**Cloudflare Workers (incl. Pages Functions)**
- Workers Paid: minimum **$5 USD/month per account**; includes Workers, Pages Functions, KV, Hyperdrive and Durable Objects usage — [Cloudflare Workers Pricing docs](https://developers.cloudflare.com/workers/platform/pricing/)
- Requests: Free = **100,000/day**; Paid = **10 million/month included, +$0.30 per additional million** — [Cloudflare Workers Pricing docs](https://developers.cloudflare.com/workers/platform/pricing/)
- CPU: Free = **10 ms CPU per invocation**; Paid = **30 million CPU-ms/month included, +$0.02 per additional million CPU-ms**; paid max CPU per invocation can be raised from 30 s default to 5 min — [Workers Pricing](https://developers.cloudflare.com/workers/platform/pricing/); [Workers Limits](https://developers.cloudflare.com/workers/platform/limits/)
- Free Worker exceeding limits returns Error 1027 — [Workers Limits](https://developers.cloudflare.com/workers/platform/limits/)

**Netlify** (credit-based plans)
- Free: **300 credits/month**, hard limit, no auto-recharge; when credits run out, **projects pause until next billing cycle** — [Netlify Pricing](https://www.netlify.com/pricing/); [Netlify docs: Credit-based pricing plans](https://docs.netlify.com/manage/accounts-and-billing/billing/billing-for-credit-based-plans/credit-based-pricing-plans/)
- Personal: **$9/month, 1,000 credits**, optional auto-recharge — [Netlify Pricing](https://www.netlify.com/pricing/); [Personal vs Free](https://www.netlify.com/pricing/personal-vs-free/)
- Pro: **from $20/month for 3,000 credits** (tiers up to 20,000 credits), unlimited seats, no per-seat charge (an older changelog said 5,000 credits — superseded) — [Netlify docs: Credit-based pricing plans](https://docs.netlify.com/manage/accounts-and-billing/billing/billing-for-credit-based-plans/credit-based-pricing-plans/); [Netlify changelog: updates to Personal and Pro](https://www.netlify.com/changelog/updates-credit-based-personal-and-pro-plans/)
- Commercial use on Free: a Netlify support-forum answer says commercial use of the free tier is welcome (but no reselling) — [Netlify Support Forums](https://answers.netlify.com/t/can-we-use-netlify-free-plan-for-commercial-purposes/41545). This is a forum answer, **not** a ToS clause.

**Render / Railway / Fly.io**
- Render: Hobby workspace $0; Free instances spin down after **15 min** without inbound traffic; **750 free instance hours/month**; Free Postgres **expires 30 days** after creation; cheapest always-on paid instance **$7/month (512 MB)** — [Render: Platforms with a real free tier 2026](https://render.com/articles/platforms-with-a-real-free-tier-for-developers-in-2026); [Render: Railway vs Fly.io (2026)](https://render.com/articles/railway-vs-fly-io) (vendor-authored articles)
- Railway: free plan gives **$5 credit in first month, then $1/month**; services pause when credits run out; **Hobby = $5/month including $5 of usage**, usage above billed — [Railway Pricing docs](https://docs.railway.com/pricing); [Railway Pricing](https://railway.com/pricing)
- Fly.io: **no free tier for new users**, pay-as-you-go, credit card required, no plan fee; shared-cpu-1x 256 MB ≈ **$2.19/month** (Ashburn), billed per second — [Fly.io: PaaS pricing compared](https://fly.io/learn/paas-pricing-compared/); [Render: Railway vs Fly.io](https://render.com/articles/railway-vs-fly-io). An older Fly community thread mentions a $5/month "hobby" plan — [Fly community](https://community.fly.io/t/free-plan-clarification/18661) — apparently outdated.

### Inferences
- A paid SaaS on Vercel Hobby violates Vercel's terms the moment it takes payments → budget **≥ $20/month** for Vercel Pro (≈ 40% of the $50 start budget per month). [Schätzung]
- Cheapest compliant Next.js hosting at launch: Cloudflare Workers Free ($0) or Paid ($5), or Netlify Free ($0, but projects pause at 300 credits — risky for a paid product), Railway Hobby ($5). [Schätzung]
- Render free (15-min sleep, 30-day Postgres expiry) is unsuitable for production paid customers; always-on starts at $7. [Schätzung]

### Gaps
- Vercel Pro price, included credit and Hobby usage limits not read directly from vercel.com/pricing (fetch failed); annual vs monthly price conflict ($20 vs $24) unresolved.
- Cloudflare's own ToS statement on commercial use of the Workers/Pages **Free** plan not retrieved in this session (no restriction surfaced in results, but not verified). Pages static-request limits and Next.js support via adapter not checked.
- Netlify's ToS on commercial use of Free not verified (only forum answer); credit-to-bandwidth/request conversion not retrieved.

## 2. Database / Auth: Supabase, Neon, Clerk, Supabase Auth

### Takeaway
Supabase Free ($0) gives 500 MB DB, 50,000 MAU and 2 free projects but **pauses after 7 days of low activity**; Pro is **$25/month** (100,000 MAU, 8 GB disk, no pausing; compute billed separately with a $10 credit per third-party sources). Neon Free gives 100 CU-hours + 1 GB per project with scale-to-zero; Launch is pay-as-you-go with no minimum ($0.106/CU-h, $0.35/GB-month). Clerk Free covers 50,000 monthly *retained* users; Pro $20/month annual ($25 monthly).

### Cited Findings
**Supabase**
- Free: **500 MB database size, 50,000 MAU**, **2 free projects**; Free projects are **paused after 1 week of inactivity** — [Supabase Pricing](https://supabase.com/pricing)
- Pausing detail: projects with low activity over a 7-day window are paused; a few user requests to the DB per day is typically enough to avoid it; paused projects can be restored from Studio within **1 year** — [Supabase docs: Project Pausing](https://supabase.com/docs/guides/platform/free-project-pausing)
- Pro: **$25/month**, **100K MAU** and **8 GB disk per project** included; paid projects are not paused — [Supabase Pricing](https://supabase.com/pricing)
- Auth overage (Pro/Team): **$0.00325 per MAU** above 100,000 — [Supabase docs: Manage MAU usage](https://supabase.com/docs/guides/platform/manage-your-usage/monthly-active-users)
- Database size ≠ disk size (provisioned disk) — [Supabase docs: Compute and Disk](https://supabase.com/docs/guides/platform/compute-and-disk)
- Third-party: Pro DB storage overage $0.125/GB over 8 GB; **$10/month compute credit covers one Micro instance (1 GB RAM)**; compute billed on top of the $25 and runs 24/7 (no scale-to-zero); spend cap on by default; free-tier egress 5 GB, file storage 500 MB — [Activepieces: Supabase pricing](https://www.activepieces.com/blog/supabase-pricing-free-tier-limits-pro-costs-egress.md); [Jetadmin: Supabase Pricing 2026](https://www.jetadmin.io/blog/supabase-pricing-2026-guide-to-plans-limits-and-real-world-costs/). **Conflict on Pro egress:** 250 GB vs 50 GB between third-party sources.

**Neon**
- Free: **$0/month, 100 CU-hours compute per project, 1 GB storage per project (20 GB account total)**; FAQ: up to **100 projects** — [Neon docs: Plans](https://neon.com/docs/introduction/plans); [Neon FAQ: Free plan limits](https://neon.com/faqs/free-plan-limits-and-quotas)
- When Free CU-hours run out, compute is **suspended** until next billing period or upgrade; no overage billing on Free — [Neon FAQ: Free plan limits](https://neon.com/faqs/free-plan-limits-and-quotas)
- Launch: **pay-as-you-go, no monthly minimum, $0.106 per CU-hour, $0.35 per GB-month** — [Neon docs: Plans](https://neon.com/docs/introduction/plans); price cut from $0.14 to $0.106/CU-h — [Neon blog](https://neon.com/blog/major-compute-price-reduction-on-neon)
- CU-hour = compute size × hours running (0.25 CU × 4 h = 1 CU-hour) — [Neon docs: Plans](https://neon.com/docs/introduction/plans)
- **Conflict:** some Neon FAQ pages say 0.5 GB storage per Free project; current plans docs say 1 GB (docs treated as authoritative) — [Neon docs: Plans](https://neon.com/docs/introduction/plans)

**Clerk**
- Free: first **50,000 monthly retained users (MRU)** and 100 monthly retained orgs; a user counts as retained only if they return ≥ 24 h after sign-up — [Clerk Pricing](https://clerk.com/pricing)
- Pro: **$20/month billed annually or $25/month monthly**, 50K MRU included, overage from **$0.02/MRU/month** with volume discounts — [Clerk Pricing](https://clerk.com/pricing); [Clerk: Pricing explained](https://clerk.com/articles/clerk-pricing-explained)
- Older 10,000-MAU free tier (Clerk blog) is outdated — [Clerk blog: new pricing plans](https://clerk.com/blog/new-pricing-plans)

### Inferences
- A live paid app with daily users will normally not trigger Supabase Free pausing (pausing is based on 7-day low activity), but a pre-launch/low-traffic project can be paused. [Schätzung]
- Auth cost per customer at small scale is **$0** on Supabase Auth (≤50k MAU) or Clerk Free (≤50k MRU); auth is not a unit-economics driver until tens of thousands of users. [Schätzung]
- Neon 0.25 CU running 24/7 ≈ 0.25 × 730 h ≈ 182 CU-h/month → exceeds the 100 CU-h Free allotment unless scale-to-zero idles it; on Launch that would be ≈ 182 × $0.106 ≈ **$19.3/month** compute + storage. [Schätzung]

### Gaps
- Supabase Pro included egress (50 vs 250 GB), Free-tier egress/storage and backup policy not verified on supabase.com.
- Neon Free: exact minimum/maximum autoscaling size and scale-to-zero delay not retrieved.

## 3. Payments for global sales: Stripe fees, Billing, Tax; Merchant-of-Record options (Paddle, Lemon Squeezy, Polar, Stripe Managed Payments)

### Takeaway
Stripe (US pricing) = **2.9% + 30¢**, +1.5% international cards, +1% currency conversion, +0.7% Billing for subscriptions, +0.5% Stripe Tax Basic (where registered) — but then the founder must register/file VAT/sales tax himself. MoR options that take on tax liability: **Paddle 5% + 50¢**, **Lemon Squeezy 5% + 50¢ (+1.5% intl, +0.5% subscriptions)**, **Polar Starter 5% + 50¢ (+1.5% intl; paid plans down to 3.4% + 30¢)**, **Stripe Managed Payments: +3.5% on top of standard Stripe fees** (official Stripe help page; a third-party claims 5% + 50¢ — conflict). Lemon Squeezy is steering users to Stripe Managed Payments.

### Cited Findings
**Stripe standard (US pricing page)**
- Domestic cards **2.9% + 30¢**; manually entered cards **+0.5%**; international cards **+1.5%**; currency conversion **+1%** — [Stripe Pricing](https://stripe.com/pricing)
- Euro-region page (Spain variant): **1.5% + €0.25 standard EEA cards**, 2.8% + €0.25 premium EEA cards, **3.15% + €0.25 international cards, +2% currency conversion** — [Stripe Pricing (ES)](https://stripe.com/en-es/pricing) (values from search summary; verify on the German page stripe.com/de/pricing)
- Stripe Billing pay-as-you-go: **0.7% of Billing volume**, no recurring fee (subscription plan option: 0.67% above tier cap; a page snapshot may be stale) — [Stripe Billing Pricing](https://stripe.com/billing/pricing); [Stripe support: Billing Starter/Scale changes](https://support.stripe.com/questions/changes-to-the-stripe-billing-starter-and-scale-plans). Usage-based billing via Metronome listed at 0.8% — [Stripe Pricing](https://stripe.com/pricing)
- Stripe Tax: **Tax Basic 0.5% per transaction where you're registered to collect** (or $0.50 per transaction via API); Tax Complete listed "starting at $620/month" on 1-year contract (inconsistent with other figures seen — verify) — [Stripe Pricing](https://stripe.com/pricing); [Stripe support: Understanding Stripe Tax pricing](https://support.stripe.com/questions/understanding-stripe-tax-pricing)
- Adaptive Pricing (local-currency display): no merchant fee; the customer-facing FX rate includes a **2–4% conversion fee** paid by the customer — [Stripe docs: Adaptive Pricing](https://docs.stripe.com/payments/currencies/localize-prices/adaptive-pricing); [Stripe support: Adaptive Pricing](https://support.stripe.com/questions/adaptive-pricing)

**Stripe Managed Payments (Stripe's MoR)**
- Fee: **3.5% per successful transaction on top of standard processing fees**, calculated on the full amount **including indirect taxes (VAT/sales tax)** — [Stripe support: Managed Payments pricing](https://support.stripe.com/questions/managed-payments-pricing). **Conflict:** third-party sources claim 5% + $0.50 (same as Lemon Squeezy) — [Dodo Payments: Lemon Squeezy vs Stripe](https://dodopayments.com/blogs/lemon-squeezy-vs-stripe/) (competitor-authored). Stripe's own help page preferred.
- Availability: generally available to businesses in **39 countries** (incl. new support for Australia) — [Stripe docs: Managed Payments changelog](https://docs.stripe.com/payments/managed-payments/changelog); GA for businesses in **Germany** announced at Stripe Tour Berlin 2026 — [Stripe Newsroom](https://stripe.com/newsroom/news/stripe-tour-berlin-2026)
- Scope: digital products (SaaS, software, digital content/downloads); requires tax codes marked "Eligible for Managed Payments"; Stripe handles indirect tax in **80+ countries**; works with **Checkout and Payment Links**; customer sees **Link** as merchant of record; can be applied to entire business or specific markets/products — [Stripe docs: Managed Payments](https://docs.stripe.com/payments/managed-payments); [How it works](https://docs.stripe.com/payments/managed-payments/how-it-works); [Set up](https://docs.stripe.com/payments/managed-payments/set-up)
- Third-party: not compatible with Elements; subscriptions still need Stripe Billing; no affiliate tools/storefront — [Dodo Payments: Lemon Squeezy vs Stripe](https://dodopayments.com/blogs/lemon-squeezy-vs-stripe/) (competitor-authored, unverified)

**Paddle**
- MSA: Paddle Checkout discount **5% of SRP + $0.50**; Paddle may apply alternative structures at its discretion — [Paddle Master Services Agreement](https://www.paddle.com/legal/terms)
- Marketing: "Total cost: 5% + 50¢" covering payments, subscription billing, global tax & compliance, fraud/chargebacks, buyer support; Paddle as reseller takes full sales-tax liability; custom pricing for larger companies — [Paddle MoR 101](https://www.paddle.com/paddle-101); [Paddle vs Stripe](https://www.paddle.com/compare/stripe)

**Lemon Squeezy (Stripe-owned)**
- Base fee **5% + 50¢**, no monthly fee; surcharges **+1.5% international (non-US) transactions, +1.5% PayPal, +0.5% subscription payments** — [Lemon Squeezy Pricing](https://www.lemonsqueezy.com/pricing); [Lemon Squeezy docs: Fees](https://docs.lemonsqueezy.com/help/getting-started/fees)
- 2026 update: Lemon Squeezy describes Stripe Managed Payments as Stripe's MoR (merchants in 35+ countries) and states its goal is an easy migration path for LS users to Stripe Managed Payments (related-articles date Jan 28, 2026) — [Lemon Squeezy: 2026 Update](https://www.lemonsqueezy.com/blog/2026-update)
- Third-party: acquisition by Stripe in 2024 (month varies by source: April/July/Sept 2024) — [fungies.io](https://fungies.io/lemon-squeezy-stripe-acquisition-saas-founders-2026/) (competitor)

**Polar**
- Plans: **Starter free, 5% + 50¢**; **Pro $20/month, 3.8% + 40¢**; **Growth $100/month, 3.6% + 35¢**; **Scale $400/month, 3.4% + 30¢**; switchable anytime — [Polar Pricing](https://polar.sh/resources/pricing); [Polar docs: Fees](https://polar.sh/docs/merchant-of-record/fees)
- Orgs created **before May 27, 2026** keep legacy 4% + 40¢ + 0.5% subscription fee (not available to new orgs) — [Polar docs: Fees](https://polar.sh/docs/merchant-of-record/fees)
- Extras: **+1.5% international (non-US) cards**; payouts **$2/month of active payouts + 0.25% + $0.25 per payout**, plus cross-border conversion fees — [Polar docs: Fees](https://polar.sh/docs/merchant-of-record/fees)
- Polar worked example: $37.50 transaction ($30 + 25% Swedish VAT), international card → fees $2.94 (Starter), $2.39 (Pro), $2.26 (Growth), $2.14 (Scale) — i.e. fee charged on VAT-inclusive amount — [Polar docs: Fees](https://polar.sh/docs/merchant-of-record/fees)

### Inferences
Fee per **$10.00 net monthly subscription payment** (no VAT on top unless stated) [Schätzung, own arithmetic from cited rates]:

| Option | US card | Non-US card (+ FX where applicable) | Tax compliance |
|---|---|---|---|
| Stripe (US account) + Billing 0.7% | 0.29+0.30+0.07 = **$0.66 (6.6%)** | (2.9+1.5+1.0)% → 0.54+0.30+0.07 = **$0.91 (9.1%)** | founder's job; +Tax Basic 0.5% = +$0.05 where registered |
| Stripe Managed Payments (+3.5%, + Billing 0.7%) | 0.29+0.30+0.35+0.07 = **$1.01** | 0.54+0.30+0.35+0.07 = **$1.26** | Stripe as MoR (80+ countries) |
| Paddle 5% + 50¢ | **$1.00 (10%)** | **$1.00** (no intl surcharge surfaced) | Paddle as MoR |
| Lemon Squeezy 5%+50¢ +0.5% sub (+1.5% intl) | **$1.05** | **$1.20 (12%)** | LS as MoR |
| Polar Starter 5%+50¢ (+1.5% intl) | **$1.00** | **$1.15** | Polar as MoR |
| Polar Pro ($20/mo) 3.8%+40¢ (+1.5% intl) | **$0.78** | **$0.93** | Polar as MoR |

- MoR fees are typically computed on the VAT-inclusive amount (explicit for Stripe MP and Polar's example): a €10 net price with 19% German VAT (€11.90 gross) on Paddle ≈ 0.595 + 0.50 ≈ **$1.10** equivalent. [Schätzung]
- The fixed 50¢ component dominates at low prices: at a $5/month price, Paddle/Polar Starter ≈ $0.75 (15%); at $29/month ≈ $1.95 (6.7%). [Schätzung]
- Polar Pro ($20/month) breaks even vs Starter when savings (1.2% × price + $0.10 per transaction) × transactions ≥ $20 → at $10 price ≈ **91 transactions/month**; at $29 ≈ 45. [Schätzung]
- For a German solo founder selling B2C worldwide, an MoR (Paddle/Polar/LS/Stripe MP) avoids EU OSS + foreign VAT/GST registrations; Stripe direct is cheaper per transaction but shifts tax registration/filing to the founder. [Schätzung]

### Gaps
- Stripe Germany/EU pricing page not read directly; premium-card and international rates (2.8%/3.15%) come from a search summary of the Spanish page and may differ from DE.
- Whether Stripe Billing 0.7% applies on top of Managed Payments for subscriptions is not confirmed by Stripe (only third-party).
- Paddle: whether "SRP" is gross (incl. tax) or net, and any international/PayPal surcharges, not confirmed; Paddle pricing page last-update date unknown.
- Lemon Squeezy: whether new sign-ups are still accepted and whether Stripe Managed Payments has open public sign-up was not confirmed on 2026-10-15.
- Payout/FX fees for non-USD payouts (Paddle, LS) not retrieved.

## 4. Transactional Email: Resend, Postmark, Amazon SES

### Takeaway
Resend Free = 3,000 emails/month (100/day), Pro $20/month for 50,000; Postmark Free = 100/month, then $15/month for 10,000; Amazon SES ≈ $0.10 per 1,000 emails, but the 12-month SES free tier ended for new customers on 2026-07-21 and SES now has plans (Essentials/Pro/Enterprise).

### Cited Findings
- Resend Free: **3,000 emails/month, limited to 100 emails/day** — [Resend docs: account quotas and limits](https://resend.com/docs/knowledge-base/account-quotas-and-limits); [Resend Pricing](https://resend.com/pricing)
- Resend Pro: **$20/month for 50,000 emails**, overage **$0.90 per 1,000**; no daily limit on paid plans — [Resend Pricing](https://resend.com/pricing); [Resend docs: What is Resend pricing](https://resend.com/docs/knowledge-base/what-is-resend-pricing)
- Postmark: free developer plan **100 emails/month**, never expires; next tier **$15/month for 10,000 emails**, overage **$1.80 per 1,000** (Basic); no tier between 100 and 10,000 — [Postmark Pricing](https://postmarkapp.com/pricing) (search snapshot may be old — verify)
- Amazon SES: pay-as-you-go **$0.10 per 1,000 emails** (plus attachment charges); **as of July 21, 2026 the SES free tier (3,000 message charges/month for 12 months) is no longer available to new customers**; new accounts start on the **Essentials** plan (plans: Essentials, Pro, Enterprise) — [AWS blog: Introducing Amazon SES pricing plans](https://aws.amazon.com/blogs/messaging-and-targeting/introducing-amazon-simple-email-service-ses-pricing-plans/); [Amazon SES FAQs](https://aws.amazon.com/ses/faqs/)

### Inferences
- Typical SaaS customer generating ~10 transactional emails/month: on Resend Free, 3,000/month ≈ 300 customers before upgrade (100/day cap binds earlier on bursty days); marginal cost on Resend Pro overage ≈ $0.009/customer/month; on SES ≈ $0.001/customer/month. [Schätzung]

### Gaps
- Price of SES Essentials plan (monthly fee, if any) not retrieved.
- Postmark current pricing page date not verified (snapshot possibly ~3 years old per search metadata).

## 5. AI APIs: Anthropic Claude prices + PDF-extraction cost; transcription (OpenAI, AssemblyAI, Deepgram)

### Takeaway
Cheapest current Claude model is **Claude Haiku 5.5 at $0.10 input / $0.50 output per million tokens** (prompts ≤100K tokens) → a 2-page PDF extraction (3,000 in / 500 out) costs ≈ **$0.00055** (~$0.55 per 1,000 PDFs), ~$0.0003 with Batch (–50%). Transcription: AssemblyAI Universal-2 $0.15/h is cheapest found; OpenAI gpt-4o-mini-transcribe $0.003/min ($0.18/h) but **OpenAI's current transcription models are deprecated, shutdown 2027-02-26**.

### Cited Findings
**Anthropic (Claude API, first-party prices per 1M tokens, input / output)** — source: Anthropic's bundled `claude-api` reference, table "Current Models (cached: 2026-10-06)", which cites the official page [platform.claude.com/docs/en/about-claude/pricing](https://platform.claude.com/docs/en/about-claude/pricing) (official page itself could not be fetched in this session):
- Claude Haiku 5.5 (`claude-haiku-5-5`): **$0.10 / $0.50** for prompts ≤100K tokens; **$0.50 / $2.50** above 100K; 1M context — [Anthropic pricing](https://platform.claude.com/docs/en/about-claude/pricing)
- Claude Haiku 4.5: **$1.00 / $5.00** (200K context) — [Anthropic pricing](https://platform.claude.com/docs/en/about-claude/pricing); consistent with [Finout](https://finout.io/blog/anthropic-api-pricing), [MetaCTO](https://metacto.com/blogs/anthropic-api-pricing-a-full-breakdown-of-costs-and-integration)
- Claude Sonnet 5.5 / Sonnet 5: **$2.00 / $10.00**; Sonnet 4.6: **$3.00 / $15.00** — [Anthropic pricing](https://platform.claude.com/docs/en/about-claude/pricing)
- Claude Opus 5.5: **$4.00 / $20.00**; Opus 5 / 4.8 / 4.7 / 4.6: **$5.00 / $25.00** — [Anthropic pricing](https://platform.claude.com/docs/en/about-claude/pricing)
- Claude Fable 5.1 / Fable 5: **$10.00 / $50.00** (Mythos 5.1 same price, Project Glasswing only) — [Anthropic pricing](https://platform.claude.com/docs/en/about-claude/pricing)
- Batch API: **50% off every token in the request, including cache reads/writes**; asynchronous — [Anthropic batch processing docs](https://platform.claude.com/docs/en/build-with-claude/batch-processing.md) (as summarized in Anthropic's claude-api reference)
- Haiku 5.5 caveats: adaptive thinking **on by default** (effort default `medium`; thinking can be disabled at effort `high` or below); thinking is billed regardless of whether it is displayed; **new tokenizer counts the same text as ~30% more tokens** than Haiku 4.5 — Anthropic `claude-api` reference, models section (official model overview: [platform.claude.com/docs/en/about-claude/models/overview](https://platform.claude.com/docs/en/about-claude/models/overview.md))
- PDF input: native PDF document blocks supported; limits 32 MB/request, 600 pages (100 for 200K-context models) — Anthropic `claude-api` reference
- Note: March-2026-era third-party aggregators list only Haiku 4.5 ($1/$5), Sonnet 4.6 ($3/$15), Opus 4.6 ($5/$25) as current — [MorphLLM](https://www.morphllm.com/anthropic-claude-api-pricing); these figures match Anthropic's table for those models; newer models (Haiku/Sonnet/Opus 5.5) postdate those articles.

**Transcription**
- OpenAI **gpt-4o-transcribe**: $2.50 input / $10.00 output per 1M tokens, est. **$0.006/minute**; **gpt-4o-mini-transcribe**: $1.25 / $5.00 per 1M tokens, est. **$0.003/minute** — [OpenAI Pricing](https://platform.openai.com/docs/pricing/); [gpt-4o-mini-transcribe model page](https://developers.openai.com/api/docs/models/gpt-4o-mini-transcribe)
- OpenAI changelog (Aug 2026): **whisper-1, gpt-4o-transcribe, gpt-4o-mini-transcribe, gpt-4o-transcribe-diarize deprecated, shutdown 2027-02-26**; migrate to **gpt-transcribe / gpt-live-transcribe** — [OpenAI Changelog](https://developers.openai.com/api/docs/changelog?mw_entry=2026-08-20-974ac0734e053853)
- whisper-1 historically $0.006/min (community posts, 2023; users reported higher real costs) — [OpenAI community](https://community.openai.com/t/api-model-whisper-real-cost/469816) (old, unofficial)
- AssemblyAI pre-recorded: **Universal-3.5 Pro ≈ $0.21/hour, Universal-2 ≈ $0.15/hour**, pay-as-you-go, billed per second, no minimums; add-ons (diarization, Medical Mode) extra — [AssemblyAI: Pre-recorded STT](https://www.assemblyai.com/products/speech-to-text); [AssemblyAI blog: speech recognition cost](https://www.assemblyai.com/blog/speech-recognition-cost). Older AssemblyAI pages cite $0.37/h and $0.27/h (stale).
- Deepgram Nova-3 pre-recorded: **$0.0043/minute (≈ $0.258/hour)** — [Deepgram: Best STT APIs 2026](https://deepgram.com/learn/best-speech-to-text-apis-2026) (Deepgram blog, not the pricing page)

### Inferences
PDF field extraction, 2-page PDF ≈ 3,000 input + 500 output tokens [Schätzung, own arithmetic]:
- **Haiku 5.5:** 3,000 × $0.10/1M = $0.00030 + 500 × $0.50/1M = $0.00025 → **$0.00055 per PDF** (≈ $0.55 per 1,000 PDFs); Batch: **≈ $0.000275**.
- With Haiku 5.5's ~30% higher token count (3,900 in / 650 out): ≈ **$0.00072**; plus e.g. 1,000 thinking tokens if thinking not disabled: +$0.0005 → ≈ **$0.0012** worst-case-ish.
- If the PDF is sent as a native document (pages also processed as images), input may well exceed 3,000 tokens; even at 10,000 input tokens: $0.0010 + $0.00025 = **$0.00125**.
- Comparison per PDF: Haiku 4.5 = $0.0030 + $0.0025 = **$0.0055**; Sonnet 5.5 = $0.006 + $0.005 = **$0.011**; Opus 5.5 = $0.012 + $0.010 = **$0.022**.
- → Even 500 PDFs/customer/month on Haiku 5.5 ≈ $0.28–0.60/customer/month; AI cost is not the unit-economics bottleneck for extraction — payment fees are.

Transcription per customer (example: 10 audio hours/month) [Schätzung]: AssemblyAI Universal-2 ≈ **$1.50**; Universal-3.5 Pro ≈ $2.10; gpt-4o-mini-transcribe ≈ $1.80; Deepgram Nova-3 ≈ $2.58; gpt-4o-transcribe ≈ $3.60.

### Gaps
- Official Anthropic pricing page not fetched directly in this session (values from Anthropic's own reference table cached 2026-10-06); verify Haiku 5.5's $0.10/$0.50 on the live page before publishing.
- Real token count of a 2-page PDF for Haiku 5.5 not measured (use `count_tokens` endpoint).
- Prices for OpenAI's replacement models gpt-transcribe / gpt-live-transcribe not found.
- Deepgram's own pricing page and free-credit amount not retrieved; AssemblyAI free credits not retrieved.

## 6. Video & Object Storage: Bunny Stream, Cloudflare Stream, Mux, Cloudflare R2, Backblaze B2

### Takeaway
**Not verified in this session** — the shared web-search budget was exhausted before these vendors could be checked and direct page fetches failed. Only clearly labelled, unverified prior knowledge is given below; it must be re-checked before use in unit economics.

### Cited Findings
- No findings retrieved from official sources on 2026-10-15.

### Inferences
- UNVERIFIED prior knowledge (model training data, not checked 2026-10-15) — **[Schätzung, unverifiziert]**: Cloudflare R2 ≈ $0.015/GB-month storage, **zero egress fees**, free tier ~10 GB-month; Cloudflare Stream ≈ $5 per 1,000 minutes stored + $1 per 1,000 minutes delivered, no encoding fee; Bunny Stream: free encoding, storage ≈ $0.01/GB per region, CDN delivery from ≈ $0.005–0.01/GB depending on network tier; Backblaze B2 ≈ $6–7/TB-month with free egress up to ~3× stored volume (a price increase may have occurred); Mux: usage-based per-minute encoding/storage/delivery with a free/basic tier — amounts unknown.
- Structural point (likely stable but unverified): per-minute pricing (Cloudflare Stream, Mux) is easier to model per customer; per-GB pricing (Bunny, R2/B2) depends on bitrate. [Schätzung]

### Gaps
- All current prices for Bunny Stream, Cloudflare Stream, Mux, Cloudflare R2 and Backblaze B2 — needs follow-up search (official pages: bunny.net/pricing/stream, developers.cloudflare.com/stream/pricing, mux.com/pricing, developers.cloudflare.com/r2/pricing, backblaze.com/cloud-storage/pricing).

## 7. Domain: .com at Cloudflare Registrar / Namecheap

### Takeaway
**Not verified in this session** (search budget exhausted). Cloudflare Registrar sells at registry cost without markup (policy, prior knowledge); a .com is roughly $10–12/year there [Schätzung, unverifiziert]; Namecheap typically has a cheaper first year and a higher renewal.

### Cited Findings
- No findings retrieved from official sources on 2026-10-15.

### Inferences
- **[Schätzung, unverifiziert]** .com at Cloudflare Registrar ≈ $10.5–11.5/year (registry wholesale + ICANN fee, no markup); Namecheap ≈ first-year promo price below that, renewal ≈ $15–19/year. Budget **≈ $12/year** for the $50 plan to be safe.

### Gaps
- Current Verisign .com wholesale price and Cloudflare/Namecheap retail prices as of Oct 2026 not verified.

## 8. Synthesis: minimal stack within $50 and per-customer unit economics

### Takeaway
A compliant, near-zero fixed-cost stack is feasible: Cloudflare Workers (Free/$5) + Supabase Free or Neon Free + Supabase Auth/Clerk Free + Resend Free + MoR without monthly fee (Paddle/Polar Starter/LS) + Claude Haiku 5.5 → fixed costs ≈ $0–5/month + domain ≈ $12/year. Choosing Vercel Pro ($20) + Supabase Pro ($25) would consume ~$45/month, i.e. the whole $50 budget in month one. Variable cost per customer is dominated by payment/MoR fees (≈ 7–12% of a $10 price), not AI or email.

### Cited Findings
- (All inputs cited in sections 1–5.) Vercel Hobby forbids taking payments — [Vercel Fair Use Guidelines](https://vercel.com/docs/limits/fair-use-guidelines); Workers Paid min $5 — [Cloudflare Workers Pricing](https://developers.cloudflare.com/workers/platform/pricing/); Supabase Pro $25 — [Supabase Pricing](https://supabase.com/pricing); Paddle 5% + $0.50 — [Paddle MSA](https://www.paddle.com/legal/terms); Polar Starter 5% + 50¢ — [Polar docs: Fees](https://polar.sh/docs/merchant-of-record/fees); Resend Free 3,000/month — [Resend Pricing](https://resend.com/pricing).

### Inferences
Fixed monthly cost scenarios [Schätzung]:
- **Lean:** Cloudflare Workers Paid $5 + Supabase Free $0 + Resend Free $0 + Polar Starter/Paddle $0 + domain ~$1/month (amortized) → **≈ $6/month** → $50 lasts ~8 months (before any revenue).
- **Vercel route:** Vercel Pro $20 + Supabase Free $0 + domain → **≈ $21/month** → ~2 months.
- **"Comfort" route:** Vercel Pro $20 + Supabase Pro $25 (+compute beyond $10 credit possible) → **≈ $45+/month** → budget exhausted in month 1.

Variable cost per paying customer at $10/month (Paddle or Polar Starter, US buyer; 500 Haiku-5.5 PDF extractions; 10 emails via Resend Free) [Schätzung]: payments $1.00 + AI ≈ $0.28–0.60 + email $0 → **≈ $1.30–1.60 (13–16%)**, contribution margin ≈ **$8.40–8.70**. With international card on Lemon Squeezy: payments $1.20 → ≈ $1.50–1.80.

### Gaps
- Video/storage and domain prices (sections 6–7) must be verified before including in unit economics.
- Stripe-direct route additionally requires VAT/OSS registration costs and tax-adviser time, not quantified here.
