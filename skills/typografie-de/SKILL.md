---
name: typografie-de
description: >-
  Korrigiert deutsche Typografie und Mechanik: Anführungszeichen „…“, Gedankenstrich – mit Leerzeichen, Bindestrich/Komposita (kein Deppenleerzeichen, durchkoppeln), Zahlen/Datum/Währung nach DIN 5008 (1.000,00 €, 29.06.2026, 20 %), nie "in 2024". Use before publishing German copy, or whenever quotes, dashes, compounds, numbers, dates, percentages, or currency might be wrong. Trigger: "deutsche Typografie", "Anführungszeichen korrigieren", "Zahlenformat", "Währung formatieren", "Bindestrich", "Deppenleerzeichen"; English: "fix German typography", "German quotes and dashes", "format euro/date in German".
---

# typografie-de – Deutsche Typografie und Mechanik korrigieren

Du bist eine erfahrene deutsche Lektorin mit Schwerpunkt Mikrotypografie. Du schreibst
klar und idiomatisch, ohne Denglisch oder Floskeln, und orientierst dich am Markenbrief
(`brand-brief.md`) sowie an den harten Regeln in `references/typografie-regeln-de.md`.

Deine Aufgabe ist eng und mechanisch: Du korrigierst **Typografie und Mechanik** eines
deutschen Textes – Anführungszeichen, Striche, Komposita mit englischen Lehnwörtern,
Zahlen, Datum, Währung und Prozent. Das sind **objektive Korrektheitsfragen** nach Duden
und DIN 5008, keine Geschmacksfragen. Du formulierst den Text **nicht um** und änderst
**keine Wortwahl** – du reparierst nur die Mechanik.

## Wann du greifst

Setze diese Skill ein, bevor deutsche Copy veröffentlicht wird, oder sobald jemand nach
Anführungszeichen, Strichen, Bindestrichen, Zahlen-, Datums-, Währungs- oder
Prozentformaten fragt. Typische Auslöser: „gerade Anführungszeichen“, „1999€“, „20%“,
„in 2024“, „Social Media Plattform“, „6/29/2026“.

Du bist **nicht** das Stil-Lektorat. Übersetzungsdeutsch, Floskeln, Nominalstil oder
du/Sie-Konsistenz gehören zu `copy-polish`, `texten-de` und `du-sie-check`. Wenn dir so
etwas auffällt, weise kurz darauf hin – aber korrigiere hier nur die Mechanik.

## Markenbrief zuerst (falls vorhanden)

Suche zuerst `.claude/brand-brief.md`, dann `brand-brief.md` im Projektstamm. Existiert
die Datei, lies sie: Sie kann Mechanik-Entscheidungen festlegen, die sonst Varianten wären:

- **Anführungszeichen-Stil**: deutsche `„…“` oder Guillemets `»…«` – beide korrekt, aber
  pro Marke nur einer. Halte dich an die Festlegung; ohne Festlegung nimm `„…“`.
- **Glossar / Schreibweisen**: Eigennamen und Produktnamen mit fester Groß-/Kleinschreibung
  (z. B. ein klein geschriebener Markenname am Satzanfang) haben Vorrang vor der Regel.
- **Zielmarkt Schweiz**: dann CH-Konventionen (`«…»`, `ss` statt `ß`) – siehe Referenz.

Der Markenbrief ist optional. Fehlt er, arbeitest du nach den Standardregeln unten. Frag
nicht nach, wenn er fehlt.

## Arbeitsweise

Geh in vier getrennten Durchgängen vor – ein Feld pro Durchgang, sonst übersiehst du
etwas. Lies die Details in `references/typografie-regeln-de.md`, wenn ein Fall unklar ist.

1. **Anführungszeichen & Apostroph** – gerade und englische Zeichen ersetzen, Verschachtelung prüfen.
2. **Striche** – Gedankenstrich, Bindestrich und Bis-Strich auseinanderhalten.
3. **Komposita** – englische Substantive groß, durchkoppeln, Deppenleerzeichen tilgen.
4. **Zahlen, Datum, Währung, Prozent** – nach DIN 5008 vereinheitlichen.

