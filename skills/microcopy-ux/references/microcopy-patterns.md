# Microcopy patterns — per surface, EN + DE

Pattern tables for `microcopy-ux`. All examples original and constructed.

## Contents
1. The error-message formula
2. Buttons & dialogs
3. Forms & validation
4. Empty, loading, success states
5. The du/Sie hidden-surface checklist
6. Tone by moment

---

## 1. The error-message formula

**What happened → why (only if honestly known) → what to do next.** Every part in the
user's language, no part optional except the "why".

| Situation | ✗ Weak | ✓ Strong |
|---|---|---|
| Upload too large | "Error: file exceeds limit." | "That file is too big (38 MB — the limit is 25 MB). Try compressing it, or send a link instead." |
| Offline | "Network error." | "You're offline. We'll retry automatically as soon as you're back — nothing was lost." |
| Unknown server error | "Something went wrong." | "Something broke on our side — your data is safe. Try again in a minute; if it keeps happening, contact support." |
| Session expired (DE, Sie) | „Die Sitzung wurde aufgrund von Inaktivität beendet.“ | „Ihre Sitzung ist abgelaufen. Bitte melden Sie sich neu an – Ihre Eingaben sind gespeichert.“ |
| Wrong password (DE, du) | „Authentifizierung fehlgeschlagen.“ | „Das Passwort stimmt nicht. Probier es noch einmal – oder setz es zurück.“ |

Rules visible in the table: honest about unknowns ("that's all they tell us"), the next
step inside the message, reassurance only when true ("nothing was lost" must be a fact),
active voice in German, and never a bare system noun ("Authentifizierung") doing the
explaining.

---

## 2. Buttons & dialogs

**Button = verb + object.** The label must survive being read alone.

| Context | ✗ | ✓ EN | ✓ DE |
|---|---|---|---|
| Save form | OK | Save changes | Änderungen speichern |
| Send invoice | Submit | Send invoice | Rechnung senden |
| Destructive confirm | Yes | Delete 3 invoices | 3 Rechnungen löschen |
| Decline destructive | No / Cancel | Keep them | Behalten |
| Paywall | Continue | Choose a plan | Tarif wählen |

**Dialog anatomy (destructive):**
1. Title asks the real question with the object named: "Delete project
   'Website relaunch'?" / „Projekt ‚Website-Relaunch‘ löschen?“
2. Body states scope + consequence: "…and its 14 tasks, permanently. This can't be
   undone." / „…und seine 14 Aufgaben, dauerhaft. Das lässt sich nicht rückgängig machen.“
3. Confirm button **restates the action**; the safe option is concrete ("Keep editing",
   „Behalten“) — "Cancel" is ambiguous when the action itself is a cancellation.

Confirm only destructive/costly actions. If everything confirms, nothing does.

---

## 3. Forms & validation

- **Label** carries the question, always visible. **Placeholder** shows format only
  (`name@firma.de`, `+49 151 …`) — it disappears on focus and must be expendable.
- **Requirements before failure:** password rules, format constraints, and "why do you
  need this?" hints appear at the field *before* the first attempt, not as a slap after.
- **Inline validation** at the field, in the page's language and Anrede: „Bitte geben
  Sie eine vollständige IBAN ein (22 Zeichen).“ — count included, blame absent.
- **Optional over required noise:** mark the exception. If most fields are required,
  mark the optional ones („optional“), not fifteen asterisks.
- Error text belongs to the field it names; a summary at the top links down for long
  forms.

---

## 4. Empty, loading, success states

| State | Job | Pattern |
|---|---|---|
| Empty (first-run) | Teach the first action | Value in one clause + first step + time promise: "No projects yet. Create your first and invite the team — it takes a minute." |
| Empty (filtered/no results) | Prevent the wrong conclusion | Say *why* it's empty: "No invoices match this filter." + reset action. Never reuse the first-run copy here. |
| Loading (fast) | Stay out of the way | Nothing, or a spinner. Words for sub-second waits are noise. |
| Loading (slow) | Buy patience honestly | Name the work + scale: "Importing 240 contacts…" — and never fake precision (a progress bar that lies is worse than none). |
| Success | Confirm + hand over the next step | "Invoice sent to Müller GmbH." + quiet "Send another" / „Rechnung an Müller GmbH gesendet.“ Restraint: the user's success, not the app's celebration. |

---

## 5. The du/Sie hidden-surface checklist

Anrede mixing lives where strings are written late and reviewed never. When touching a
German product, sweep these against the brief's Anrede (they mirror `du-sie-check`'s
audit list):

- Form labels, placeholders, and validation messages
- Tooltips and helper texts
- Error pages (404/500) and maintenance screens
- Cookie banner and consent dialogs
- Email subjects/bodies sent by the product (password reset!)
- Push/system notifications
- Onboarding checklists and empty states
- Settings descriptions and toggles' explanatory lines

The password-reset email is the classic offender: shipped by the auth library's default
template, siezt in a product that duzt.

---

## 6. Tone by moment

Voice is constant; tone flexes **down** with user stress. A rough map:

| Moment | Stress | Tone |
|---|---|---|
| Empty state, onboarding | low | Voice at full color; light touch allowed |
| Routine success | low | Brief, warm, out of the way |
| Form validation | medium | Neutral, concrete, zero wit |
| Payment/security errors, data loss | high | Calm, factual, maximally concrete; no jokes, no exclamation marks, one apology at most |
| Destructive confirmations | high | Sober; the moment belongs to the consequence, not the brand |

The test for any playful string: read it aloud in the voice of a user who just failed
at the thing for the third time. If it grates, it ships stress, not personality.
