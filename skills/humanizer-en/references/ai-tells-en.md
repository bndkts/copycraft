# English AI-tell catalogue (humanizer-en)

The full catalogue the `humanizer-en` skill draws on, plus the voice-calibration
procedure. This list is **English-tuned**: these are the patterns that mark *English*
machine prose. German AI-generated copy has its own, different tells (Über-Nominalisierung,
Floskel-Einstieg, Konnektoren-Ketten) — for German use `humanizer-de`, never a translation
of this file.

> **Source.** The smell list is built on Wikipedia's "Signs of AI writing" guide (the same
> basis as the bundled `humanizer` skill). Treat every item here as a **contested style
> smell**, not a grammatical error: cut it by default, but keep the word or structure when
> it is genuinely the most accurate one. The job is to make text read like a specific human
> wrote it — not to sand it into beige "AI-clean" output. All examples below are **original
> and constructed** (brand-protection / anti-phishing domain), not copied from any site.

## Contents

1. Em-dash overuse
2. AI vocabulary
3. Rule of three on autopilot
4. Negative parallelism ("It's not just X — it's Y")
5. False ranges ("from startups to enterprises")
6. Vague attributions ("studies show")
7. Promotional puffery ("world-class")
8. Superficial -ing analyses ("highlighting the importance of…")
9. Inflated symbolism / grandiosity
10. Filler phrases ("it is important to note that…")
11. Passive voice that hides the actor
12. Voice calibration — match the user's own writing
13. The few genuine errors (hard rules)

---

## 1. Em-dash overuse

**What it is.** A paragraph where the em dash (—) does most of the punctuation work —
clause after clause hung off dashes — like this — instead of full stops and commas.

**Why it reads as AI.** Models reach for the em dash as a default connective; humans vary
their punctuation. A page where every other sentence has a dash feels machine-paced.

**Fix.** Keep at most one em dash where it earns a genuine dramatic break; convert the rest
to periods (for a hard stop), commas (for a soft aside), or a colon (to introduce). Vary
the rhythm.

- ✗ *We scan the web — around the clock — and flag fakes — usually within the hour — so you
  never find out too late.*
- ✓ *We scan the web around the clock and flag fakes, usually within the hour. You never
  find out too late.*

Note: the dash itself is not an error. **Overuse** is the smell. Don't crusade against every
dash — strip the pile-up.

---

## 2. AI vocabulary

**What it is.** A cluster of words models over-produce: *delve, tapestry, realm, robust,
seamless, leverage, navigate (the landscape), underscore, testament, beacon, bustling,
ever-evolving, fast-paced.* Add the marketing cousins *empower, unlock, elevate, harness,
streamline, foster.*

**Why it reads as AI.** Each is a generic upgrade of a plain word. Stacked, they signal that
no specific person chose them.

**Fix.** Swap for the plain verb or noun the sentence actually means. Keep one only when it
is the precise word — e.g. "robust" for a security claim that really is robust, "leverage"
in a finance context where it has a literal meaning.

| Tell | Plain fix |
|---|---|
| delve into | look at, dig into, go through |
| leverage | use |
| robust suite of tools | tools that hold up / that work |
| seamless | smooth, with no extra steps |
| navigate the landscape | handle, deal with, get through |
| underscore | show, stress, point to |
| a testament to | shows, proves |
| ever-evolving / fast-paced | changing, busy (or cut the adjective) |
| unlock / empower / elevate | let you, help you (or name the concrete outcome) |

---

## 3. Rule of three on autopilot

**What it is.** Triads everywhere: "fast, simple, and powerful"; "detect, protect, resolve";
"secure, scalable, and seamless." Three items feel complete, so models default to three even
when only one is true or load-bearing.

**Why it reads as AI.** Real emphasis is uneven. When every list is exactly three balanced
adjectives, the rhythm becomes a tic.

**Fix.** Keep the one that is true and provable; cut the padding. If you keep a triad, make
the three items genuinely distinct and earned, not synonyms.

- ✗ *A fast, simple, and powerful way to protect your brand.*
- ✓ *Fakes flagged within the hour — and taken down for you.* (pick the real promise)

---

## 4. Negative parallelism ("It's not just X — it's Y")

**What it is.** The construction "It's not just X, it's Y" / "This isn't about X. It's about
Y." It manufactures contrast and gravitas without adding information.

