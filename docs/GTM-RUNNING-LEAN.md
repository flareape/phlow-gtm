# Phlow GTM Strategy — Running Lean Framework
### Product-Led Growth · Community-First · Zero Paid Ads
**Status:** MVP live · User research done · Signal project for Flare  
**Reference:** *Running Lean* — Ash Maurya · *Continuous Innovation Framework*  
**Last updated:** April 2026

---

## The Actual Purpose of Phlow

> Phlow is not the final product. **Phlow is the proof layer for Flare.**

Flare is the larger vision. Phlow exists to answer one question before building it:

> *Does cycle-aware work planning content actually resonate with real women — enough that they come back on their own, without being asked?*

### What This Changes About How We Operate

| If Phlow were the product... | Because Phlow is a signal project... |
|---|---|
| Optimize for conversion | Optimize for **signal quality** |
| Build onboarding funnel | Keep zero onboarding — friction masks the signal |
| Maximize DAU | Measure **voluntary return rate** — the only honest signal |
| Push notifications + email capture | Only passive measurement — no artificial retention |
| Scale channels fast | Go narrow and deep — understand *why* people return |
| Assess PMF by revenue | Assess PMF by **referral behavior** and **unprompted return** |

**The zero-onboarding constraint is intentional signal design.** If someone returns to Phlow with no email nudge, no push notification, no login — that return is real. It means the content earned it. That is exactly the behavior Flare needs to see proven.

### The Phlow → Flare Signal Handoff

```
Phlow proves:                          Flare builds on:
──────────────────────────────────     ──────────────────────────────────
✓ Content format resonates             Deeper content, richer phases
✓ Audience segment is real             Expanded user segments
✓ Voluntary return exists              Full habit-layer product
✓ Referral behavior is natural         Community-native social features
✓ Science framing is trusted           Premium science-backed intelligence
✓ Community forms around the topic     Community is the product
```

When Phlow shows unprompted Day-14 return rates above 40% and community members referring peers without being asked — **that is the green light for Flare.**

---

## Where We Are in the Running Lean Journey

Ash Maurya defines three stages. Be honest about where you actually are.

```
Stage 1: Problem/Solution Fit     ← WE WERE HERE
"Do I have a problem worth solving?"
        ↓
Stage 2: Product/Market Fit       ← WE ARE NOW ENTERING THIS
"Have I built something people want?"
        ↓
Stage 3: Scale
"How do I accelerate growth?"
```

**Assessment:**
- ✅ Problem confirmed via research: no tool maps cycle → work planning
- ✅ Solution hypothesis tested: MVP shipped, phase card UX validated
- ✅ Zero-onboarding constraint confirmed: open the app → see today's phase → done
- 🔄 Not yet proven: do users voluntarily return across a full 28-day cycle with no prompting?
- 🔄 Not yet proven: does the community form naturally around the content?
- 🔄 Not yet proven: do users refer others unprompted?

The riskiest assumption at this stage is **voluntary return** — not acquisition, not revenue. Revenue is a Flare question. Phlow's job is to prove the behavior exists.

---

## The Lean Canvas Snapshot (April 2026)

| Block | Status | Current Answer |
|---|---|---|
| **Problem** | ✅ Validated | Women treat all days as equal; hormonal phases create 4 distinct productive modes |
| **Customer Segment** | ✅ Validated | Women 25–45, knowledge workers, cycle-aware but lacking work-planning layer |
| **Unique Value Prop** | ✅ Defined | "Know in 5 seconds what to work on today, tuned to your cycle." |
| **Solution** | ✅ Built | Daily card: phase name + energy profile + 3 task types + 1 avoid + tip |
| **Channels** | 🔄 Testing | Direct DMs → community → organic social → content |
| **Revenue Streams** | 🔜 Phase 2 | €4.90/mo premium unlock; free tier is PLG acquisition engine |
| **Cost Structure** | ✅ Low | Domain ~€12/yr; Vercel free tier; no backend in Phase 1 |
| **Key Metrics** | 🔄 Gathering | `onboarding_completed`, `returning_user`, `pwa_installed`, referrer source |
| **Unfair Advantage** | ✅ Real | Peer-reviewed science baked in; offline-first; no account friction |

---

## What User Research Told Us (Synthesis)

> Read this before any campaign, channel, or copy decision. Users teach us our own language.