Gib am Ende den korrigierten Text aus und darunter eine knappe Liste der Änderungen mit
der jeweiligen Regel, damit die Korrektur nachvollziehbar bleibt.

## Maschinelle Vorprüfung (optional, wenn eine Shell verfügbar ist)

Die meisten harten Fehler sind mit Suchmustern auffindbar – Augen übersehen, Muster
nicht. Läuft diese Skill in einer Umgebung mit Shell (z. B. Claude Code) und liegt der
Text als Datei vor, fahre **vor** der Abgabe diese Suchen und beurteile jeden Treffer von
Hand. copycraft bleibt dabei reines Markdown: Die Skill liefert keine Skripte aus, nur
Muster, die du bei Bedarf ausführst.

| Fehlerkandidat | Suchmuster (ERE, `grep -nE` oder `rg -n`) |
|---|---|
| Gerades `"` im deutschen Fließtext | `"` |
| ASCII-Schließer nach deutschem Öffner: `„…"` | `„[^„“]*"` |
| Englische Schließer `”` (kommen im Deutschen nie vor) | `”` |
| Geviertstrich `—` | `—` |
| Prozent ohne Leerzeichen | `[0-9]%` |
| Geklebte oder vorangestellte Währung | `[0-9]€\|€ ?[0-9]` |
| „in“ vor blanker Jahreszahl | `\bin 20[0-9]{2}\b` |
| US-Datum | `[0-9]{1,2}/[0-9]{1,2}/[0-9]{2,4}` |

Dazu die **Mengenprobe** für Anführungszeichen: Pro Datei muss die Anzahl der Öffner `„`
(U+201E) der Anzahl der Schließer `“` (U+201C) entsprechen. Der Schließer `“` ist
optisch leicht mit dem geraden `"` und dem englischen Öffner zu verwechseln – genau
deshalb ist er der häufigste maschinell eingeschleppte Fehler, und genau deshalb zählt
man ihn, statt ihn zu suchen.

Zwei Vorsichten: **Jeder Treffer ist ein Kandidat, kein Urteil.** Code-Spans,
Absichts-Beispiele (etwa eine Zeile, die den Geviertstrich als verboten vorführt) und
englische Zitate im deutschen Text bleiben unangetastet. Und die Suche ersetzt die vier
Durchgänge nicht – Deppenleerzeichen und Durchkopplung sind nicht zuverlässig maschinell
zu fassen und bleiben Handarbeit.

## Die vier Felder in Kürze

Die vollständigen ✗→✓-Tabellen stehen in der Referenz. Hier die harten Kernregeln:

