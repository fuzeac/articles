## Dek / Subtitle
A Telegram‑native consumer app for Web3 that prioritizes verification, safety, and recourse—while rewarding participation. Designed for communities; built for investors who care about defensibility and scale.

<!-- Image: “Hero — clean Telegram UI mock with ‘Verified’ badge, wallet card, dispute/recourse ribbon” -->

## TL;DR
- **Verification + Safety** first: role‑based verification, rate limits, and idempotent transactions to prevent double charges and abuse.
- **Wallets & Payments** with guardrails: Stars ↔ FZ points, withdrawal queues, receipts, and dispute resolution with refunds when things go wrong.
- **Real Community Mechanics**: referrals, daily rewards, watchlists, alerts, and events to turn passive chats into productive networks.
- **Privacy by Design**: minimal data, no raw IP storage, k‑anonymous analytics, and clear consent paths.
- **Investor‑grade Discipline**: error transparency, SLOs, observability, and a roadmap to escrow and governance—moats that compound.

<!-- Image: “TL;DR cards — Verification, Payments, Community, Privacy, Discipline” -->

## The Problem
Crypto communities mostly live on Telegram. That’s where alpha, presales, and scams collide. Newcomers don’t know who to trust. Builders struggle to show credible signals. Investors can’t see governance, recourse, or risk controls in one place.

Real user pain looks like this:
- *“I clicked a link and paid, then nothing happened.”*
- *“We can’t verify who’s real without doxxing.”* (glossary: **doxxing** = publicly exposing personal identity)
- *“Project pages are hypey; there’s no consistent way to compare them.”*
- *“Group alerts spam at 3 a.m.; I muted everything and missed the real updates.”*
- *“If something breaks, nobody tells me what happened or what to do next.”*

## Our Solution
We built a Telegram‑first app with **explicit business rules** that make Web3 usable. Every major flow—verification, wallets, rewards, events, listings, alerts—has **clear policies, edge‑case handling, and acceptance criteria**. The goal is simple: **safety you can feel, utility you can use.**

> “Rules aren’t red tape; they’re how we make crypto behave like software with guarantees.” — *Founder*

### What that means in practice
- **Idempotency on every money/identity change** (safe retries, no double charges) and **plain‑language error messages** you can act on.
- **Verification gates** that unlock features without forcing public identity; users prove what’s needed for the feature—no more, no less.
- **Rate limits, fraud checks, and quiet hours** so alerts and outreach stay helpful, not predatory.
- **Refund/recourse** paths for boosted listings, alerts, and escrow; actions are logged and reproducible.
- **Privacy‑first analytics:** no raw IP retention; cohort‑level counts with weekly salt rotation (k‑anonymous).
- **Investor visibility:** health checks, status updates during incidents, and signed receipts where it matters (escrow, fee sharing, governance).

<!-- Image: “Flow map — Verify → Participate → Earn → Escrow → Govern” -->

## How It Works (Plain English)

### Verification & Safety
Users apply for roles (e.g., **Investor**, **Project Owner**, **Validator**) and submit only the proofs required for those roles. Reviews can be approved or denied; either way, the decision is logged. Approved roles **unlock gated features** (like investing or creating listings) and can be revoked if abused. *Result: fewer bots, more accountability.*

**Trust signals** include visible badges, consistent decisions (backed by acceptance criteria), and an audit trail. Rate limits and reputation weighting curb floods and brigading.

### Wallets & Transactions (Risk‑Reduced Flows)
Inside the app you’ll see **Stars** (platform currency) and **FZ** (points). Top‑ups and withdrawals are processed with **queue states** you can track. Every payment mutation is **idempotent**, so if a Telegram reconnect forces a retry, you won’t be charged twice. **Daily check‑ins** add +5 FZ; redemptions burn points atomically and issue a receipt.

For digital‑asset trades, we are rolling out **Stars‑settled escrow** (ETH/USDC/USDT on Ethereum) with **seller‑escrow‑first** mechanics: the asset is locked on‑chain before Stars are collected, and **release occurs only when both sides’ conditions are met**. If details change after invoice (like the destination address), the trade is **re‑quoted** or must go through **dispute resolution**—never a silent failure.