### Validated Pain Points (from discovery phase)
1. **Scheduling blindness** — Women know their cycle exists but don't apply it to work scheduling. They only realize the mismatch in retrospect ("I shouldn't have pitched that day").
2. **Energy surprise** — Unexpected low-energy days feel like personal failure, not biology.
3. **No actionable layer** — Flo/Clue track symptoms. They don't say "do your deep work now."
4. **Cycle-invisible tools** — Notion, Todoist, Calendly treat day 1 and day 17 identically.

### Language Users Actually Use (steal this)
- "I feel like I'm fighting myself"
- "I used to think I was just bad at consistency"
- "I wish I'd known not to schedule that"
- "My brain literally doesn't work the same every week"
- "I can't believe this is backed by real science"

### What's Still Missing (gaps from research → product backlog)
- [ ] **Retroactive insight**: "Why was last Tuesday so hard?" — cycle history view
- [ ] **Forward planning**: "What should I NOT schedule next week?" — 28-day preview
- [ ] **Chronic condition awareness**: MCAS/POTS users want severity-aware cards
- [ ] **Partner/team sharing**: "I want to send this to my manager/collaborator"
- [ ] **Habit integration**: morning routine trigger; push notification as anchor habit

> These gaps define the Phase 2 product roadmap AND the Phase 2 copywriting.

---

## The Riskiest Assumptions Right Now

Running Lean demands we identify and kill risk systematically. Do not scale until these are answered.

| Rank | Assumption | Type | How to Test | Pass Condition |
|---|---|---|---|---|
| 🔴 1 | Users return across a full 28-day cycle | **Retention** | Cohort: `returning_user` at Day 7, Day 14, Day 28 | >40% Day-28 retention |
| 🔴 2 | Users change actual work behavior based on the card | **Value** | Interview 10 users after their first full cycle | >6/10 report a scheduling change |
| 🟠 3 | Users will pay €4.90/month for the 28-day preview | **Willingness to pay** | Mafia offer pilot: 8 pre-commitments before building payment | 8 of 15 qualified prospects say yes |
| 🟠 4 | The mid-luteal phase card is the "aha" moment | **Activation** | Session recording + event: `phase_card_viewed`, phase = luteal_mid | High re-open rate on luteal_mid days |
| 🟡 5 | Referral is primary acquisition channel | **Channel** | Track `referrer_source`; interview how users found us | >30% of sign-ups via direct referral |
| 🟡 6 | Women founder community is reachable without paid | **Channel** | 20 personal DMs → measure response + install rate | >5 installs from first 20 DMs |

---

## PLG Growth Engine (Product-Led Growth)

> This is not a feature decision. It is a go-to-market strategy. The product IS the acquisition channel.

### How PLG Works for Phlow

```
ACQUISITION             ACTIVATION              RETENTION              REFERRAL
     │                       │                      │                     │
User hears about Phlow  →  Opens app, enters    →  Returns on cycle  →  Screenshots aha
via DM, post, or share     cycle day, sees         day 14, 17, 20...     moment → shares
                           today's card                                   it naturally
                           "Oh wow — this is
                           literally today"
                                │
                           INSTANT FIRST VALUE
                           (no account, no onboarding wall)
```

### PLG Mechanics to Protect

1. **Zero friction to first value**: one question (cycle start date), instant output. No login. No email capture. No paywall.
2. **Value before ask**: the free card must be genuinely useful every day, forever. The premium unlock extends the view, not the value.
3. **The shareable moment**: when a card lands perfectly ("this is exactly how I feel"), users screenshot and share. Design for that. Make phase names, tips, and cards copy-friendly.
4. **PWA as habit anchor**: home screen install = daily opt-in without push. This is Phlow's version of a notification. Make the install flow compelling.
5. **Virality by biology**: cycle phases are universal. "You have to see what it says on day 17" is a natural invite. Build a share/send card feature early.

### The Free → Paid Upgrade Trigger

The upgrade is not a paywall. It's a desire moment:
> User opens Phlow on follicular day 9. The card is great. She thinks: *"What does day 17 look like? I have a board meeting then."* → The 28-day preview unlocks that answer.

**Freemium is only working if:** at least 10% of active users are trying to click "forward" into the calendar. That's the signal to activate Phase 2 premium.

---

## Community Strategy — The Growth Moat

> Community is not a marketing channel. It is the compounding asset. Product alone churns. Product + community retains.

### Why Community First for Phlow