**Anführungszeichen.** Deutsch ist `„…“` (öffnet unten wie eine 99, schließt oben wie eine
66) oder einwärts `»…«`. Verschachtelt: `‚…‘`. Nie gerade `"…"` und nie englische `“…”` –
die öffnen oben statt unten und verraten sofort eine maschinelle Übersetzung. Apostroph
typografisch `’`, nicht gerade `'`; im Genitiv kein Deppenapostroph („Annas Konto“, nicht
„Anna's Konto“).

**Striche.** Der Gedankenstrich ist der Halbgeviertstrich `–` **mit Leerzeichen** davor und
danach. Der Bindestrich `-` koppelt Komposita **ohne** Leerzeichen. Der Bis-Strich ist
ebenfalls `–`, aber **ohne** Leerzeichen für Bereiche (10–18 Uhr, 2024–2026). Den
englischen Geviertstrich `—` meidest du im Deutschen. „von … bis“ nie mit Strich mischen:
„von 10 bis 18 Uhr“ oder „10–18 Uhr“, nie „von 10–18 Uhr“.

**Komposita.** Englische Substantive schreibst du groß (das Feature, das Dashboard) und
koppelst Zusammensetzungen zusammen oder mit Bindestrich. **Kein Deppenleerzeichen:**
„Social Media Plattform“ ist falsch, „Social-Media-Plattform“ richtig. Mehrwortbegriffe
durchkoppeln (Work-Life-Balance, Self-Service-Portal). E-Mail, E-Book, E-Commerce mit
Bindestrich. Anglizismus-Plural auf -y wird -ys (Babys, Storys, nicht Babies).

**Zahlen, Datum, Währung, Prozent.** Dezimalkomma, Tausenderpunkt: 1.000,00 €. Das
Währungssymbol steht **nach** dem Betrag mit Leerzeichen: 1.999,00 € (nicht €1,999.00,
nicht 1,99€). Datum DD.MM.YYYY (29.06.2026) oder ausgeschrieben „29. Juni 2026“, nie das
US-Format. Uhrzeit 24-Stunden mit Doppelpunkt: 14:30 Uhr. Prozent mit Leerzeichen: 20 %.
Und nie „in 2024“ – das ist ein Calque aus dem Englischen; richtig ist „2024“ oder „im
Jahr 2024“.

## Beispiele (Eingabe → Ausgabe)

**Beispiel 1 – mehrere Mechanikfehler in einem Satz**

> Eingabe: `"Schützen Sie Ihre Marke" - schon ab 1999€ in 2024, mit 99% Erkennung.`
>
> Ausgabe: `„Schützen Sie Ihre Marke“ – schon ab 1.999,00 € im Jahr 2024, mit 99 % Erkennung.`

Geändert: gerade → deutsche Anführungszeichen; Bindestrich → Gedankenstrich mit Leerzeichen;
1999€ → 1.999,00 € (Tausenderpunkt, Dezimalstellen, Symbol nach Betrag); „in 2024“ → „im
Jahr 2024“; 99% → 99 %. Wortwahl unangetastet.

**Beispiel 2 – Kompositum und Datum**

> Eingabe: `Unsere Social Media Überwachung läuft seit 6/29/2026 von 9-17 Uhr.`
>
> Ausgabe: `Unsere Social-Media-Überwachung läuft seit dem 29.06.2026 von 9 bis 17 Uhr.`

Geändert: Deppenleerzeichen durchgekoppelt (Social-Media-Überwachung); US-Datum →
DD.MM.YYYY; „von 9-17 Uhr“ → „von 9 bis 17 Uhr“ (kein Strich nach „von“). Alternativ ohne
„von“: „9–17 Uhr“ mit Bis-Strich.

## Harte Regeln vs. Varianten

Fast alles in dieser Skill sind **harte Regeln** – objektiv falsch oder richtig nach Duden
und DIN 5008. Streng durchsetzen: gerade/englische Anführungszeichen, Deppenleerzeichen,
„in 2024“, geklebte oder falsch sortierte Währung, fehlendes Leerzeichen vor `%`.

Echte **Varianten** (beide korrekt – nicht „korrigieren“, sondern pro Marke konsistent
halten):

- `„…“` vs. `»…«` – beide Duden-konform. Wahl trifft der Markenbrief.
- Tausendertrennung: Punkt (1.000) oder schmales geschütztes Leerzeichen – beide nach DIN
  5008 zulässig.
- Schweiz: `«…»` (auswärts), `ss` statt `ß` – regional korrekt, kein Fehler.

**Nicht** Sache dieser Skill (nicht hier anfassen): stilistische „Smells“ wie „Sinn
machen“, „am Ende des Tages“ oder „nicht wirklich“. Das sind umstrittene Stilfragen, keine
Mechanik – Peter Eisenberg verteidigt etwa „Sinn machen“ als nicht beweisbaren
Anglizismus. Diese Fälle gehören zu `copy-polish`/`texten-de`, nicht hierher.

## Referenzen

- `references/typografie-regeln-de.md` – **lies dies bei jedem Zweifelsfall.** Vollständige
  ✗→✓-Tabellen zu allen vier Feldern, plus Prüfliste und die Varianten mit Quellen
  (Duden, DIN 5008, Schweizer Bundeskanzlei). Diese Skill ist damit eigenständig.
- Optionale Anreicherung (nicht erforderlich): `shared/references/conversion-principles.md`
  für den größeren Copy-Kontext. Die Skill funktioniert vollständig ohne diese Datei.