> “You shouldn’t need to trust a stranger to trade. You should be able to trust the rules.” — *Founder*

### Rewards & Loyalty
The app rewards **consistent, healthy participation**: daily check‑ins, fair streaks, and referral bonuses (three tiers with cooldowns and anti‑sybil checks). Everything is logged; duplicate triggers are deduped; suspicious webs are held. *You earn by contributing—not by spamming.*

### Events & Community Mechanics
We ingest **event signals** (e.g., from Luma) and display momentum with drift guards (so numbers stay believable). **Connections** work like “friend requests” with **auto‑accept when both sides agree** and **14‑day pending expiry** to keep inboxes clean. **Watchlists & Alerts** let you follow topics with backoff and **quiet hours (22:00–07:00)** so you don’t get pinged in the middle of the night.

### Refunds & Recourse
Boosted listings that are taken down for fraud are **refunded automatically**. Escrow disputes have a documented path with longer windows for low‑rep sellers. **All sensitive operations emit an audit log**, so moderators can review and users can understand outcomes.

### Privacy, Rate Limits & Trust Signals
We minimize and protect personal data: **no raw IP storage**, export/delete requests are queued and rate‑limited, and consent is explicit. **Token‑bucket rate limits** protect money flows and messaging—keeping the experience useful, not noisy. The product exposes **reliability signals** (status pages, latency/error monitors) to build trust over time.

> “Our promise isn’t perfection. It’s **predictability**—and a clear path when things go wrong.” — *Founder*

## Why It’s Different / Defensibility
- **Clear, enforceable rules** across verification, payments, and community mechanics—published, testable, and user‑visible.
- **Network effects** that reward *healthy* behavior: referrals, watchlists, alerts, and events create compounding discovery without spam.
- **Operational moats**: idempotency, dispute/recourse systems, signed payout summaries, and governance receipts are non‑trivial to copy.
- **Unit‑economics signals** (underway): weekly fee pools split to contributors with minimum thresholds to avoid dust, plus transparent summaries (signatures).  
- **Privacy posture** that respects users and reduces regulatory risk: less data stored, less to breach.

Compared to typical “hype feed” tools, we focus on **safety, outcomes, and reproducibility**, not countless tabs and unclear rules.

## Traction & Proof
- **Pilot underway** for verification, rewards, and alerts with staged rollouts.
- Events ingestion, investor gating, and portfolio pricing are in **progress** with safeguards already defined.
- Escrow and governance are in **sequenced pilots** (see Roadmap).  
*Metrics forthcoming*—we will publish adoption and reliability stats as modules graduate from pilot to GA.

## Roadmap & What’s Next
**Near‑term (next 1–2 months)**
1. **Verification → Investor Gating** live for selected cohorts.  
2. **Listings + Refund Logic** with reproducible vote tallies and takedowns.  
3. **Events Ingestion** with drift guards and staleness indicators.  
4. **Rewards & Referrals** steady‑state launch (multipliers and fraud holds).  

**Mid‑term (quarter)**
1. **Stars‑Settled Escrow (Ethereum)** with address‑locking, slippage guards, and dispute flows.  
2. **Fee Sharing Epochs**: signed weekly summaries; minimum payout logic to avoid dust.  
3. **Governance (DAO‑lite)**: proposals, votes, timelocks, and **enactment receipts**.  
4. **BTC Pulse** snapshots for market context.  

**Honest Risks & Assumptions**
- Verification quality (false positives/negatives) needs continuous tuning.  
- Escrow UX must balance safety with speed; we will iterate with clear metrics.  
- External dependencies (price oracles, event sources) can drift; we show provenance and staleness warnings.

## Governance & Community
Anyone can read proposals; verified participants can **submit and vote** within timed windows. Decisions, votes, and enactments are **public and signed**. Community members can join as **Curators** or **Validators** to help maintain quality and earn part of the weekly fee pool.

**How to participate today**
- Get verified for the role that fits you (Investor, Project Owner, Curator, Validator).  
- Join events, set watchlists, and turn on alerts (quiet hours respected).  
- Refer high‑quality participants—rewards accrue across three tiers.

