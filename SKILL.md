---
name: stop-slop-de
description: Entfernt typische KI-Schreibmuster, Floskeln und unnatürlichen Ton aus deutschen Texten. Für Entwürfe, Redaktion und Textoptimierung.
metadata:
  trigger: Texte verfassen, deutsche Entwürfe überarbeiten, KI-Texte humanisieren
  author: Jochen Gererstorfer (https://github.com/jochen-gererstorfer)
  based_on: Hardik Pandya (https://github.com/hardikpandya/stop-slop)
---

# Stop Slop (DE)

Befreie deutsche Texte von vorhersehbaren KI-Schreibmustern, leeren Floskeln und künstlicher Dramatik.

## Die 8 Kernregeln

1. **Füllwörter und Räusper-Einstiege streichen.** Keine Ankündigungen vor der eigentlichen Aussage, keine leeren Beteuerungen, keine überflüssigen Adverbien. Siehe [references/phrases.md](references/phrases.md).

2. **Formelhafte Satzstrukturen aufbrechen.** Keine binären Schein-Gegensätze („Nicht X, sondern Y“), keine Negationsketten, keine theatralischen Ein-Wort-Sätze, keine rhetorischen Scheinfragen. Siehe [references/structures.md](references/structures.md).

3. **Nominalstil radikal abbauen.** Verben statt Substantiv-Monster. Keine Ketten aus *-ung*, *-keit*, *-heit* oder *-tion*. Schreibe, wer was tut, statt Tätigkeiten zu Substantiven zu erstarren.

4. **Aktiv formulieren und Handelnde benennen.** Jede Aussage braucht ein echtes Subjekt. Vermeide unpersönliche Passiv-Konstruktionen (*„Es wird empfohlen…“*, *„Hierbei lässt sich feststellen…“*). Keine leblose Pseudo-Handlung (*„Die Entscheidung reift heran“* – jemand entscheidet!).

5. **Konkret statt schwammig sein.** Keine vagen Behauptungen (*„Die Auswirkungen sind immens“*). Nenne Zahlen, Fakten oder konkrete Beispiele. Keine faulen Extreme (*„jeder“*, *„immer“*, *„nie“*).

6. **Lesende direkt ansprechen.** Kein distanzierter Dozenten-Tonfall. Konkrete Situationen schlagen Abstraktionen. Sprich dein Gegenüber an (*„Du“* / *„Sie“*), statt von *„den Menschen“* oder unpersönlich von *„man“* zu fabulieren.

7. **Rhythmus variieren.** Satzlängen mischen. Zwei Punkte genügen oft, es muss nicht immer die typische KI-Dreierreihe sein. Absätze unterschiedlich beenden. Gedankenstriche (*Em-Dashes*) streichen oder durch Kommas/Punkte ersetzen.

8. **Dem Leser vertrauen.** Sprich Tatsachen direkt aus. Kein Händchenhalten, keine vorsorglichen Entschuldigungen (*„Und das ist völlig okay“*), keine Kalenderspruch-Pointe am Ende.

## Schnell-Check vor Textabgabe

Vor dem Veröffentlichen prüfen:

- [ ] **Gibt es Füll-Adverbien?** (*wirklich, einfach, buchstäblich, tatsächlich, quasi, quasi-automatisch*) → Streichen.
- [ ] **Steckt ein „Nicht X, sondern Y“-Gegensatz drin?** → Direkt **Y** sagen.
- [ ] **Gibt es Räusper-Floskeln?** (*„Fakt ist:“*, *„Hier ist das Problem:“*, *„Es ist wichtig zu beachten, dass…“*) → Sofort zur Sache kommen.
- [ ] **Ist der Text im Passiv oder „Man“-Modus verfasst?** (*„Es wird beobachtet…“*) → Wer handelt? Zum Subjekt machen.
- [ ] **Handelt ein lebloses Ding wie ein Mensch?** (*„Die Beschwerde wird zur Lösung“*) → Die handelnde Person benennen.
- [ ] **Häufen sich Substantivierungen?** (*„Zur Optimierung der Bereitstellung…“*) → In lebendige Verben umwandeln (*„Um schneller bereitzustellen…“*).
- [ ] **Drei Sätze hintereinander mit ähnlicher Länge?** → Einen Satz aufbrechen oder kürzen.
- [ ] **Endet jeder Absatz mit einem punchigen One-Liner?** → Variieren.
- [ ] **Gedankenstriche (—) im Text?** → Entfernen. Im Deutschen meist durch Komma oder neuen Satz ersetzbar.
- [ ] **Vage Behauptung?** (*„Die Konsequenzen sind weitreichend“*) → Konkret benennen, was passiert.
- [ ] **Meta-Gequatsche?** (*„Im nächsten Abschnitt schauen wir uns an…“*) → Streichen und direkt zum Thema springen.

## Bewertung (Scoring)

Bewerte den Text von 1 bis 10 in fünf Dimensionen:

| Dimension | Prüffrage |
|-----------|-----------|
| **Direktheit** | Direkte Aussage oder endlose Ankündigung? |
| **Rhythmus** | Lebendig und abwechslungsreich oder monotoner Metronom? |
| **Vertrauen** | Respektiert der Text die Intelligenz der Lesenden? |
| **Authentizität** | Klingt der Text nach einem echten Menschen mit Haltung? |
| **Dichte** | Lässt sich noch ein einziges Wort ohne Sinnverlust streichen? |

**Unter 35 / 50 Punkten:** Text überarbeiten.

## Beispiele

Vorher-/Nachher-Vergleiche findest du in [references/examples.md](references/examples.md).

## Lizenz

MIT – frei nutzbar, gerne teilen und erweitern.
Basierend auf [stop-slop](https://github.com/hardikpandya/stop-slop) von Hardik Pandya.
