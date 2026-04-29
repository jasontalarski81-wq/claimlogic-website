# ClaimLogic Cold Email Sequence

**Target:** Roofing company owners (5-25 employees, $1M-$10M revenue, insurance-heavy)
**Goal:** Book a 15-min demo or get free trial signup
**Strategy:** 5-email sequence over 14 days
**From:** Jason Talarski <info@getclaimlogic.com>
**Reply-to:** Personal email so replies feel real

---

## SETUP

**Send via:** Resend (already configured in your CRM)
**Throttle:** 30 emails/day max, 3-6 minute delays
**Track:** Opens (Resend webhooks), replies (Zoho IMAP), trial signups (Stripe)
**Personalize at minimum:** First name, company name, state/city

---

## EMAIL 1 — Day 1 (The Hook)

**Subject:** {{first_name}}, are you eating supplements at {{company}}?

Hey {{first_name}},

Quick question: when State Farm or Allstate "forgets" drip edge on a $20K claim, do you have time to fight them line-by-line?

Most roofing owners I talk to don't. They eat the loss. ~$5K per claim, every claim.

I built ClaimLogic to fix that. AI reads the carrier scope, finds every missed line item, writes the supplement, and emails the adjuster — in 90 seconds.

Want to see it work on a real {{state}} claim? 2-minute video, no signup:
https://getclaimlogic.com/demo

— Jason
Trustman Roofing | ClaimLogic Founder
(636) 541-7005

P.S. We just recovered $19,064 on a single State Farm claim last week. The roofer that closed it took 90 seconds.

---

## EMAIL 2 — Day 4 (Social Proof)

**Subject:** Re: $5K per claim

{{first_name}},

Following up on my last email — I know you're slammed running crews.

Here's the deal in 30 seconds:

**Real case study.** Kyle Smith job. St. Louis, MO.
- Carrier approved: $19,200 (partial roof + siding repair)
- ClaimLogic flagged: $4,200 in missed line items
- LKQ full replacement supplement: $38,264 total
- **Net recovery: +$19,064 in 90 seconds**

The system learns YOUR carriers in YOUR markets. The more claims you process, the smarter it gets at predicting what each carrier denies, omits, and short-pays.

If we don't recover at least $5,000 for you in month one — it's free.

Worth a 15-min demo? https://calendly.com/claimlogic/demo

— Jason

---

## EMAIL 3 — Day 7 (The Problem Stack)

**Subject:** The 5 line items adjusters always skip

{{first_name}},

I won't bore you with another pitch. Here's a free cheat sheet instead — the 5 line items {{state}} carriers omit most often:

1. **Drip edge** — IRC R905.2.8.5 requires it. Carriers skip it 73% of the time. ~$440/claim.
2. **Ice & water shield** — Required in cold zones. Skipped 41%. ~$720/claim.
3. **Starter strip (rakes)** — Manufacturer spec. Skipped 64%. ~$280/claim.
4. **Step flashing** — Required at all wall intersections. Undercounted 58%. ~$320/claim.
5. **Steep charge** — Capped at 7/12 even when pitch is 10/12. Short-paid 51%. ~$400+/claim.

Add it up: that's $2,160 you're potentially missing on EVERY claim.

ClaimLogic catches all 5 automatically and writes the supplement letter for you. 90 seconds.

Free trial (no card): https://getclaimlogic.com/signup

— Jason

---

## EMAIL 4 — Day 11 (Pattern Interrupt / Direct)

**Subject:** Should I take you off the list?

Hey {{first_name}},

I've reached out a few times about ClaimLogic. No reply yet, which is fine — you're busy.

Just want to be clear:

If you're already crushing supplements with AccuLynx, JobNimbus, or in-house — awesome, ignore me.

If you're losing $5K+ per claim and don't have time to fight every line item — let's talk for 15 minutes.

Reply with one word and I'll act accordingly:
- **"YES"** — book the demo
- **"NO"** — I'll take you off the list
- **"MAYBE"** — I'll send you the case study PDF and back off

— Jason

---

## EMAIL 5 — Day 14 (Final)

**Subject:** Last one from me

{{first_name}},

Last email from me, promise.

The math on ClaimLogic:
- $499/mo Growth plan
- Avg recovery: $5,200/claim × 4 claims/week = $20,800/week
- Net ROI: 41x in month one

If even one of those numbers makes you raise an eyebrow, give me 15 minutes:
https://calendly.com/claimlogic/demo

If not, I'll stop emailing. No hard feelings.

Either way — best of luck on the {{state}} season.

— Jason
Trustman Roofing | ClaimLogic Founder
(636) 541-7005
info@getclaimlogic.com

---

## REPLY HANDLERS

### "Tell me more"
Send: case study PDF + Calendly link + offer to call within 24h

### "How is this different from AccuLynx?"
> AccuLynx is a CRM. ClaimLogic is a supplement engine. We integrate alongside AccuLynx — your team uses both. AccuLynx tracks the job; ClaimLogic recovers the money.

### "We do supplements in-house"
> That's great. How long does it take to write one? Average is 2 hours per claim. ClaimLogic does it in 90 seconds. What would your team do with the time back?

### "Send me pricing"
Send: pricing PDF + 14-day trial link + $5K guarantee mention

### "Not interested"
> No problem — best of luck. If you ever change your mind, the door's open. I'll take you off the list.

---

## METRICS TO TRACK

- **Open rate target:** 35%+ (subject lines tested)
- **Reply rate target:** 5-8%
- **Demo booking rate:** 1-2% of total sent
- **Trial-to-paid conversion:** 25-35%
- **Avg sales cycle:** 7-14 days from first email

## A/B TESTS TO RUN

1. **Email 1 subject:** "are you eating supplements" vs "$5K per claim missing"
2. **Email 2:** Case study format vs bullet stat format
3. **CTA:** Calendly vs free trial vs reply with "YES"
4. **Length:** 50-word vs 150-word vs 300-word

## WHEN TO SEND

- **Best days:** Tuesday, Wednesday, Thursday
- **Best times:** 7:00-9:00 AM CST or 2:00-4:00 PM CST
- **Avoid:** Mondays (inbox overflow), Friday afternoons, holidays

## TARGET LIST SOURCES

You already have: 240 OK businesses, 98 with emails (from earlier scrape)

Add:
- Google Maps scrape: "roofing company [city]" in TX, OK, MO, KS, CO, FL
- LinkedIn Sales Navigator: roofing owners 5-50 employees
- Roofing Insights podcast guest list
- IRE / RoofCon attendee lists
- Storm chaser FB groups (extract members, look up companies)
