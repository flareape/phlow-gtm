# Phlow — Social Media Operations Flow
**Owner:** Denisa Juna  
**Last updated:** May 14, 2026  
**Scheduler:** Postiz (sole platform)  
**Status:** Phase 1 active

---

## Decision: Postiz Only

**Why Postiz over Later:**
- Postiz has a public REST API — automation from VS Code / Make.com / MCP is possible
- Later has no public API — it is a manual-only tool with no automation path
- Preview quality gap in Postiz is solved by verifying natively in TikTok/Instagram before approving (see Section 5)
- As content volume grows, automation saves more time than a visual preview does

**What Postiz covers for Phlow:**
- TikTok (carousel + video)
- Instagram Standalone (feed, reels, stories)
- LinkedIn

---

## 1. Ideal State (Target Workflow — When MCP Is Stable)

```
GitHub Issue (social content brief with hook, caption, platform, date)
    ↓
GitHub Copilot reads issue via Postiz MCP in VS Code
    ↓
Caption reviewed + approved in VS Code
    ↓
Copilot calls Postiz MCP → creates scheduled post with media
    ↓
Postiz publishes to TikTok / Instagram / LinkedIn at scheduled time
    ↓
Analytics fetched back → logged in SOCIAL-CONTENT.md tracking table
```

**What is already in place:**
- Postiz MCP configured in VS Code: `https://api.postiz.com/mcp/[api-key]`
- Postiz REST API working (verified May 13, 2026)
- TikTok integration: **@sheleadsfuture** (Female work balance)
- Instagram integration: **@denisapyxis** (Denisa Juna standalone)
- LinkedIn integration: **Denisa Juna**

**Remaining blocker:** Reload VS Code window (Cmd+Shift+P → Developer: Reload Window) to activate MCP tools. Until then, REST API is used directly.

---

## 2. Current Working Workflow (May 2026)

### 2a. TikTok + Instagram — Video (face-to-cam)

```
1. Talk track / script from CONTENT-CALENDAR-90DAY.md
        ↓
2. Film on phone — raw, no filter, 30–60 seconds
        ↓
3. Edit in CapCut
   - Auto-captions on
   - Trim to time
   - Export WITHOUT watermark (available in CapCut free)
        ↓
4. Upload video file to Postiz
   - Go to Postiz → New Post → select TikTok channel
   - Upload MP4
   - Paste caption from content plan
   - Set privacy: PUBLIC_TO_EVERYONE
   - Set schedule date/time
   - Save as Draft or Schedule
        ↓
5. Verify natively before confirming (see Section 5)
        ↓
6. TikTok publishes at scheduled time
        ↓
7. Wait 24h → repeat for Instagram Reels
   - Upload same raw MP4 (NOT the TikTok export — no watermark)
   - Adapt caption: replace "phlow.work" with "link in bio"
   - Add 5 hashtags at bottom
   - Schedule in Postiz → Instagram channel
```

**Rules:**
- Never repost TikTok-watermarked video to Instagram — Meta's algorithm deprioritises it
- Film once → post raw file to both, separately
- TikTok: 0–3 hashtags max · Instagram: 5 hashtags at bottom of caption

---

### 2b. TikTok + Instagram — Carousel (slides)

```
1. Slide copy from CONTENT-CALENDAR-90DAY.md (hook + body per slide)
        ↓
2. Design in Canva
   - Size: 1080 × 1920px (TikTok + Instagram vertical)
   - One bold statement per slide — large font, nothing small
   - Dark background (#0a0a0a or deep navy) + white text
   - If using background photo:
       · Add rectangle → set colour #0a0a0a → transparency 65%
       · Layer order: photo → rectangle → text
   - Citation "Xu et al., 2022" visible on any science claim slide
   - No wellness aesthetics (no pastels, moons, florals, cursive fonts)
   - Add pages: click "+" in Canva page panel (each page = one carousel slide)
   - Group text + overlay box per slide (Cmd+G) for easy duplication
        ↓
3. Download from Canva
   - Share → Download → PNG → All pages → downloads as ZIP
   - Unzip → numbered PNGs (slide-1.png, slide-2.png ...)
        ↓
4. Upload to Postiz
   - New Post → select TikTok channel
   - Upload all PNGs in order
   - Paste TikTok caption from content plan
   - Schedule
        ↓
5. Verify natively before confirming (see Section 5)
        ↓
6. TikTok carousel publishes
        ↓
7. Wait 24–48h → repurpose to Instagram
   - New Post → Instagram channel
   - Upload same PNGs (no watermark issue — raw images)
   - Adapt caption:
       · Replace "phlow.work" → "link in bio"
       · Remove TikTok-specific CTAs ("save this")
       · Add: #womenfounder #cycleawareness #productivitytips #womenshealth #femalefounder
   - Schedule
```