## Call to Action
**For Investors**
- Review the verification policy and investor gating details.  
- Join the pilot cohort and help shape governance and escrow guardrails.  
- Subscribe for quarterly reliability and economics updates.

**For the Community**
- Claim your username, verify your role, and start earning through healthy participation.  
- Use watchlists and alerts to keep your signal high and your noise low.  
- Report suspicious behavior—refunds and recourse exist for a reason.

> **Disclaimer:** Nothing in this article is investment advice. No promises of returns are made or implied.

<!-- Image: “Governance — proposal card with voting window and enactment receipt badge” -->
<!-- Image: “Escrow — seller‑escrow‑first diagram with check marks for both conditions required” -->
<!-- Image: “Privacy — k‑anonymous analytics concept art: cohorts not individuals” -->

## FAQ
1) **How do you keep people from gaming referrals?**  
We bind the inviter on first use, dedupe duplicate events, apply cooldowns, and hold suspicious webs until reviewed.

2) **What if I pay and the listing is taken down?**  
Fraudulent boosts are refunded automatically; actions are logged and reproducible.

3) **Will you leak my personal data?**  
We minimize collection, do not store raw IPs, and support export/delete requests with rate limits and audit logs.

4) **What happens if the app crashes during payment?**  
Idempotency ensures a safe retry—either the original result returns or nothing changes. You also get a readable error envelope.

5) **Can I change the destination address after opening an escrow trade?**  
Before payment, changes trigger a re‑quote. After payment, a dispute is required to protect both parties.

6) **Do alerts spam my phone?**  
No—quiet hours (22:00–07:00) and backoff logic apply by default.

7) **How do you compare to typical “airdrop hunters” apps?**  
We prioritize verified roles, reproducible decisions, and recourse. Rewards are for healthy participation, not spam.

8) **What’s the timeline for governance and fee sharing?**  
Pilots are underway; we’ll publish signed summaries and enactment receipts as modules graduate to GA.

9) **Which chains and assets are supported in escrow?**  
Ethereum first (ETH/USDC/USDT). Others considered after we validate safety and throughput.

10) **Is there a public status page?**  
Yes—major incidents will be posted promptly with SLO burn alerts and next steps.

## Appendix — Business Rules Map
- **0) Global Contract & Error Envelope** → *Our Solution*, *How It Works (Wallets & Transactions)*, *FAQ #4*  
- **1) Wallet & Stars ↔ FZ** → *How It Works (Wallets & Transactions)*, *Rewards & Loyalty*  
- **2) Referrals (Three‑Tier)** → *Rewards & Loyalty*, *FAQ #1*  
- **3) Verification (Role‑based)** → *Verification & Safety*, *Call to Action*  
- **4) Discovery (Privacy‑first)** → *Events & Community Mechanics*, *Privacy*  
- **5) Connections** → *Events & Community Mechanics*  
- **6) Subscriptions & Entitlements** → *Why It’s Different* (moat signals)  
- **7) Listings & Fundraising Intelligence** → *Refunds & Recourse*, *Traction & Proof*  
- **8) Events Registrations** → *Events & Community Mechanics*  
- **9) Investor Gating** → *Verification & Safety*, *Call to Action (Investors)*  
- **10) Portfolio ROI** → *Traction & Proof* (progress), *Roadmap*  
- **11) Watchlists & Alerts** → *Events & Community Mechanics*, *FAQ #6*  
- **12) Rewards & Streaks** → *Rewards & Loyalty*, *TL;DR*  
- **13) BTC Pulse (Analytics)** → *Roadmap*  
- **14) Governance (DAO‑lite)** → *Governance & Community*, *Roadmap*, *FAQ #8*  
- **15) Economy & Fee Sharing** → *Why It’s Different*, *Roadmap*  
- **16) AI Copilot (Explainable)** → *Why It’s Different* (operational moat)  
- **17) FOMO Cache** → *Why It’s Different* (network effects)  
- **18) Privacy & Security** → *Privacy*, *FAQ #3*, *TL;DR*  
- **19) Stars‑Settled Digital Asset Escrow — Ethereum** → *Wallets & Transactions*, *Refunds & Recourse*, *FAQ #5*, *Roadmap*  
- **20) Operations & Observability** → *Traction & Proof*, *FAQ #10*

