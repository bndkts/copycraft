# Ad formats — limits, combinability, policy pitfalls

Reference for `ads-copy`. All examples original and constructed.

> **Limits drift.** The numbers below were accurate as of mid-2026. Platforms change
> them without ceremony — when an exact limit is load-bearing (it always is), verify in
> the platform's current documentation or ad editor before delivering, and say you did.

## Contents
1. Limits table
2. Google responsive search ads — the combinability craft
3. Meta (Facebook/Instagram) — the fold and the feed
4. LinkedIn — B2B register
5. Policy pitfalls that read as copy problems
6. German character economics

---

## 1. Limits table

| Platform / asset | Limit | Notes |
|---|---|---|
| Google RSA headline | **30 chars**, up to 15 headlines | ≥3 shown, order not guaranteed |
| Google RSA description | **90 chars**, up to 4 | 2 shown |
| Google display path | 15 chars × 2 | vanity URL segments |
| Meta primary text | ~**125 chars visible** before "See more" | hard cap much higher; the fold is what matters |
| Meta headline | ~**27 chars visible** in feed | longer gets truncated per placement |
| Meta description | ~27 chars, shown inconsistently | don't put anything essential here |
| LinkedIn intro text | ~**150 chars** before "…see more" (desktop; less on mobile) | same fold logic as Meta |
| LinkedIn headline | ~70 chars | keep the promise ≤ ~50 to survive mobile |

Treat every "visible before truncation" number as the real budget: what folds is
optional reading, what's above the fold is the ad.

---

## 2. Google responsive search ads — the combinability craft

The mixer assembles your assets; you write materials, not a finished ad.

**Angle checklist — cover most of these across 8–15 headlines, one each:**
- Keyword match ("Salon Booking Software") — earns the bold-match in the SERP.
- Outcome ("Fewer No-Shows, More Revenue")
- Differentiator / mechanism ("SMS Reminders, Sent On Time")
- Proof number ("[1,200]+ Salons On Board" — placeholder until real)
- Offer ("Free 30-Day Trial")
- Friction-reducer ("Set Up In One Afternoon")
- CTA ("Start Your Free Trial")
- Brand (optional — the display URL already carries it)

**Combinability rules:**
- Each headline is a complete thought; any three must read sanely in any order.
- No punctuation that implies sequence ("…", "and", trailing commas).
- Don't repeat one idea in three wordings — the mixer will happily show all three
  together and the ad reads stuttered.
- Descriptions: mechanism + proof + CTA; assume the reader sees exactly two.
- Pin sparingly. A pinned headline shows in that slot always — reserve for legally
  required lines, and know it narrows optimization.

---

## 3. Meta (Facebook/Instagram) — the fold and the feed

- **The first ~125 characters are the ad.** The one promise, complete, before the fold;
  detail after the fold is for the already-interested.
- Primary text is read like a post, not a billboard: one or two short sentences beat a
  slogan. Write in the page's Anrede (German) and the brand's register.
- **Headline** (under the creative) restates the promise in ≤ ~27 visible characters —
  it's a caption, not a second message.
- The **creative carries the stop**; the text carries the claim. If the user has no
  creative brief, note the dependency instead of writing text that must do both jobs.
- Meta ads are archived publicly (Ad Library) — one more reason invented claims are a
  hard error.

---

## 4. LinkedIn — B2B register

- Same fold logic: ~150 characters of intro before "…see more". Lead with the reader's
  problem or the differentiator, not "We're excited to share".
- The audience tolerates substance: a concrete number or named capability outperforms
  feed-style breeziness.
- German B2B on LinkedIn is predominantly **Sie** — but the brief decides; never mix
  registers between ad and landing page.

---

## 5. Policy pitfalls that read as copy problems

Rejections often look like copy mistakes. Avoid writing them in:

- **Excessive capitalization or punctuation** ("FREE!!!") — rejected by Google/Meta
  policy, not just ugly.
- **Unsupported superlatives** ("the best", "#1") without on-page substantiation —
  Google may allow, German competition law (UWG) is stricter; prefer the checkable fact.
- **Personal attributes targeting in the copy** ("Are you diabetic?") — Meta rejects
  copy that implies knowledge of personal characteristics. Address the situation, not
  the person's condition.
- **Trademark terms** in headlines for comparison ads — platform-dependent; flag rather
  than assume.
- **Urgency claims** ("Only today") that aren't literally true — deceptive under
  platform policy and consumer law both.

---

## 6. German character economics

German is ~20–30% longer than English and compounds concentrate the length in single
unbreakable tokens. Inside a 30-character ceiling:

| Instead of | Write | Chars saved |
|---|---|---|
| `Zeiterfassungssoftware testen` (29) | `Zeiten mobil erfassen` (21) | 8, and a verb |
| `Markenschutz-Analyse anfordern` (30) | `Marke jetzt prüfen lassen` (25) | 5, and active |
| `Buchhaltungsautomatisierung` (27) | `Buchhaltung automatisch` (23) | 4, and legible |

Rules that survive the squeeze: verb-first where possible; split forms over monster
compounds *when both are natural German*; abbreviations only if the audience reads them
cold (DSGVO yes, ZE-Software no). **Never** a Deppenleerzeichen to dodge the length —
„Zeiterfassung Software“ is wrong at any character count. Umlauts stay umlauts in ad
copy; only slugs/URLs transliterate.