**Why it reads as AI.** It is a rhetorical template, not a thought. It tells the reader how
to feel instead of giving them a reason to.

**Fix.** Delete the frame and state Y plainly. If X carried real meaning, keep it as a
straight statement.

- ✗ *It's not just monitoring — it's peace of mind.*
- ✓ *You hear about a fake shop the hour it launches, not weeks later from an angry
  customer.*

---

## 5. False ranges ("from startups to enterprises")

**What it is.** "From X to Y" framing that pretends to span a spectrum but just means
"everyone": *from startups to enterprises, from healthcare to finance, from small teams to
global organizations.*

**Why it reads as AI.** It is filler that gestures at breadth while saying nothing specific.

**Fix.** Cut it, or replace with the one segment you actually serve and a real number.

- ✗ *Trusted by organizations from startups to enterprises.*
- ✓ *Trusted by 1,200 e-commerce security teams.* (use real proof; never fabricate — see §13)

---

## 6. Vague attributions ("studies show")

**What it is.** Authority with no source: *studies show, experts say, research suggests,
it's widely regarded, many believe, industry leaders agree.*

**Why it reads as AI.** It borrows credibility the text hasn't earned and can't be checked.

**Fix.** Name the source and the number, or cut the claim. Do **not** invent a study to
keep the sentence — that is the one unforgivable error (see §13).

