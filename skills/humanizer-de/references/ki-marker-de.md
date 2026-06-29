# KI-Marker DE – die deutsche Liste

Lies diese Datei, bevor du einen Text **menschlicher** machst. Sie ist die eigenständige
Werkzeugkiste von `humanizer-de` und enthält alles, was du brauchst – sie funktioniert
allein, auch wenn du den Skill-Ordner aus dem Plugin herauskopierst.

> **Wichtig: Dies ist KEINE Übersetzung der englischen Marker-Liste.** Deutsche KI-Sprache
> hat eigene Verräter. Die englischen Tells („delve“, „tapestry“, „realm“, Em-Dash-Flut,
> „rule of three“ als Vokabel-Tic) treffen das Deutsche nur teilweise. Diese Liste ist
> **nativ für das Deutsche gebaut**: Über-Nominalisierung, Behördington, gestapelte
> Floskeln, mechanische Konnektoren-Ketten. Wer die englische Liste übersetzt, übersieht
> genau das.

**Hard Rule vs. umstrittener Stil:** Diese Datei trennt **harte Regeln** (objektive Fehler
im Standarddeutsch) von **umstrittenem Stil** („Smells“, die du herunterstufst, aber
**nie** verbietest). Wo eine Regel umstritten ist, steht die Quelle dabei.

---

## Inhaltsverzeichnis