**Canva slide structure for TK-34 "Lazy or day 26":**

| Slide | Text |
|---|---|
| 1 — Hook | "I used to think I was lazy. / It was day 26." |
| 2 | "Late luteal = progesterone dropping. Not your character. Biology." |
| 3 | "Xu et al., 2022 — cognitive flexibility measurably lower in late luteal vs mid-luteal." |
| 4 | "Not your discipline. Your hormones." |
| 5 — CTA | "Check what phase you're in → phlow.work / Free. No account." |

---

### 2c. LinkedIn — Founder Voice

```
1. Draft written in VS Code (from SOCIAL-CONTENT.md)
        ↓
2. Review: no wellness language, science claims cited, hook in first 2 lines
        ↓
3. New Post in Postiz → LinkedIn channel
   - Paste text
   - No hashtags
   - Schedule Monday or Tuesday 8:00–9:00am
        ↓
4. Publish
```

---

## 3. Verifying Posts Natively Before Approving

Postiz preview is unreliable. Always verify the actual output before the post goes live.

**For TikTok:**
1. Open TikTok app → tap **"+"** → select your video or images
2. Add caption and hashtags
3. Tap **"Drafts"** → save (not published — only you see it)
4. Swipe through carousel / scrub video → check readability, text size, order
5. If good → go back to Postiz → confirm schedule → delete the TikTok draft
6. If broken → fix in Canva/CapCut → re-upload to Postiz

**For Instagram:**
1. Open Instagram → tap **"+"** → select images/video
2. Go through the full carousel flow to the final screen
3. Either: tap **Advanced Settings → Close Friends** (only you see it) → post → check → delete
4. Or: back out without posting — you have seen the preview in-app
5. Fix anything needed → re-upload to Postiz

This takes ~60 seconds and catches all layout issues before anything goes live.

---

## 4. Make.com Automation

### What Make.com is and how it fits

Make.com is a no-code automation platform that runs **in the cloud, 24/7, without you doing anything**. It watches for events (a new GitHub Issue, a post going live, a new database row) and reacts automatically.

It is not connected to VS Code. The three layers work independently:

| Layer | Tool | What it does |
|---|---|---|
| Content writing | VS Code + GitHub Copilot | You write briefs and captions here |
| Scheduling | Postiz (via MCP or REST API) | Posts are created and published here |
| Automation | Make.com | Watches events, triggers actions automatically |

Make.com talks to Postiz via the Postiz REST API (HTTP module). No code needed.

---

### The Full Automated Flow (target state)

This is what happens after you write one GitHub Issue and upload media to Postiz — everything else runs automatically:

```
YOU: Write content brief as GitHub Issue
     (hook, TikTok caption, Instagram caption, media URLs, TikTok date)
        ↓
MAKE.COM watches GitHub for new Issues labelled "social-post"
        ↓
MAKE.COM reads the issue body and extracts:
  - TikTok hook + caption
  - Instagram hook + caption (slightly different)
  - Image/video URLs already uploaded to Postiz
  - TikTok publish date
        ↓
MAKE.COM calls Postiz API → schedules TikTok post for Day 1
        ↓
─── Day 1: TikTok publishes ───────────────────────────────
        ↓
POSTIZ fires a webhook → Make.com receives it
        ↓
MAKE.COM waits 24 hours
        ↓
MAKE.COM calls Postiz API → schedules Instagram post for Day 2
  - Same images (no watermark issue — raw files)
  - Instagram caption (different hook, "link in bio" CTA, 5 hashtags)
        ↓
─── Day 2: Instagram publishes ────────────────────────────
        ↓
MAKE.COM sends message to Telegram community channel:
  "New post just dropped → [TikTok link]
   Same topic, more context → Instagram tomorrow"
        ↓
MAKE.COM logs both posts to Google Sheet:
  date | platform | post ID | caption snippet | status
```