- ✗ *Studies show that phishing attacks are on the rise.*
- ✓ *Anti-Phishing Working Group counted 1M+ phishing sites in Q1 2024.* (only if real)
- ✓ (or just cut it and lead with the reader's own stake)

---

## 7. Promotional puffery ("world-class")

**What it is.** Self-congratulation with no evidence: *world-class, cutting-edge,
best-in-class, game-changing, industry-leading, state-of-the-art, next-generation,
revolutionary, unparalleled.*

**Why it reads as AI.** It is the English twin of German Floskeln. A competitor could paste
the exact sentence onto their own site without it becoming false — the **competitor
copy-paste test**.

**Fix.** Replace the adjective with the fact that would earn it: a number, a named customer,
a mechanism, a guarantee.

- ✗ *Our world-class, cutting-edge platform delivers best-in-class protection.*
- ✓ *GDPR-compliant, data hosted in Germany, takedowns confirmed within 24 hours.*

---

## 8. Superficial -ing analyses ("highlighting the importance of…")

**What it is.** A trailing participial clause that gestures at significance instead of
stating a fact: *…, highlighting the importance of brand security* / *…, showcasing its
ability to scale* / *…, reflecting a growing trend* / *…, emphasizing the need for vigilance.*

**Why it reads as AI.** It is editorializing wallpaper. The clause adds a verdict the reader
didn't ask for and no evidence backs.

**Fix.** Cut the clause, or replace it with the concrete consequence.

- ✗ *We removed 4,000 fake shops last year, highlighting the importance of monitoring.*
- ✓ *We removed 4,000 fake shops last year. Each one was live for under 48 hours.*

---

## 9. Inflated symbolism / grandiosity

**What it is.** Cosmic framing for an ordinary product: *in a world where…, more than ever
before, the cornerstone of, a beacon of trust, stands as a testament to, ushering in a new
era of.*

**Why it reads as AI.** The stakes are inflated past what the product delivers, so the reader
discounts everything that follows.

**Fix.** Drop to the reader's actual, concrete stake. Smaller and true beats grand and empty.

- ✗ *In a world where trust is everything, we stand as a beacon of brand security.*
- ✓ *When a fake shop uses your name to scam customers, you lose the sale and the trust. We
  take the fake down.*

---

## 10. Filler phrases ("it is important to note that…")

**What it is.** Throat-clearing that delays the point: *it is important to note that, it is
worth mentioning, in today's fast-paced world, when it comes to, at the end of the day, needless
to say, in order to, due to the fact that.*

**Why it reads as AI.** Models open with a wind-up. Humans who know their point lead with it.

**Fix.** Delete the opener and start at the verb. Front-load (inverted pyramid).

- ✗ *It is important to note that, in today's fast-paced digital world, monitoring matters.*
- ✓ *A fake shop can be live for weeks before you notice. Monitoring closes that gap.*

Quick swaps: *in order to* → *to*; *due to the fact that* → *because*; *a number of* →
*several / dozens*; *in the event that* → *if*; *has the ability to* → *can*.

---

## 11. Passive voice that hides the actor

**What it is.** Constructions that drop who does the thing: *fake sites are detected and
removed, your brand is protected, results are delivered.* By whom? When the agent matters,
the passive buries it.

**Why it reads as AI.** Passive is the path of least resistance for a model and it drains
agency from the copy. For a security/trust brand it is actively harmful — the reader wants
to know **who** acts and **how fast**.

**Fix.** Name the actor and use an active verb. Keep the passive only when the actor is
genuinely unknown or irrelevant.

- ✗ *Impersonation attempts are identified and taken down.*
- ✓ *We spot the impostor account and file the takedown — usually within the hour.*

(Aim is not "zero passive." It is "no passive that hides an actor the reader cares about.")

---

## 12. Voice calibration — match the user's own writing

The biggest difference between a real edit and a generic "clean-up" is **rhythm**. Default
humanizing produces correct, flat prose. If the user gives you a sample of their own
writing, match *them* instead.

**When to do it.** Whenever the user supplies (or you ask for) 2–3 paragraphs of their own
writing — a past email, a blog post, a Slack message they're happy with. Calibrate before
you rewrite.

**Procedure.**

1. **Read the sample for its fingerprint, not its content.** Note:
   - **Sentence length and variance** — short and punchy? long and winding? a mix? Measure
     the rough average and the spread.
   - **Punctuation habits** — do they use dashes, semicolons, parentheticals, ellipses,
     one-line paragraphs? How often?
   - **Contractions and register** — "we're / don't / you'll" vs. "we are / do not"; formal,
     casual, or in between.
   - **Vocabulary level** — plain Anglo-Saxon words or longer Latinate ones? Any field
     jargon they use comfortably?
   - **Idiosyncrasies** — favorite connectives ("So,", "Look,", "Here's the thing"), rhetorical
     questions, sentence fragments, signature phrasings.
   - **Person and stance** — first person "I/we", direct "you", or detached third person.

2. **Write a one-line voice note** back to yourself, e.g. *"Short declaratives, ~10 words,
   heavy on 'you', no em dashes, contractions throughout, dry not hyped."* This is your target.

3. **Rewrite to that fingerprint** — remove the AI tells (§1–§11) *and* bend the rhythm,
   length, and word choice toward the sample. A humanized line that doesn't sound like the
   user has only half-succeeded.

4. **Preserve, don't impose.** Calibration matches the user's existing voice; it does not
   invent a new one or copy the *content* of the sample. If the sample and the brand brief
   disagree on register, flag it and ask which wins.

**If no sample is available.** Don't stall. Infer voice from the copy you're fixing and from
any `brand-brief.md` present (voice adjectives and anti-adjectives, du/Sie does not apply in
English but formality does, glossary, banned words). Produce a clean, plain, human default —
and tell the user that giving you 2–3 paragraphs of their writing will make the next pass
sound like them.

---

## 13. The few genuine errors (hard rules)

Most of this catalogue is contested style — downgrade, don't forbid. A short list are real
errors, fix them every time:

- **Never fabricate proof.** Filling a vague attribution (§6) or a false range (§5) with an
  invented study, customer count, or statistic is the one unforgivable move. Use a bracketed
  placeholder — `[X brands protected]`, `[name the study]` — for the user to fill.
- **Number & currency mechanics.** Group thousands ("$50,000", not "$50000"); keep one
  format across the page; symbol and amount stay together ("$1,999" or "1,999 USD", never a
  stray "$ 1999").
- **Quotation marks.** Pick straight (") or curly (") and stay consistent — don't mix them
  in one document.
- **Don't contradict the brand brief.** Voice, banned words, glossary, and the formality it
  sets are rules, not suggestions.

Everything else here is a **smell**: cut by default, keep when it is genuinely the best word.
"Robust" can be exactly right for a security claim; one em dash can land a real beat.
Improve — don't blandify.

---

## Optional enrichment (not required)

This file is self-contained. If the full `copycraft` plugin is present, you may also draw on
`shared/references/conversion-principles.md` (the competitor copy-paste test, the "Seven
Sweeps", front-loading) and `examples/before-after-en.md` (constructed before/after pairs).
The skill works without them.