1. [Warum deutsche KI-Marker anders sind als englische](#1-warum-deutsche-ki-marker-anders-sind-als-englische)
2. [Die sechs Marker – Tabelle mit Fix](#2-die-sechs-marker--tabelle-mit-fix)
3. [Über-Nominalisierung im Detail](#3-über-nominalisierung-im-detail)
4. [Floskel-Einstiege – die Blacklist der Anläufe](#4-floskel-einstiege--die-blacklist-der-anläufe)
5. [Mechanische Konnektoren-Ketten](#5-mechanische-konnektoren-ketten)
6. [Übervorsichtige Sie-Steifheit / Behördington](#6-übervorsichtige-sie-steifheit--behördington)
7. [Importierte Dreierfiguren & Scheinparallelismen](#7-importierte-dreierfiguren--scheinparallelismen)
8. [Leere Superlative & generische „Lösungen“](#8-leere-superlative--generische-lösungen)
9. [Floskeln-Blacklist (die Ersetzungsliste)](#9-floskeln-blacklist-die-ersetzungsliste)
10. [Trust-Vokabular – womit du Floskeln ersetzt](#10-trust-vokabular--womit-du-floskeln-ersetzt)
11. [Voice-Kalibrierung](#11-voice-kalibrierung)
12. [Harte Regeln vs. umstrittener Stil](#12-harte-regeln-vs-umstrittener-stil)
13. [Checkliste](#13-checkliste)

---

## 1. Warum deutsche KI-Marker anders sind als englische

Englische KI-Glättung jagt Em-Dashes, „delve/tapestry/robust“, „It's not just X – it's Y“,
vage Zuschreibungen („studies show“). Diese Tics gibt es im deutschen Text nur teilweise –
und sie sind nicht das, was deutschen KI-Text entlarvt. Deutsche KI-Sprache klingt **steif,
verschachtelt und feierlich**, nicht poliert-werblich. Ihre Marker:

| Englisch (humanizer-en) | Deutsches Gegenstück – eigener Marker |
|---|---|
| Em-dash overuse | **Über-Nominalisierung** (Substantiv-Ketten statt Verben) |
| „In today's fast-paced world…“ | **Floskel-Einstieg** „In der heutigen schnelllebigen Welt…“ |
| Filler-Konnektoren („Moreover, Furthermore“) | **Mechanische Konnektoren-Ketten** „Darüber hinaus … Zudem … Des Weiteren“ |
| Passive voice hiding the actor | **Übervorsichtige Sie-Steifheit / Behördington** |
| Rule of three on autopilot | **Importierte Dreierfiguren** (aus dem Englischen gekippt) |
| Promotional puffery („world-class“) | **Leere Superlative & generische „Lösungen“** |

Die rechte Spalte ist nativ deutsch gedacht – nicht aus der linken übersetzt. Das ist der
Punkt dieser Datei.

---

## 2. Die sechs Marker – Tabelle mit Fix

| # | Marker | Wie er klingt (✗) | Fix (✓) |
|---|---|---|---|
| 1 | Über-Nominalisierung | „Zur Gewährleistung der Sicherstellung der Überwachung“ | Verben: „damit wir lückenlos überwachen“ |
| 2 | Floskel-Einstieg | „In der heutigen schnelllebigen Welt…“ | Ersten Satz streichen, mit der Sache einsteigen |
| 3 | Konnektoren-Kette | „Darüber hinaus … Zudem … Des Weiteren …“ | Höchstens einen behalten, Gedanken inhaltlich verbinden |
| 4 | Sie-Steifheit | „Wir möchten Sie höflich darauf hinweisen, dass…“ | Direkt: „Bitte beachten Sie“ oder die Aussage selbst |
| 5 | Importierte Dreierfigur | „leistungsstark, zuverlässig und vertrauenswürdig“ | Das eine wahre Wort, Rest streichen |
| 6 | Leerer Superlativ | „der beste Markenschutz am Markt“ | Zahl / Mechanismus / Beleg – oder streichen |

---

## 3. Über-Nominalisierung im Detail

Der häufigste deutsche KI-Marker. Substantivierungen enden auf **-ung, -heit, -keit,
-tion, -ive, -anz, -tät, -nis, -tum**. KI stapelt sie zu blassen Ketten; Verben machen den
Text wieder lebendig und zeigen, **wer** handelt.

| Nominalstil (KI, steif) | Verbalstil (menschlich) |
|---|---|
| Zur Durchführung der Analyse | Um zu analysieren |
| Die Implementierung der Optimierung | Wir optimieren |
| Unter Berücksichtigung der Ergebnisse | Wir berücksichtigen die Ergebnisse |
| Zur Gewährleistung der Sicherheit Ihrer Marke | Damit Ihre Marke sicher bleibt |
| Die Durchführung der Überwachung erfolgt automatisiert | Wir überwachen automatisch |

**Funktionsverbgefüge → starke Verben:** Beachtung schenken → beachten · Hilfe leisten →
helfen · in Anspruch nehmen → beanspruchen · zur Sprache bringen → ansprechen · eine
Entscheidung treffen → entscheiden · zur Durchführung bringen → durchführen · Gültigkeit
haben → gilt.

**Begleiterscheinung Passiv:** KI versteckt den Handelnden gern im Passiv. „Der Bericht
wurde erstellt“ → „Wir haben den Bericht erstellt.“ Aktiv vor Passiv (Faustregel ≤ 10 %
Passiv); bei einer Vertrauensmarke ist es wichtig, dass man sieht, wer handelt.

---

## 4. Floskel-Einstiege – die Blacklist der Anläufe

Der „Anlauf“ ist reiner Leerlauf vor der ersten Information. Streich ihn ganz und steig
mit der konkreten Sache ein. Typische KI-Einstiege (alle streichen):

- „In der heutigen schnelllebigen Welt…“
- „In einer zunehmend digitalen / vernetzten Welt…“
- „Mehr denn je…“ / „Heutzutage ist es wichtiger denn je…“
- „In Zeiten von [X]…“
- „Es ist allgemein bekannt, dass…“ / „Es lässt sich nicht leugnen, dass…“
- „Stellen Sie sich vor, …“ (als reflexhafter Aufhänger ohne Substanz)

**Fix:** Der erste echte Satz ist der mit der ersten echten Information. Beispiel: statt
„In der heutigen digitalen Welt ist Markenschutz wichtiger denn je.“ → „Jeden Tag gehen
Dutzende gefälschter Shops unter Ihrem Namen online.“

---

## 5. Mechanische Konnektoren-Ketten

KI gliedert sichtbar: Jeder Absatz beginnt mit einem Aufzählungs-Konnektor. Das wirkt wie
eine abgehakte Liste, nicht wie ein Gedankengang.

Typische Kette: „Darüber hinaus … Zudem … Des Weiteren … Nicht zuletzt … Abschließend
lässt sich festhalten …“. Auch: „Einerseits … andererseits“, wenn rein dekorativ.

**Fix:** Höchstens **einen** Konnektor behalten und ihn dort setzen, wo er wirklich eine
logische Beziehung trägt (Gegensatz, Folge, Begründung). Sonst die Gedanken inhaltlich
verbinden oder zu kurzen, eigenständigen Sätzen machen. Variiere: „auch“, „dazu kommt“,
„und“, schlicht der nächste Satz. Aufzählungs-Konnektoren sind kein Ersatz für einen roten
Faden.

---

## 6. Übervorsichtige Sie-Steifheit / Behördington

Sie sein heißt **nicht** steif sein. Man kann warm siezen. KI verwechselt Höflichkeit mit
Aufblähung und produziert Amtsdeutsch.

| Aufgebläht (✗) | Direkt (✓) |
|---|---|
| „Wir möchten Sie höflich darauf hinweisen, dass…“ | „Bitte beachten Sie: …“ / direkt die Aussage |
| „Es sei an dieser Stelle erwähnt, dass…“ | (streichen, Aussage selbst bringen) |
| „Wir gestatten uns, Ihnen mitzuteilen, dass…“ | „Wir teilen Ihnen mit: …“ / direkt |
| „Im Rahmen der Bereitstellung unserer Dienstleistungen“ | „Wenn wir für Sie arbeiten“ |
| „Sollten Sie Fragen haben, stehen wir Ihnen gerne zur Verfügung“ | „Fragen? Schreiben Sie uns.“ |

**Quelle/Hintergrund:** Seriosität kommt aus fehlerfreien Texten, belegten Fakten und
echten Kundenzitaten – nicht aus langen Wörtern (Lamer). Amtsdeutsch-Signale killen:
Nominalstil, Passiv, Schachtelsätze, Funktionsverbgefüge.

**du-Variante:** Auch beim Duzen gibt es KI-Steifheit („Wir würden dich gerne darauf
aufmerksam machen, dass…“). Anrede konsequent halten, nie du/Sie mischen (Details:
`du-sie-check`).

---

## 7. Importierte Dreierfiguren & Scheinparallelismen

Die Dreierfigur ist im Deutschen nicht verboten – aber KI importiert sie reflexhaft aus dem
Englischen, wo sie als „rule of three“ zum Reflex gehört. Im Deutschen klingt die
automatische Dreier-Reihe hohl.

- **Dreier-Adjektiv auf Autopilot:** „leistungsstark, zuverlässig und vertrauenswürdig“,
  „schnell, einfach und sicher“. → Nimm das **eine wahre** Wort, belege es, streich den Rest.
- **Scheinparallelismus / Negativ-Parallele:** „Es ist nicht nur ein Tool, sondern eine
  Lösung.“, „Nicht X – sondern Y.“ → Sag die Aussage direkt: „Das Tool meldet gefälschte
  Profile automatisch.“
- **Importierte Floskel-Trias:** „Menschen, Prozesse und Technologie“, „heute, morgen und
  in Zukunft“. → Konkretisieren oder streichen.

**Test:** Trägt jedes der drei Glieder eine eigene Information? Wenn nicht, ist die Dreier-
Figur Dekoration.

---

## 8. Leere Superlative & generische „Lösungen“

KI greift zu Superlativen und Abstrakta, weil sie keinen konkreten Beleg hat. Deutsche
Zurückhaltung schlägt englischen Hype: Substanz überzeugt, gestapelte Superlative wirken
leer.

- Leere Superlative: „der beste … am Markt“, „die führende Plattform“, „höchste Qualität“,
  „maximale Sicherheit“. → Zahl / Mechanismus / Beleg, oder streichen.
- Generische „Lösungen“: „maßgeschneiderte Lösungen“, „Lösungen aus einer Hand“,
  „ganzheitlicher Ansatz“. → Konkret benennen, was das Produkt tut.

**Wettbewerber-Test (der schärfste Filler-Detektor):** Könnte ein Mitbewerber den Satz 1:1
auf seine Seite kopieren, ohne dass er falsch wird? Wenn ja, sagt der Satz nichts
Spezifisches – ersetz ihn durch eine Zahl, eine benannte Funktion, einen Mechanismus oder
einen Beleg. **Erfinde dabei nie** Zahlen, Kundennamen oder Zertifikate – markiere die
Lücke und frag nach.

---

## 9. Floskeln-Blacklist (die Ersetzungsliste)

Dies ist die Ersetzungsliste für Marker 5, 6 und 8: jede Floskel durch einen konkreten
Fakt, eine Zahl oder einen Mechanismus ersetzen.

**Adjektive (Worthülsen):** innovativ, ganzheitlich, maßgeschneidert, kundenorientiert,
einzigartig, nachhaltig, hochwertig, zukunftssicher, zukunftsweisend, erstklassig, führend,
leistungsstark, wegweisend, revolutionär, disruptiv, skalierbar (unbelegt).

**Phrasen:** „maßgeschneiderte Lösungen“, „Lösungen aus einer Hand“, „Wir sind für Sie da“,
„Ihre Zufriedenheit ist unser oberstes Ziel“, „Der Kunde steht im Mittelpunkt“,
„Qualität, die überzeugt“, „Wir setzen Maßstäbe“, „Erleben Sie den Unterschied“,
„Wir gehen die Extrameile“, „Ihr starker/kompetenter/verlässlicher Partner“,
„ganzheitlicher Ansatz“.

**Buzzword-Bingo (oft Denglisch):** Synergien (heben), Best Practices, wertschöpfend,
Pain Points, Touchpoints, Customer Journey, Deep Dive, Low-Hanging Fruits, Game-Changer,
proaktiv, Mindset, agil, Ecosystem, Commitment, „out of the box“, „next Level“.

**Test:** „Könnte ein Mitbewerber den Satz 1:1 übernehmen?“ → ja = Floskel = streichen.

---

## 10. Trust-Vokabular – womit du Floskeln ersetzt

Wenn du einen leeren Superlativ entfernst, brauchst du Substanz an seiner Stelle. Im
Security-/Compliance-Feld trägt prüfbares Vokabular, weil es **nachprüfbar** ist:

DSGVO-konform · ISO-zertifiziert · Serverstandort Deutschland · SSL-verschlüsselt · in [N]
Wochen einsatzbereit · über [N] Kunden · Antwort in 24 Stunden · fester Ansprechpartner ·
transparente Preise · Made in Germany · geprüft · nachweislich · revisionssicher.

**Achtung:** Diese Begriffe sind nur dann erlaubt, wenn sie **wahr** sind. Setz keinen
Beleg ein, den du nicht hast – sonst baust du aus einer Floskel eine Falschaussage.
Im Zweifel: Platzhalter markieren (z. B. „[Anzahl Kunden einsetzen]“) und nachfragen.

---

## 11. Voice-Kalibrierung

Das Ziel ist nicht „neutral und korrekt“, sondern „klingt nach **dieser** Person“. Ein
humanisierter Text, der wie jeder andere humanisierte Text klingt, hat die Aufgabe
verfehlt – auch wenn er „besser“ ist als das Original.

**Wenn 2–3 Absätze eigener Texte vorliegen:**
1. **Satzlänge und Rhythmus messen.** Eher kurz und knapp oder lange, ruhige Bögen?
   Mischt die Person kurz und mittel? Bau denselben Rhythmus nach, nicht einen generisch
   „guten“.
2. **Wortwahl und Register.** Lieblingswörter, Grad an Lockerheit, Fachsprache ja/nein,
   Anglizismen ja/nein. Übernimm das Vokabular der Person, nicht das der KI.
3. **Anrede.** du oder Sie – wie in der Probe, konsequent durchziehen.
4. **Eigenheiten respektieren.** Eine rhetorische Frage, ein Gedankenstrich-Einschub, ein
   trockener Schluss – solche Marotten machen die Stimme aus. Glätte sie nicht weg.

**Ohne Probe:** Leite die Stimme aus dem vorhandenen Text ab (was klingt nach Autorin, was
nach KI?) und mach weiter. Bei echter Unsicherheit über Anrede oder Register **kurz
nachfragen**, statt eine generische Fassung zu liefern. Den Markenbrief (`brand-brief.md`),
falls vorhanden, immer zuerst heranziehen – er **schlägt** jede Annahme.

---

## 12. Harte Regeln vs. umstrittener Stil

**Harte Regeln (echte Fehler, immer korrigieren):**
- Kein „in“ vor blanker Jahreszahl: „in 2024“ ✗ → „2024“ / „im Jahr 2024“ ✓.
- Deutsche Anführungszeichen „…“ (oder »…«), nie gerade "…" oder englische “…”.
- Kein Deppenleerzeichen: „Social Media Plattform“ ✗ → „Social-Media-Plattform“ ✓.
- Währung mit Leerzeichen, Symbol **nach** dem Betrag, Dezimalkomma: 1.999,00 €, nicht
  1999€ oder €1,999.00. Prozent mit Leerzeichen: 20 %.
- Gedankenstrich – (Halbgeviert) mit Leerzeichen, nicht der englische Geviertstrich —.

**Umstrittener Stil (Smells, nur abwerten, mit Quelle):**
- „Sinn machen“ – laut Duden umgangssprachlich, aber **Eisenberg** verteidigt es als
  korrekt. In polierter Copy lieber „ergibt Sinn“; ein Fehler ist es nicht.
- „am Ende des Tages“ (Calque von „at the end of the day“) → „letztlich“, „unterm Strich“,
  „im Endeffekt“.
- „nicht wirklich“ (Calque von „not really“) → „eigentlich nicht“, „kaum“.
- „realisieren“ im Sinne von „erkennen“ – laut Bundeskanzlei (CH) ein Bedeutungslehnwort;
  „realisieren“ heißt eigentlich verwirklichen. → „erkennen“, „merken“, „begreifen“.

Diese Smells sind **kein** KI-Marker an sich – verbiete sie nie, stuf sie nur herunter.

---

## 13. Checkliste

- [ ] Markenbrief gelesen (falls vorhanden); Anrede, Glossar, verbotene Wörter übernommen.
- [ ] Stimmprobe genutzt oder Stimme aus dem Text abgeleitet (nicht generisch geglättet).
- [ ] Floskel-Einstieg gestrichen.
- [ ] Über-Nominalisierung zu Verben aufgelöst; Passiv reduziert.
- [ ] Konnektoren-Ketten aufgebrochen (höchstens einer, inhaltlich begründet).
- [ ] Sie-Steifheit / Behördington entkrampft, ohne unhöflich zu werden.
- [ ] Importierte Dreierfiguren / Scheinparallelismen gestrichen.
- [ ] Leere Superlative & generische „Lösungen“ durch Belege ersetzt – nichts erfunden.
- [ ] Anrede konsequent (du/Sie nie gemischt).
- [ ] Harte Regeln (Typografie, Zahlen, „in 2024“) korrigiert; Smells nur abgewertet.
- [ ] Kurze Änderungsliste „was & warum“, an Marker gekoppelt, mitgeliefert.
