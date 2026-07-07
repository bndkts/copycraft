# Eval briefs — fixed inputs for benchmarking skill changes

Five constructed briefs to run **before and after** editing a skill, so a change's
effect on output quality is comparable rather than anecdotal. Run the matching skill on
the same brief at the same settings, then score both outputs against the rubric below
(blind if possible — shuffle which output is which before judging).

These briefs are fixtures: **don't "improve" them**, or every past comparison breaks.
Add new briefs at the end instead.

---

## Brief 1 — German from scratch, Sie, trust-sensitive B2B (`texten-de`)

> Produkt: Plattform für Lieferketten-Compliance (LkSG-Berichte). Zielgruppe:
> Compliance-Verantwortliche im Mittelstand. Belege: Berichte in 2 Wochen statt
> 3 Monaten; 400+ Unternehmen; Serverstandort Deutschland; TÜV-geprüft. Anrede: Sie.
> Ziel: Demo buchen. Liefere Hero, Subhead, CTA und zwei Feature-zu-Nutzen-Blöcke
> (Features: automatischer Lieferantenfragebogen; Risiko-Dashboard).

## Brief 2 — German from scratch, du, B2C app (`texten-de`)

> Produkt: App für Haushaltsbudgets von Paaren. Zielgruppe: Paare Ende 20 bis Ende 30,
> die über Geld streiten. Belege: 100.000 Downloads; Konten bleiben getrennt, Überblick
> gemeinsam; Bankverbindung nur lesend. Anrede: du. Ziel: App installieren. Liefere
> Hero, Subhead, CTA und einen Objection-Absatz („Ich will kein gemeinsames Konto“).

## Brief 3 — English from scratch, plain B2B (`copywriting-en`)

> Product: automated invoice-chasing for agencies. Audience: agency owners who hate
> chasing late payers. Proof: invoices paid [X] days faster on average; polite-by-default
> reminder sequences; used by 900+ agencies. Goal: start free trial. Deliver hero,
> subhead, CTA, and three value props.

## Brief 4 — Localization EN→DE (`lokalisieren-de`)

> Brand: the couples-budget app from Brief 2 (du). Localize this hero + CTA into German:
> "Take control of your shared finances — without giving up your own account. See
> everything in one place, decide together, and stop arguing about money. Get started
> for free today."

## Brief 5 — Polish, German with translationese (`copy-polish`)

> Anrede Sie. Verbessere diesen Abschnitt einer Agentur-Website:
> „Am Ende des Tages macht es Sinn, mit einem Partner zu arbeiten, der die Extrameile
> geht. Unsere innovative Full-Service-Agentur bietet maßgeschneiderte Lösungen aus
> einer Hand und stellt die Realisierung Ihrer digitalen Transformation sicher. Starten
> Sie noch heute durch!“

---

## Rubric — score each output 0–2 per row (2 = fully holds)

| # | Check |
|---|---|
| 1 | **Hard rules clean**: typography (run the `typografie-de` scan patterns on German output), no fabricated proof, one primary CTA. |
| 2 | **Anrede consistent** across every string, including buttons and risk-reducers. |
| 3 | **Competitor copy-paste test**: no line a rival could reuse verbatim. |
| 4 | **Proof carried**: every claim backed by a brief-supplied fact or a bracketed placeholder. |
| 5 | **Native execution**: German reads written-in-German (no calques, Verbalstil, native CTA); English is free of AI-vocabulary tells. |
| 6 | **Voice**: matches brief adjectives; if voice samples exist, rhythm/word choice mirror them. |
| 7 | **Process followed**: variants + judgment for high-stakes units where the skill requires it; refresh-vs-rewrite verdict stated for polish jobs. |
| 8 | **Reader-fit**: benefits lead, features prove; the stated goal's action is the obvious next step. |

Interpretation: a change to a skill should raise (or hold) the total on the briefs that
skill serves, without lowering the others. A rise on one brief bought with a fall on
another is a regression wearing a costume.