1. Cycle awareness is **personal and social** — women talk about this with each other
2. No existing community combines *work planning* with *cycle tracking* — there is a gap to own
3. Community generates the **social proof** that paid ads cannot buy
4. Founding users become **product co-creators** — their language shapes the copy that converts

### The Founding Community (First 100 Women)

**Platform:** Telegram (low friction, no algorithm, direct)  
**Goal:** 100 women who get genuine value and are willing to say so publicly  
**Offer:** Lifetime free premium for the first 100 women who post a real aha moment in `#aha-moments`

**Channel structure:**
| Channel | Purpose |
|---|---|
| `#aha-moments` | Screenshots, realizations, "I finally understand why..." — this is the proof engine |
| `#phase-of-the-day` | Daily check-in: what day are you on? What's landing? Builds habit + social proof |
| `#forward-planning` | What are you protecting in your next luteal peak? — 28-day use case preview |
| `#science-questions` | Denis and team answer with real research citations — builds trust and authority |
| `#product-feedback` | Direct input loop → shapes the roadmap |

**Community rituals:**
- Weekly "phase check-in" post from Denis (founder visibility)
- Monthly "cycle wrap" — what worked? What shifted? (retrospective social proof)
- Bi-weekly research share from `RESEARCH.md` — keeps the community intellectually honest

### Community Growth Path

```
Month 1: Seed 20 women via personal DMs (no pitch — just "what do you think?")
Month 2: Founding community goes live (50 invited, 30+ active)
Month 3: First aha moments captured → turned into first content
Month 4: Community-to-community: members invite their peers ("you have to see this")
Month 6: Founding community is the proof engine for press outreach
Month 12: Community has momentum of its own — less Denis-dependent
```

---

## Go-To-Market Traction Roadmap

### Now (Months 1–3): Confirm Retention, Build the Proof Engine

**Objective:** Validate that women return across at least one full cycle and report behavioral change.

| Action | Output | Owner | Timeline |
|---|---|---|---|
| 15 problem discovery interviews → 10 follow-up "cycle wrap" interviews | Validated aha moments; confirmed behavioral change | Denis | Month 1–2 |
| Personal DMs to 20 women founders/operators | First 20 installs with direct feedback loop | Denis | Week 1 |
| Founding Telegram community live | First 30 active members | Denis | Month 1 |
| Capture first 3 aha moment screenshots | Content proof; social proof | Community | Month 2 |
| Implement Day-7/14/28 cohort tracking | Retention data | Dev | Month 1 |
| First 3 Instagram posts: "What my cycle taught me about work" | Channel testing; 0-to-1 social presence | Denis | Month 2 |
| Mafia offer pilot: pre-commit to pay before Phase 2 is built | 8 paying commitments | Denis | Month 3 |

**Success looks like:** >40% Day-28 retention, >6/10 interview users report a scheduling change, 8 pre-commit paying users.

---

### Next (Months 3–12): Product/Market Fit

**Objective:** Build the growth loop — users activate, retain, and refer without Denis pushing every cycle.

| Action | Output | Owner | Timeline |
|---|---|---|---|
| Phase 2 build: auth + 28-day preview + payment (€4.90/mo) | Paying tier live | Dev | Month 3–4 |
| Share/send card feature | Viral coefficient increase | Dev | Month 4 |
| Referral program: "Invite 3 cycle-aware women, unlock 1 free month" | Referral loop | Dev | Month 5 |
| TikTok content: "I used Phlow for one full cycle — here's what happened" | First video with real cycle story | Denis/user | Month 4 |
| LinkedIn founder article: "I stopped scheduling pitches on day 26" | Founder/operator audience reach | Denis | Month 4 |
| MCAS/POTS Reddit + Facebook outreach | Underserved niche activation | Denis | Month 5 |
| 3 journalist pitches (not press releases — personal emails with the science) | First editorial coverage | Denis | Month 6 |
| Women founder Slack/Discord communities (Chief, FFC-adjacent) | Community channel activation | Denis | Month 5–6 |
| NPS survey at Day-28 | NPS baseline; qualitative referral signals | Analytics | Month 4+ |

**Success looks like:** NPS >50, Day-28 retention >40%, first 20 paying users, first organic press mention.

---

### Later (Months 12–36): Scale

**Objective:** Turn what's working into a repeatable acquisition and retention engine.

