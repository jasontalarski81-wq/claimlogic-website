# ClaimLogic Call Center Playbook
**Goal:** 10 reps live by Tuesday next week, generating qualified demos and closes.
**Comp:** 20% recurring on every deal they close, paid monthly as long as the customer pays.

---

## THE MATH (show this to recruits)

| Plan | MRR | Rep Commission | Annual to Rep (1 close) |
|---|---|---|---|
| Starter $199 | $39.80/mo | $477.60/yr per close |
| Growth $499 | $99.80/mo | $1,197.60/yr per close |
| Pro $899 | $179.80/mo | $2,157.60/yr per close |

**Avg rep targets:** 4 closes/month at Growth tier = $399/mo recurring after month 1
- Month 1: $399
- Month 6: $2,394/mo if all retain
- Month 12: $4,788/mo if pipeline keeps filling

**Top performer (8 closes/mo Growth):** $957/mo new × 12 months = $11,484/mo by month 12

That's why this comp model attracts hungry closers.

---

## WEEK 1 — SETUP (Mon-Fri before launch)

### Monday — Tools & Stack ($200-500 setup)
1. **Phone system:** [Aircall](https://aircall.io) ($30/seat/mo) or [Dialpad](https://dialpad.com) ($25/seat) — power dialer, call recording, CRM integration
   - Alt cheap option: [CloseRinger](https://close.com) bundles dialer + CRM
2. **CRM for reps:** Use ClaimLogic's own backend (you have Stripe + recurring tracking) OR [Close.com](https://close.com) ($99/seat) for sales-specific
3. **Lead source:** ClaimLogic outreach scraper (free, you already built it) — scrape 1,000 roofers across 20 cities by Friday
4. **Slack/Discord** workspace for reps + daily huddle channel
5. **Loom** account ($10/mo) — record demos to send prospects who can't take a live call

### Tuesday — Hire 10 Reps
- **Where to post:** Indeed, Craigslist, FB groups ("Sales Jobs Remote"), LinkedIn
- **Job title:** "B2B SaaS Sales Rep — 100% Recurring Commission — Roofing Vertical"
- **Pitch in posting:**
  > "Sell AI software to roofing companies. $499/mo product. You earn 20% recurring on every close, paid monthly forever as long as customer pays. Top reps making $4K-$10K/mo by month 6. Remote OK. Must have B2B phone sales experience."
- **Filter for:** prior roofing sales, prior SaaS sales, or prior call-center performance
- **Interview format:** 15-min Zoom — make them roleplay a cold call. If they can't pivot when you object, pass.

### Wednesday — Compensation & Contract
- **1099 contractors** (not employees) — keeps you flexible
- **Comp structure:**
  - 20% MRR for life of customer (vests immediately)
  - $100 spiff for first close in week 1
  - $500 bonus when they hit 5 lifetime closes
  - **No base, no draw** — pure commission keeps cost variable, attracts true closers
- **Contract:** Have a basic 1099 commission agreement signed before training (Stripe Atlas template or LegalZoom $149)
- **Stripe Connect** — set up Express accounts so commissions auto-route monthly

### Thursday — Training Materials
1. **Product walkthrough video** (45 min) — record yourself demoing ClaimLogic on Kyle Smith's job
2. **5-page sales script** (provided below — see SCRIPT section)
3. **Objection handling doc** (provided below)
4. **Discovery questions cheat sheet**
5. **Top 10 FAQs**

### Friday — Lead List Ready
Run scraper across 20 cities (10K+ prospects):
```bash
cd ~/.openclaw/workspace/claimlogic_outreach
for city in "Dallas, TX" "Houston, TX" "Austin, TX" "Atlanta, GA" "Charlotte, NC" \
            "Nashville, TN" "Memphis, TN" "Birmingham, AL" "Jacksonville, FL" \
            "Tampa, FL" "Orlando, FL" "Kansas City, MO" "Springfield, MO" \
            "Wichita, KS" "Denver, CO" "Colorado Springs, CO" "Phoenix, AZ" \
            "Tulsa, OK" "Oklahoma City, OK" "Little Rock, AR"; do
  /usr/bin/python3 scrape_roofers.py "$city"
done
```
Should yield 800-1,200 prospects. Split evenly: 80-120 per rep.

---

## WEEK 2 — LAUNCH (Mon-Fri)

### Monday — Onboarding Day (4 hours)
- 9-10 AM: Watch product demo video (homework)
- 10-11 AM: Live Q&A with you
- 11-12: Roleplay calls (rep vs manager)
- 1-3 PM: Set up phones, dialer, Loom, ClaimLogic admin access
- 3-5 PM: First 25 dials each (~50% pickup, ~5 conversations per rep)

### Tuesday onward — Daily Rhythm
- **8:30 AM:** 15-min huddle (yesterday's wins, today's goals, blockers)
- **9-12:** Power hour 1 (40 dials minimum)
- **12-1:** Lunch + lead research
- **1-4:** Power hour 2 (40 dials)
- **4-5:** Demo follow-ups, email replies, CRM hygiene
- **5 PM:** End-of-day Slack stats post (dials, conversations, demos booked, closes)

### KPIs (track per rep)
- **Dials/day:** 80 minimum (industry standard for inside sales)
- **Conversations/day:** 8-12 (10% pickup × decision-maker filter)
- **Demos booked/day:** 1-2
- **Demos held/week:** 5-7
- **Closes/week:** 1-2
- **Show rate:** 60%+ (use SMS reminders 1hr before)
- **Close rate:** 20-30% of demos held

---

## THE SALES SCRIPT (give this to every rep)

### OPENING (30 seconds — earn the next 30)
> "Hey, this is [Name] with ClaimLogic — quick question for the owner: when State Farm short-pays a claim by five grand, who at [Company] handles writing the supplement?"

**If receptionist:** "Got it — can you connect me to whoever handles insurance claims and supplements? I'll be 90 seconds with them."

**If owner picks up:** "Cool, this'll be quick — do you guys take insurance work? Wind/hail, storm restoration?"
- **YES** → continue script
- **NO** → "Got it — appreciate your time. Have a great day." [hang up, mark as DQ]

### HOOK (the $5K story — 30 seconds)
> "Cool. Reason I'm calling — most roofers I talk to are leaving five to eight thousand on every claim because adjusters omit drip edge, short-pay steep charge, deny code upgrades. Sound familiar?"

**Wait for them to say "yeah"**

> "Right. So we built ClaimLogic — it reads the carrier scope, finds every missed line item, writes the supplement letter, and emails the adjuster in 90 seconds. Last week one of our customers recovered $19,064 on a single State Farm claim using it."

### PIVOT TO DEMO (don't pitch — show)
> "It's way faster to show you than tell you. I can hop on a Zoom for 15 minutes Thursday or Friday and run it on one of your actual claims — you tell me which one was lowballed and we'll see what ClaimLogic finds. Worst case, you walk away with insight on a real claim. Thursday 2 PM or Friday 10 AM work?"

### IF THEY ASK PRICE BEFORE DEMO
> "Three plans — $199, $499, or $899 a month depending on team size. Most roofers go with the $499 plan because it includes the LKQ engine and carrier learning. We have a $5K guarantee — if you don't recover at least five grand month one, it's free. But honestly, the price is irrelevant once you see what it does. Thursday 2 or Friday 10?"

---

## OBJECTION HANDLERS

**"We already use AccuLynx/JobNimbus"**
> Perfect — ClaimLogic doesn't replace your CRM, it sits next to it. AccuLynx tracks the job. ClaimLogic recovers the money the carrier owes you. Most of our customers run both.

**"We do supplements in-house"**
> Awesome — how long does each one take? Most teams say 90 minutes to 2 hours. ClaimLogic does it in 90 seconds. What would your team do with that time back? Demo'll show you the difference — Thursday 2 or Friday 10?

**"Send me info"**
> Happy to. But honestly, info docs don't show you what ClaimLogic does — the demo does. It's 15 minutes and we run it on one of YOUR claims live. Thursday or Friday?

**"How much?"** (before they've seen value)
> $499/month for the most popular plan. Pays for itself the first claim it touches. We have a $5K month-one guarantee. Demo's the way to know if it works for you.

**"Not interested" / "We're good"**
> Totally fair. Quick question before I let you go — what does your team currently do when an adjuster lowballs you on drip edge or steep charge? Just eat it, or fight it?
- **Eat it** → "That's the gap we close. 60-second demo, no commitment — Thursday or Friday?"
- **Fight it** → "Cool — what's your average win rate when you fight? Most folks are at 40-50%. ClaimLogic users hit 80-90%. Thursday or Friday?"

**"Call me back"**
> Sure — what day specifically works? [pin them to a time, send calendar invite immediately]

**"I need to talk to my partner"**
> Smart. Bring them on the demo — Thursday at 2, both of you. I'll send the Zoom link.

---

## THE DEMO STRUCTURE (15 minutes — manager runs these, not reps)

You (Jason) run the demos personally for the first 30 days, while reps book them. Then promote your best rep to lead-demo specialist.

1. **0-2 min: Discovery**
   - "Walk me through your last 3 claims and what frustrated you about them"
   - "How many claims/month?" "Avg ticket size?" "How many people touch a supplement?"

2. **2-12 min: Live demo on THEIR claim**
   - Have them upload their carrier scope live (or screenshare their CRM)
   - Run Claim Intelligence → score appears, missed revenue calculated
   - Click LKQ Full Roof + Siding → fill in their actual numbers
   - Generate supplement PDF → show the dollar amount
   - Send to Adjuster button → "imagine this every claim"

3. **12-14 min: The close**
   - "Based on what you just saw, what plan makes sense — Starter, Growth, or Pro?"
   - "Want to start the 14-day free trial right now? I can have you logged in by the time we hang up."

4. **14-15 min: Trial setup**
   - Send signup link in chat
   - Walk them through first claim upload
   - Schedule 7-day check-in

---

## REP TIERS & PROMOTIONS

After 30 days, rank reps by closes:

| Tier | Closes/mo | Reward |
|---|---|---|
| **Bronze** | 0-2 | Continue training, more dials |
| **Silver** | 3-5 | Standard 20% comm |
| **Gold** | 6-9 | Bump to 25% comm + their pick of leads |
| **Platinum** | 10+ | 30% comm + bonus pool eligibility |

After 60 days, fire bottom 30% (no shame, just math). Keep refilling.

---

## TECH STACK COSTS (10 reps)

| Tool | Cost/mo |
|---|---|
| Aircall (10 seats) | $300 |
| Slack workspace | $0 (free tier OK) |
| Loom team | $80 |
| Domain emails (10 × @claimlogic.com via Zoho) | $30 |
| Lead scraping (Google Places API) | $0-50 (free credits) |
| Zoom (for demos) | $15 |
| **TOTAL** | **~$425/mo** |

**Break-even:** 1 close on Growth plan ($499/mo gross, $399 net of rep comm) covers your stack month one.

---

## CALL CENTER LOCATION

You said you want to start a call center. Two paths:

**A) Remote-only (recommended start)**
- Zero overhead
- Hire from anywhere (more talent pool)
- Zoom huddles 2x/day
- Aircall handles routing
- Pros: faster launch, lower risk
- Cons: less culture, harder to manage rookies

**B) Physical call center (St. Louis)**
- Office space in St. Louis: ~$1,500-2,500/mo for 10-desk space
- Better culture, faster training
- Cons: setup time, lease commitment
- **Wait until you have 5 proven Gold-tier reps before opening physical office**

**Recommended:** Start remote, prove the model month 1-2, open physical office month 3 once you have 3-5 Gold reps to seed the culture.

---

## WHAT YOU NEED FROM ME (Lexi)

Tell me when you're ready and I'll:
1. **Build the rep CRM dashboard** inside ClaimLogic — track each rep's pipeline, deals closed, MRR generated, commission owed
2. **Auto-commission tracking** — every Stripe payment → calculate 20% → log to rep's account → pay out via Stripe Connect monthly
3. **Lead distribution system** — auto-assign scraped leads to reps round-robin, prevent duplicate calls
4. **Onboarding email/SMS sequence** for new reps
5. **Recruiting funnel** — landing page at jobs.claimlogic.com to capture rep applications

---

## TIMELINE TO LAUNCH

| Day | Action |
|---|---|
| **Thu (today)** | Post job listings, build training video |
| **Fri** | Interview 30-50 candidates (15 min each) |
| **Sat-Sun** | Sign 10 contracts, set up tools |
| **Mon** | Onboarding day, first dials |
| **Tue-Fri** | Reps dialing 80/day, you running demos |
| **Following Mon** | First close projected (best rep) |
| **Day 30** | Target: 15-25 closes total = ~$1.5K-$2.5K MRR new |
| **Day 60** | Rank reps, promote/cut, expand |

---

## YOUR ASKS FROM ME (today)

Pick what you want me to build first:

1. **Recruiting landing page** at jobs.claimlogic.com with apply form
2. **Rep CRM dashboard** inside ClaimLogic (pipeline + commission tracking)
3. **Job posting copy** ready to paste into Indeed/Craigslist/LinkedIn
4. **30-50 question candidate screening doc** for interviews
5. **5-day onboarding curriculum** with daily videos + quizzes
6. **Lead distribution + dialer integration** with Aircall API

Say which order you want them and I'll start tonight.
