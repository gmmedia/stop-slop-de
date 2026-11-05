---
name: stop-slop-de
description: Entfernt typische KI-Schreibmuster, Floskeln und unnatürlichen Ton aus deutschen Texten. Für Entwürfe, Redaktion und Textoptimierung.
metadata:
  trigger: Texte verfassen, deutsche Entwürfe überarbeiten, KI-Texte humanisieren
  author: Jochen Gererstorfer (https://github.com/gmmedia)
  based_on: Hardik Pandya (https://github.com/hardikpandya/stop-slop)
---

# Stop Slop (DE)

Befreie deutsche Texte von vorhersehbaren KI-Schreibmustern, leeren Floskeln und künstlicher Dramatik.

## Die 8 Kernregeln

1. **Füllwörter, Räusper-Einstiege und KI-Metaphern streichen.** Keine Ankündigungen vor der eigentlichen Aussage, keine leeren Beteuerungen, keine überflüssigen Adverbien. Vermeide abgedroschene Schmuckwörter (*„Herzstück“*, *„Katalysator“*, *„Wandteppich“*) und mechanische Scharnier-Floskeln (*„Darüber hinaus…“*, *„Des Weiteren…“*). Siehe [references/phrases.md](references/phrases.md).

2. **Formelhafte Satzstrukturen aufbrechen.** Keine binären Schein-Gegensätze („Nicht X, sondern Y“), keine Negationsketten, keine theatralischen Ein-Wort-Sätze, keine rhetorischen Scheinfragen. Siehe [references/structures.md](references/structures.md).

3. **Nominalstil und Amtsdeutsch abbauen.** Verben statt Substantiv-Monster. Keine Ketten aus *-ung*, *-keit*, *-heit* oder *-tion*, keine trägen Funktionsverbgefüge (*„zur Anwendung bringen“* → anwenden). Schreibe, wer was tut, statt Tätigkeiten zu Substantiven erstarren zu lassen.

4. **Aktiv formulieren und Handelnde benennen.** Jede Aussage braucht ein echtes Subjekt. Vermeide unpersönliche Passiv-Konstruktionen (*„Es wird empfohlen…“*, *„Hierbei lässt sich feststellen…“*). Keine leblose Pseudo-Handlung (False Agency: *„Die Entscheidung reift heran“* – jemand entscheidet!).

5. **Konkret statt schwammig sein.** Keine vagen Behauptungen (*„Die Auswirkungen sind immens“*). Nenne Zahlen, Fakten oder konkrete Beispiele. Keine faulen Extreme (*„jeder“*, *„immer“*, *„nie“*).

6. **Lesende direkt ansprechen und Anredeform strikt beibehalten.** Kein distanzierter Dozenten-Tonfall. Konkrete Situationen schlagen Abstraktionen. Sprich dein Gegenüber an, statt von *„den Menschen“* oder unpersönlich von *„man“* zu fabulieren.
   * **Eiserne Regel für die deutsche Anrede:** Ändere niemals eigenmächtig die vorgegebene Form! Behalte die ursprüngliche Form des Ausgangstextes strikt bei und ziehe sie im gesamten Text lückenlos durch:
     - Kleingeschriebenes **„du“** (*du, dir, dich, dein*) – modern, direkt, nahbar.
     - Großgeschriebenes **„Du“** (*Du, Dir, Dich, Dein*) – persönlich, traditionell.
     - Förmliches **„Sie“** (*Sie, Ihnen, Ihr*) – professionell, distanziert.
   * Niemals zwischen verschiedenen Formen springen, niemals ein *„du“* in ein *„Sie“* (oder umgekehrt) umwandeln.

7. **Rhythmus und Architektur variieren.** Satzlängen aktiv mischen. Zwei präzise Begriffe genügen oft, es muss nicht immer die typische KI-Dreierreihe sein. Absätze unterschiedlich lang gestalten und nicht jeden Text in Bullet-Point-Listen zerhacken. Gedankenstriche (*Em-Dashes*) streichen oder durch Kommas/Punkte ersetzen.

8. **Den Lesenden vertrauen.** Sprich Tatsachen direkt aus. Kein Händchenhalten, keine vorsorglichen Entschuldigungen (*„Und das ist völlig okay“*), kein formelhaftes Fazit (*„Zusammenfassend lässt sich sagen…“*) und keine Kalenderspruch-Pointe am Ende.

## Schnell-Check vor Textabgabe

Vor dem Veröffentlichen prüfen:

- [ ] **Wurde die Anredeform strikt beibehalten?** (*„du“* vs. *„Du“* vs. *„Sie“*) → Ursprüngliche Form niemals ändern, lückenlos durchziehen.
- [ ] **Gibt es Füll-Adverbien oder Weichmacher?** (*wirklich, einfach, buchstäblich, tatsächlich, quasi, durchaus, gewissermaßen*) → Streichen.
- [ ] **Stecken KI-Schmuckwörter oder Metaphern im Text?** (*Herzstück, Wandteppich, Katalysator, Paradigmenwechsel, Leuchtturm, transformative Reise*) → Durch konkrete Begriffe ersetzen.
- [ ] **Kleben Scharnier-Floskeln an Satzanfängen?** (*„Darüber hinaus…“*, *„Des Weiteren…“*, *„In diesem Zusammenhang…“*) → Streichen.
- [ ] **Steckt ein „Nicht X, sondern Y“-Gegensatz drin?** → Direkt **Y** sagen.
- [ ] **Gibt es Räusper-Floskeln?** (*„Fakt ist:“*, *„Hier ist das Problem:“*, *„Es ist wichtig zu beachten, dass…“*) → Sofort zur Sache kommen.
- [ ] **Ist der Text im Passiv oder „Man“-Modus verfasst?** (*„Es wird beobachtet…“*) → Wer handelt? Zum Subjekt machen.
- [ ] **Handelt ein lebloses Ding wie ein Mensch (False Agency)?** (*„Die Beschwerde wird zur Lösung“*, *„Die Daten sprechen…“*) → Die handelnde Person benennen.
- [ ] **Häufen sich Substantivierungen oder Amtsdeutsch?** (*„Zur Optimierung der Bereitstellung…“*, *„zur Anwendung bringen“*) → In lebendige Verben umwandeln (*„Um schneller bereitzustellen…“*, *„anwenden“*).
- [ ] **Sperrige Partizipien vor Substantiven?** (*„die durch X hervorgerufenen Veränderungen“*) → In Nebensatz oder zwei Hauptsätze auflösen.
- [ ] **Wurde Fließtext unnötig in Listen oder Dreierreihen zerhackt?** → Natürlich im Fließtext argumentieren.
- [ ] **Drei Sätze hintereinander mit ähnlicher Länge?** → Einen Satz aufbrechen oder kürzen.
- [ ] **Gedankenstriche (— / –) im Text?** → Entfernen. Im Deutschen meist durch Komma oder neuen Satz ersetzbar.
- [ ] **Vage Behauptung?** (*„Die Konsequenzen sind weitreichend“*) → Konkret benennen, was passiert.
- [ ] **Meta-Gequatsche?** (*„Im nächsten Abschnitt schauen wir uns an…“*) → Streichen und direkt zum Thema springen.
- [ ] **Endet der Text mit einem formelhaften Fazit oder Kalenderspruch?** (*„Zusammenfassend lässt sich sagen…“*, *„…kein Sprint, sondern ein Marathon“*) → Streichen, mit konkreter Handlung oder Fakt enden.

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