| Action | Condition to start |
|---|---|
| SEO content strategy (cycle × work keyword clusters) | After organic social proves the language that converts |
| Podcast pitches (women founder / biohacking / women's health shows) | After first press mention establishes credibility |
| Partnership with productivity communities (e.g., Ness Labs, Ali Abdaal adjacents) | After NPS >50 and clear referral signal |
| B2B / team plans (wellness, HR, women founder orgs) | After 200 paying individual users |
| Native app (iOS + Android) | After Day-28 retention >40% consistently |
| Paid acquisition | Only as a multiplier on a proven organic funnel |

---

## The Experiment Queue (Running Lean style)

> Every campaign, post, and outreach is an experiment. Define success before you run it.

### Active Experiments

| # | Hypothesis | Action | Metric | Pass Condition | Status |
|---|---|---|---|---|---|
| E1 | Women in personal network will install via DM | 20 personal DMs (see `DM-PLAYBOOK.md`) | Install rate from DM | >25% (5/20 installs) | 🔄 Running |
| E2 | Mid-luteal card is the highest-value card | Track re-open rate by phase | `phase_card_viewed` breakdown | Luteal mid = highest re-open | 🔄 Running |
| E3 | "Day 26 pitch" hook generates social engagement | 1 TikTok + 1 Instagram post | Saves + shares (not likes) | >50 saves | 🔜 Queued |
| E4 | MCAS/POTS community has high activation | Post in 2 Reddit communities | Click + install vs. other channels | Top-2 referrer source | 🔜 Queued |
| E5 | Mafia offer generates pre-payment commitment | Offer to 15 qualified users | Pay-before-built commitments | 8/15 say yes | 🔜 Queued |
| E6 | Founding community post generates aha moments | Open Telegram, post prompt | Posts in `#aha-moments` within 7 days | >5 aha posts | 🔜 Queued |

### Fail Paths — What to do when an experiment doesn't pass

> Running Lean demands you precommit to the fail path *before* running the experiment. Read these before you launch each test.

**E1 fails (< 5 of 20 DMs convert to install):**
The message format is wrong, the relationship wasn't warm enough, or the product doesn't survive first contact. Do NOT send more DMs. Instead: interview 5 of the 15 non-installers. Ask exactly one question: "What made you not try it?" The answer is either (a) the framing — fix the DM type, (b) the product premise — the problem doesn't resonate without more context, or (c) the relationship — the wrong 20 people were chosen. Identify which, fix that one thing, run again with the next 20.

**E2 fails (mid-luteal is NOT the highest re-open phase):**
The science framing around mid-luteal isn't the primary value driver. Don't force it. Look at which phase IS highest — follicular ("new start energy") and menstrual ("explains why I crashed") are both plausible breakout candidates. Adjust the content hierarchy and the social hook: lead with the phase that's actually resonating. Update `RESEARCH.md` with this finding before any content decisions.

**E3 fails (< 50 saves on first social post):**
The creative hook isn't landing in that format. Do not keep posting the same thing. Run an immediate post-mortem: was it the hook (first 3 seconds), the format (face vs. text vs. phone demo), or the platform (TikTok vs. Instagram)? Make one change only, re-run on the same platform. If it fails again with a different hook and format, try the other platform before concluding social doesn't work. Minimum 3 varied attempts before abandoning a channel.

**E4 fails (MCAS/POTS community doesn't activate):**
Either the language was too generic for a community where people discuss medical-grade symptom severity, or the framing felt promotional before trust was built. Do not post a product link again in the same community. Spend 2 weeks contributing genuinely — answering questions, sharing the research paper, acknowledging complexity — before posting again. If the second attempt fails, the channel timing is wrong (not the audience), revisit at month 6 with case studies from actual MCAS/POTS users.

**E5 fails (< 8 of 15 pre-payment commitments):**
**Stop. Do not build the payment flow.** Interview every person who said no. The blocker will be one of three things: (a) price — test €2.90/month, (b) feature — the 28-day preview isn't compelling enough, try offering cycle history instead, or (c) trust — they like it but won't pay without seeing it first. If (c), build a 7-day free premium trial before the hard paywall. Re-test with 15 fresh qualified users before any payment infrastructure is built.

**E6 fails (< 5 aha posts in 7 days from founding community):**
The community prompt isn't creating the conditions for aha moments to be shared publicly. Try a different trigger: instead of a general prompt, ask a specific question ("What day of your cycle were you on when Phlow first made sense?") that requires a personal answer, not a performance. Also check: is the founding premium offer (lifetime access for aha moment) clearly visible? If members don't know the offer exists, the incentive isn't working. If the problem persists past 14 days, the community format (Telegram) may not be the right platform — consider a private Instagram group as an alternative.

### Experiment Log Template (use for every new test)

```
Experiment: [Name]
Hypothesis: If [action], then [outcome], because [belief]
Action: [Exactly what will be done]
Duration: [Time bound]
Metric: [Single measurable signal]
Pass condition: [Specific threshold]
Fail path: [What to do if it fails — precommitted]
Result: [Fill after]
Learning: [One sentence]
```

### Experiment Log Template (use for every new test)

```
Experiment: [Name]
Hypothesis: If [action], then [outcome], because [belief]
Action: [Exactly what will be done]
Duration: [Time bound]
Metric: [Single measurable signal]
Pass condition: [Specific threshold]
Result: [Fill after]
Learning: [One sentence]
```

---

## Measuring a Zero-Onboarding Product

> This is the hardest measurement problem in PLG: **no account = no user identity = no email funnel.**  
> That constraint is the point. We can only see honest signal.

### What We Can Measure Without an Account

With localStorage + Vercel Analytics + 4 custom events, we can capture everything that matters:

| Signal | How | What It Proves |
|---|---|---|
| **First visit → phase card viewed** | `phase_card_viewed` event on load | Content reached someone |
| **PWA installed** | `pwa_installed` event | Strong intent — they want it on their homescreen |
| **Return visit within 7 days** | localStorage `first_visit` timestamp delta + `return_visit` event | Content pulled them back without any nudge |
| **Return visit at Day 14** | Same localStorage delta | Mid-cycle voluntary return — the core Flare signal |
| **Phase at each return** | `phase_card_viewed` + `cycle_day` param | Which content drives return? |
| **Referrer source** | `referrer_source` event + `document.referrer` | How did they find it? Was it a share? |
| **Swipe / forward navigation** | `day_swiped` event | Are they exploring future phases? (28-day preview desire) |
| **Share interaction** | `card_shared` event | Viral coefficient proxy |
| **Session frequency** | localStorage visit count | Habit formation signal |

### The Signal Stack — Ranked by What Matters for Flare

```
TIER 1 — Flare green-light signals (prove content pull)
├── Day-14 unprompted return rate         > 35% = green
├── PWA install rate                      > 25% = green
└── Referrer = direct/share (not search)  > 30% = green

TIER 2 — Content quality signals (prove format works)
├── Phase card viewed per session         avg > 1.5 = exploring, not bouncing
├── Mid-luteal phase re-open rate         highest of 5 phases = science ≠ science is landing
└── Day-swiped (forward)                  > 20% of users = 28-day desire exists

TIER 3 — Community readiness signals (prove social layer is viable)
├── Telegram join rate from app           any organic joins = community pull
├── Direct referrer share rate            > 15% = women sending it to friends
└── User quotes / aha moments collected   5+ in month 1 = social proof exists
```

### What NOT to Measure (it creates false signal)

| Metric | Why to ignore it for Phlow |
|---|---|
| Total page views | Inflated by single visits; tells us nothing about pull |
| Time on page | Meaningless for a card that delivers value in 10 seconds |
| Social follower count | Vanity; follows ≠ installs ≠ returns |
| Press mentions | Flare metric, not Phlow signal |
| Revenue | Phlow is free; revenue is a Flare validation, not Phlow's job |

### The Single Dashboard to Build

Track only these 5 numbers, weekly:

```
Week [N] Signal Report
─────────────────────────────────────────────────
New first-time visitors:        ____
PWA installs:                   ____   (__ %)
Day-7 voluntary returns:        ____   (__ %)
Day-14 voluntary returns:       ____   (__ %)
Referral / direct share visits: ____   (__ %)
─────────────────────────────────────────────────
Top referrer source:            ____
Most-viewed phase:              ____
Community joins this week:      ____
─────────────────────────────────────────────────
Green light conditions met:     Y / N
```

Run this every Monday. First 8 weeks of data is the Flare investment case.

---

## Key Metrics — The Pirate Metrics for Phlow

> AARRR adapted for a zero-onboarding, PLG signal project.

| Stage | Metric | Measurement | Signal threshold | Flare green light |
|---|---|---|---|---|
| **Acquisition** | New visitors / week | Vercel Analytics | 10/week by month 2 | 50+/week |
| **Acquisition** | Primary referrer source | `referrer_source` event | Know top 2 channels | Direct/share = #1 |
| **Activation** | `pwa_installed` rate | Custom event | >25% of visitors | >40% |
| **Activation** | Phase card fully viewed | `phase_card_viewed` event | >80% of visits | — |
| **Retention** | Day-7 unprompted return | localStorage delta | >40% | >50% |
| **Retention** | Day-14 unprompted return | localStorage delta | >35% | >40% |
| **Referral** | % visits from direct share | `referrer_source` | >20% | >30% |
| **Referral** | Community (Telegram) joins | Manual count | 30 in month 2 | 100 founding members |
| **Content** | Most-returned-to phase | `phase_card_viewed` breakdown | Track only | Mid-luteal = #1 |

### The One Metric That Matters Right Now

> **Unprompted Day-14 return rate.**

Not Day-28 — that's a Flare metric. For Phlow as a signal project, Day-14 is sufficient and honest: it means someone returned at roughly the mid-cycle point with zero email, zero push, zero login. Pure content pull.

If this number is above 35%, the content format resonates. That's the Flare green light.

If it's below 20%, the content isn't landing — and Flare needs a different approach before building.

---

## Channel Playbook — Tier by Tier

### Tier 1 — High Trust, Immediate (Do This Now)

**Personal DMs (Weeks 1–4)**
- Target: 20 women founders, freelancers, operators in Denis's network
- Message format: "I built something weird. Not a period tracker. 5 seconds to tell you what to work on today, based on your cycle. Can you try it?" + link
- Do not pitch. Do not explain. Let the product speak.
- Follow up once: "What do you think?"
- Capture: install? Returned? Said what?

**MCAS/POTS/Endometriosis Communities (Month 2)**
- Platforms: Reddit (r/MCAS, r/POTS, r/endometriosis), Facebook groups
- Approach: organic, not promotional. Contribute before sharing. Lead with the problem.
- Opening line: "Anyone else notice their worst symptom days are phase-specific? Found something that maps that to work planning."
- Why this audience converts fast: they already track their cycle obsessively; Phlow gives it an actionable layer they've never had.

**Women Founder Communities (Month 2–3)**
- Targets: Female Founder Collective Discord, Chief (where accessible), local women founder Slack groups (city-level)
- Do NOT post a product link cold. Share the *insight* first:
  - "I keep hearing women founders say they crashed on day 26 of their cycle after a sprint. There's actual neuroscience behind why that happens. Anyone else managing this?"
- Then: "I built something for this." Only after trust is earned.

---

### Tier 2 — Content That Compounds (Month 2+)

**TikTok — Format that works:**
- "I tracked my work output for one full cycle. Here's what I found." (face-to-camera, messy and real)
- "The reason your productivity crashes every month isn't discipline — it's biology." (hook, then card demo)
- "What my cycle taught me about scheduling" (story format, no tech speak)
- Rule: never show the UI before showing the problem. The science is the hook.

**Instagram — Format that works:**
- Phase cards as shareable graphics (screenshot-native design)
- Carousel: "The 4 cognitive modes of your cycle" (each slide = one phase)
- Quote cards from real user aha moments
- Reels: same format as TikTok, repurposed

**LinkedIn — Founder angle:**
- Long-form post: "I stopped scheduling my biggest pitches on day 26. Here's the research behind why."
- Data story: "I ran an experiment: scheduling by cycle phase for 90 days. The results surprised me."
- Target: women founders, women in leadership, productivity-adjacent audience

**Content Rule:** Never produce content that could appear on a generic wellness Instagram. Every post must cite science or show real behavior change.

---

### Tier 3 — PR and Credibility (Month 5–6)

**Journalist Pitch (3 targets, personal email, not press release)**

Target publications: Fast Company (Future of Work), Refinery29, Well+Good, The Lily, Quartz

Pitch structure:
```
Subject: The cognitive science behind why women shouldn't schedule pitches on day 26

[1 sentence personal intro]

There's a peer-reviewed study (Xu et al., 2022, n=79) showing that mid-luteal phase 
creates measurable cognitive advantages in task-switching, divided attention, and 
impulse control — but high workload cancels it.

I built a free tool that translates this into daily work recommendations.

[X] women in [community/profession] have been using it for [timeframe].
Here's one of their stories: [aha moment quote + attribution]

Happy to share the research, the data, or an interview with a user.

[Name]
```

**Podcast Pitches (Month 6+):**
- Target shows: How I Built This (women episodes), Dare To Lead, She Did It Her Way, The Huberman Lab (women's health adjacent), Ness Labs podcast, My First Million (if women angle)
- Pitch angle: "The productivity hack hidden in peer-reviewed neuroscience that no one is building for"

---

## The Mafia Offer (Finalized for Phase 2 Gate)

> An offer so good that saying no feels stupid.

**What:**
- Access the full 28-day cycle preview + cycle history + custom task types
- Price: €4.90/month
- Add-on for founding users: Lifetime premium for the first 100 women who post an aha moment in the community

**Why it's a mafia offer:**
1. The free tier gives real daily value — you're not paying to try
2. The preview answers a question you're already asking ("what should I protect next week?")
3. No data stored — you keep full control. No lock-in.
4. Backed by published peer-reviewed science, not wellness intuition
5. Built by someone who has the same problem (founder credibility)

**Pre-launch validation process (Running Lean):**
Before building Phase 2 payment flow, Denis manually collects 8 verbal/written commitments to pay €4.90/month from women who have used the free tier. If <8, do not build. Instead, identify what's missing.

---

## Organic Growth Loops (What Makes This Compound)

The best marketing for Phlow happens when users do it themselves. Build toward these three loops.

### Loop 1 — The Screenshot Loop
```
User sees their mid-luteal card → Has aha moment → Screenshots it
→ Sends to a friend in a WhatsApp/DM → Friend installs → Loop repeats
```
**Enable this:** ✅ Done — "Share with a Phlowie" button is live in DailyCard. Native share sheet on mobile (Web Share API), clipboard fallback on desktop. Tracks `card_shared` event. Cards show phase name, key insight, and tip in one frame — screenshottable by design.

### Loop 2 — The Community Loop
```
User joins Telegram → Posts phase check-in → Another user engages
→ Social validation of cycle phases → Both users open Phlow more
→ Both refer more people
```
**Enable this:** Daily `#phase-of-the-day` prompt from Denis. Make the first post easy.

### Loop 3 — The Content Loop
```
Denis/team publishes science-backed content → Someone shares it
→ New user discovers Phlow → Converts to community member
→ Posts their aha moment → That post becomes new content
→ Loop repeats
```
**Enable this:** Every piece of content must have a clear CTA to Phlow or the community. Not "download the app" — "see what your phase says today."

---

## Constraints and Guardrails

**DO NOT:**
- Launch paid ads until Day-28 retention >40% is proven — ads on a leaky bucket burn money
- Create a generic content calendar — all content must be grounded in specific users, specific phases, specific science
- Use wellness-speak ("harmonize," "flow state," "honor your body") — it actively repels the target user
- Build Phase 2 features before 8 pre-commit paying users are secured
- Expand to secondary audiences (partners, teams, B2B) before PMF on primary segment

**DO:**
- Document every user quote, every aha moment, every piece of language users use — this language owns the copy
- Run every channel as a timed experiment with a defined pass condition
- Share progress in the community — transparency builds trust and retention
- Read `RESEARCH.md` before every piece of content — the science is the unfair advantage

---

## The One-Page Summary

```
WHAT PHLOW IS:    Signal project proving content resonance before Flare is built.

WHY ZERO ONBRD:   No account = no artificial retention = only honest signal counts.

RISKIEST BET:     Do women return on Day 14 with zero prompting? → This proves Flare.

PLG ENGINE:       Open app → see today's phase → aha moment → screenshot → share

COMMUNITY:        Telegram founding community → 100 women → proof engine for Flare

GROWTH ORDER:     Personal DMs → community → organic content → PR → paid (never yet)

KEY METRIC:       Unprompted Day-14 return rate  (>35% = Flare green light)
SECONDARY:        PWA install rate + referral/share as primary referrer source

REVENUE:          Not a Phlow goal. A Flare goal. Phlow's job is to prove the behavior.

FLARE GATE:       Day-14 return >35% sustained over 8 weeks + 30+ community members
                  + 5+ unprompted referrals → Begin Flare architecture.
```

---

*Strategy is useless without specificity. The next action is always a single name, a single message, a single post. Start there.*