**You only did two things:** wrote the GitHub Issue + uploaded media to Postiz. Everything else was automatic.

---

### GitHub Issue format for Make.com to read

Each content brief should follow this structure so Make.com can parse it reliably:

```
Title: [TK-34] Lazy or day 26 — TikTok carousel

## Platform
TikTok → Instagram (24h delay)

## TikTok date
2026-05-13T18:00:00Z

## TikTok caption
Late luteal isn't a personality trait. It's progesterone dropping.

Peer-reviewed: Xu et al., 2022 (Front Behav Neurosci) — cognitive flexibility
measurably lower in late luteal vs. mid-luteal. Not your discipline. Your hormones.

Check what phase you're in → phlow.work (free, no account)

## Instagram caption
Late luteal isn't a personality trait. It's progesterone dropping.

If you've felt sharp one week and completely flat the next — this is the explanation.

Peer-reviewed: Xu et al., 2022. Free tool: link in bio.

#womenfounder #cycleawareness #productivitytips #womenshealth #femalefounder

## Media
https://uploads.postiz.com/slide1.png
https://uploads.postiz.com/slide2.png
https://uploads.postiz.com/slide3.png
https://uploads.postiz.com/slide4.png
https://uploads.postiz.com/slide5.png

Labels: social-post
```

---

### Telegram community notification

When a post goes live, Make.com sends a message to the Phlow Telegram channel automatically. Template:

**On TikTok publish:**
```
New on TikTok 👀
[post title / hook]
→ [TikTok link]

Instagram version drops tomorrow.
```

**On Instagram publish:**
```
Also on Instagram now →
[Instagram link]
Save it if it's useful.
```

This keeps the Telegram community in the loop without you having to manually post every time.

---

### Scenario build order (priority)

| # | Scenario | Build when |
|---|---|---|
| 1 | TikTok published → wait 24h → schedule Instagram in Postiz | Now — Postiz webhook is ready |
| 2 | Instagram published → send Telegram community message | Now — Telegram bot is easy to set up |
| 3 | GitHub Issue → schedule TikTok draft in Postiz | When GitHub Issue format is agreed |
| 4 | New Supabase install row → personalised Telegram DM | When user base grows |
| 5 | Monday analytics pull → log to Google Sheet | When posts have 7-day data |

---

### Make.com pricing

| Plan | Cost | Operations |
|---|---|---|
| Free | $0 | 1,000 ops/month, 2 scenarios |
| Core | $9/mo | 10,000 ops, unlimited scenarios |
| Pro | $16/mo | 10,000 ops + advanced routing |

Start on Free (covers Scenarios 1 + 2). Upgrade to Core when adding GitHub automation.

### Make.com limitations
- Cannot publish directly to TikTok — must go through Postiz (certified TikTok partner)
- Instagram direct publish goes through Postiz (Meta Business API)
- No visual preview — Make is automation logic only, not a design or scheduling UI
- Each action costs operations — at 3 posts/week the Free plan is sufficient

---

## 5. Hashtag Research

Do this before writing any caption. Use **TikTok Creative Center** (free):  
→ [ads.tiktok.com/business/creativecenter/hashtag](https://ads.tiktok.com/business/creativecenter/hashtag)

**Strategy — mix of sizes per post:**
- 1 large (>500k posts) — reach
- 2 medium (50k–500k) — discoverability
- 1 niche (<50k) — community

**Current hashtag sets:**

| Platform | Tags |
|---|---|
| TikTok | `#womenfounder` `#cycleawareness` `#productivitytips` `#periodscience` |
| Instagram | `#womenfounder` `#cycleawareness` `#productivitytips` `#womenshealth` `#femalefounder` `#periodscience` `#biohacking` |
| LinkedIn | None — algorithm deprioritises hashtag-heavy posts |

---

## 6. Per-Post Publish Checklist

- [ ] Content brief in `CONTENT-CALENDAR-90DAY.md`
- [ ] Caption drafted — no wellness language, citation if science claim
- [ ] Hashtags researched in TikTok Creative Center
- [ ] Media created: Canva (carousel) or CapCut (video)
- [ ] Media uploaded to Postiz
- [ ] Verified natively in TikTok/Instagram app before approving
- [ ] Schedule date/time set in Postiz
- [ ] Post ID recorded in `SOCIAL-CONTENT.md` tracking table
- [ ] 7 days after publish: log saves/shares, note pass/fail
