# Email patterns — subjects, preheaders, lifecycle map (EN + DE)

Patterns and length budgets for `email-copy`. All examples are original and constructed.

## Contents
1. Subject-line patterns (EN + DE)
2. Preheader craft
3. The lifecycle map — one job per email
4. Newsletter structure
5. Deliverability & legal checklist

---

## 1. Subject-line patterns (EN + DE)

Aim **≤ ~45 characters**; phones truncate around there, and the operative words must
survive. Front-load. Write 3–5 options, recommend one.

| Pattern | EN example | DE example |
|---|---|---|
| The thing is ready | "Your June report is ready" | „Ihr Juni-Report ist da“ |
| Deadline + what's at stake | "Trial ends Friday — keep your projects" | „Testphase endet Freitag – deine Projekte bleiben“ |
| Their progress as hook | "You're one step from going live" | „Dir fehlt noch ein Schritt bis zum Start“ |
| Useful number | "3 changes to your plan pricing" | „3 Änderungen an Ihren Tarifen“ |
| Plain announcement | "New: export to Excel" | „Neu: Export nach Excel“ |
| Honest question | "Still working on your Spanish?" | „Lernst du noch Spanisch?“ |

**What never works long-term:** bait ("You won't believe…"), fake threads ("Re:" on a
first contact), manufactured urgency, subject/body mismatch. Each buys one open and
costs the next ten.

**German notes:** Betreff is copy — German typography applies (`„…“`, `20 %`, no
Deppenleerzeichen: „Juni-Report“, not „Juni Report“). Calm specificity beats cleverness
for Sie-register brands; du-register consumer brands can be looser but not baity. The
Anrede may appear in the subject; keep it consistent with the body.

---

## 2. Preheader craft

The preheader (preview text) renders next to the subject in the inbox — roughly
**80–100 characters** before truncation. It is the subject's second line, not its echo:

- Subject makes the promise → preheader adds mechanism, proof, or stake.
- ✗ Subject "Your June report is ready" + preheader "Your June report is ready" (echo)
- ✓ … + preheader "Two takedowns confirmed, one new finding — 3 minutes to read."
- Never let it default to "View this email in your browser" or the first nav link —
  that's the most-read line in the email doing no work.

---

## 3. The lifecycle map — one job per email

A sequence is a relay: each email moves the reader to one next state. If an email has
two jobs, split it.

| Email | Trigger | The one job | Craft notes |
|---|---|---|---|
| **Welcome** | signup / opt-in | Confirm the decision; deliver the promised thing; one first step | Highest open rate the sender will ever see — spend it on the first moment of value, not a feature tour or a founder essay. |
| **Activation nudge(s)** | user *hasn't* done X after N days | Remove one hurdle | Behavior-triggered beats calendar-triggered. Name the step, show it takes minutes, link straight into it. One hurdle per email. |
| **Trial-end / upgrade** | N days before expiry | Convert with the user's own usage as proof | "Here's what you built" (real data or placeholder) → what upgrading keeps → what lapsing means, stated plainly, no menace. Friction-reducer at the button. |
| **Win-back** | inactive N weeks/months | One honest second look | What changed since they left, one reason to return, and an easy out. One attempt; a win-back *sequence* is how brands get marked as spam. |
| **Announcement** | you shipped something | Make one change matter to this reader | Lead with what the reader can now do, not "we're excited to announce". |

**Sequence-level checks:** consistent Anrede and sender name across every email;
each subject distinct (no "Reminder: " prefix stacking); the sequence stops when the
job is done (someone who upgraded must not get the trial-end mail).

---

## 4. Newsletter structure

A newsletter earns its slot by being scannable and consistent:

1. **One lead item** — the thing worth opening for, front-loaded in the first two lines
   (they're the preview). Write it like a tiny landing section: point, proof, link.
2. **2–4 short items** — one paragraph each, bolded first words as scan anchors, one
   link each. Cut anything that's filler this issue; shorter beats padded.
3. **A consistent sign-off** — same voice, same place, every issue. Recognizability is
   the newsletter's compounding asset.

The competitor copy-paste test applies to newsletters too: if an item could appear
unchanged in a competitor's newsletter, it's industry filler, not your letter.

---

## 5. Deliverability & legal checklist

Copy-level items only — infrastructure (SPF/DKIM/DMARC) is out of scope for a
copywriting skill, but flag it if the user asks why emails land in spam.

- [ ] **Unsubscribe link** present and honest (one click, no login wall).
- [ ] **Sender identity** real; German senders: **Impressum** in the footer.
- [ ] **Consent**: recipients opted in; for Germany assume **double opt-in** is the
      standard (§7 UWG) — surface this once when a request implies a bought or scraped
      list, then stop.
- [ ] **Subject matches body** — also a spam-complaint driver, not just ethics.
- [ ] **Text-first**: the email works with images off; no image-only emails.
- [ ] Don't contort copy around spam-word folklore; sender reputation dominates. Write
      plainly and the words take care of themselves.

> Not legal advice — when a German sender is unsure about UWG/DSGVO specifics, say so
> and point them to counsel rather than improvising compliance copy.
