# Stop Slop (DE) 🇩🇪

**Ein KI-Skill und Regelwerk, um deutsche Texte von typischen KI-Schreibmustern, leeren Floskeln und künstlichem Tonfall zu befreien.**

Basierend auf dem englischen Original [stop-slop](https://github.com/hardikpandya/stop-slop) von [Hardik Pandya](https://hvpandya.com), von Grund auf adaptiert und erweitert für die Besonderheiten der deutschen Sprache.

---

## Die deutsche Besonderheit: Die Anredeformen (*du* / *Du* / *Sie*)

Das Englische kennt im Wesentlichen nur *„you“*. Im Deutschen ist die Wahl der Anrede jedoch die wichtigste stilistische Weichenstellung eines Textes. KI-Modelle versagen hier regelmäßig: Sie wechseln unbemerkt mitten im Text das Register, wandeln vertrauliche Texte in Behördensprache um oder flüchten in unpersönliche *„man“*-Konstruktionen.

`stop-slop-de` verankert hierfür eine **eiserne Grundregel**:

> **Die ursprüngliche Anredeform des Ausgangstextes darf niemals eigenmächtig geändert werden und muss im gesamten Text lückenlos durchgezogen werden.**

### Die drei legitimen Anredeformen:

1. **Modernes, kleingeschriebenes „du“ (*du, dir, dich, dein*):**  
   Standard im modernen Web, in SaaS-Produkten, Startups, Social Media und agilen Teams. Nahbar, direkt und auf Augenhöhe.
2. **Klassisches, großgeschriebenes „Du“ (*Du, Dir, Dich, Dein*):**  
   Traditionelle direkte Leseransprache, häufig im Direktmarketing, in persönlichen Newslettern oder redaktionellen Texten. Wertschätzend und persönlich.
3. **Förmliches „Sie“ (*Sie, Ihnen, Ihr*):**  
   Standard im klassischen B2B, Finanz-, Rechts- oder Behördenumfeld. Professionell, respektvoll und distanziert.

**Verboten:**
- Ein *„du“* eigenmächtig in ein *„Sie“* (oder umgekehrt) umschreiben.
- Schreibweisen innerhalb eines Textes mischen (*„du“* und *„Dir“*).
- Innerhalb von Absätzen zwischen *du*, *wir*, *Sie* und unpersönlichem *man* hin- und herspringen.

---

## Warum eine deutsche Version?

KI-generiertes Deutsch leidet unter ganz spezifischen Problemen, die englische Prompts nicht abfangen:

1. **Anrede-Brüche:** Unkontrolliertes Springen zwischen *du*, *Du*, *Sie* und *man*.
2. **Räusper-Floskeln & Schmuck-Metaphern:** *„In der heutigen, schnelllebigen Welt…“*, *„Fakt ist:“*, *„Das Herzstück…“*, *„Der Katalysator für Innovation…“*, *„Ein bunter Wandteppich aus…“*.
3. **Hölzern übersetzter Business-Jargon:** *„Tief in Daten eintauchen“* (dive into), *„Herausforderungen navigieren“* (navigate), *„die Marktlandschaft“* (landscape), *„nahtlos integrieren“*.
4. **Extremer Nominalstil & Passiv:** Sätze ersticken in Substantiven (*-ung, -heit, -keit*) und bürokratischen Funktionsverben (*„zur Anwendung bringen“*), statt aktiv zu sagen, wer was tut.
5. **Erweiterte Partizipialmonster:** Riesige Einschübe zwischen Artikel und Nomen (*„die durch die Digitalisierung hervorgerufenen Veränderungen…“*).
6. **Künstliche Dramatik & Listenwahn:** *„Nicht X, sondern Y“*-Gegensätze, Gedankenstriche (`—`), monotone 3-Punkte-Listen und Kalenderspruch-Schlüsse (*„Zusammenfassend lässt sich sagen…“*).

`stop-slop-de` trainiert Sprachmodelle darauf, diese Muster zu erkennen, radikal zu kürzen und menschlich, präzise und direkt zu formulieren.

---

## Die 8 Kernregeln im Überblick

| Nr. | Regel | Kernbotschaft |
|:---:|-------|---------------|
| **1** | **Füllwörter & Räuspern streichen** | Keine Anläufe (*„In der heutigen Welt…“*), keine KI-Metaphern (*Herzstück, Wandteppich*), keine Scharnierwörter (*Darüber hinaus*). |
| **2** | **Formelhafte Satzstrukturen aufbrechen** | Keine binären Kontraste (*„Nicht X, sondern Y“*), keine Staccato-Einwortsätze, keine Scheinfragen. |
| **3** | **Nominalstil & Amtsdeutsch abbauen** | Aktive Verben statt Substantiv-Monster (*-ung, -heit, -keit*) und träger Funktionsverben (*„zur Anwendung bringen“*). |
| **4** | **Aktiv formulieren & Handelnde benennen** | Wer tut was? Keine leblose Pseudohandlung (*False Agency*: *„Die Daten sprechen…“*). |
| **5** | **Konkret statt schwammig sein** | Zahlen, Fakten und greifbare Beispiele statt vager Behauptungen (*„immense Auswirkungen“*). |
| **6** | **Lesende direkt ansprechen & Anrede einhalten** | Ursprüngliche Anrede (*du* / *Du* / *Sie*) strikt beibehalten und lückenlos durchziehen. |
| **7** | **Rhythmus & Architektur variieren** | Satzlängen mischen, keine Gedankenstriche (`—`), keine starre Listenmonotonie. |
| **8** | **Den Lesenden vertrauen** | Fakten aussprechen, kein Händchenhalten, keine belehrende Fazit-Moral am Schluss. |

---

## Aufbau des Repositories

```
stop-slop-de/
├── SKILL.md              # Die 8 Kernregeln & 16-Punkte-Checkliste für KI-Agenten
├── references/
│   ├── phrases.md        # Verbotene Phrasen, KI-Schmuckwörter & Füllwortlisten
│   ├── structures.md     # Syntax-Muster, Nominalstil, Partizipien & Anrederegeln
│   └── examples.md       # Vorher-/Nachher-Beispiele aus der echten Praxis
├── README.md
├── CHANGELOG.md
└── LICENSE
```

---

## Schnelleinstieg

### 1. Claude Code / Antigravity / Agent-Tools
Klone dieses Repo oder binde den Ordner als lokalen Skill ein:
```bash
git clone https://github.com/jochen-gererstorfer/stop-slop-de.git
```
In Claude Code oder Antigravity kann der Skill über `SKILL.md` direkt geladen werden.

### 2. Claude Projects / Custom GPTs
Lade die Datei `SKILL.md` sowie die Dateien aus dem Ordner `references/` als Projektwissen / Knowledge hoch.

### 3. Benutzerdefinierte Anweisungen (Custom Instructions)
Kopiere die 8 Kernregeln und die Checkliste aus `SKILL.md` direkt in deine Custom Instructions bei ChatGPT, Claude oder Perplexity.

### 4. System-Prompt / API
Füge den Inhalt von `SKILL.md` in deinen System-Prompt ein. Die Referenzdateien können bei Bedarf punktuell beigezogen werden.

---

## Was dieser Skill eliminiert

* **Anrede-Brüche (du / Du / Sie):** Garantiert den strikten Erhalt der vom Verfasser gewählten Anrede und verhindert stilistische Sprünge.
* **Räusper-Einstiege:** Keine Ankündigungen vor der eigentlichen Aussage. Sofort zur Sache kommen.
* **KI-Schmuckwörter & Metaphern:** Streicht *Herzstück*, *Wandteppich*, *Katalysator*, *Paradigmenwechsel*, *Leuchtturm* etc.
* **Formelhafte Kontraste:** Keine *„Nicht X, sondern Y“*-Scheingegensätze. Direkt die Kernaussage treffen.
* **Nominalstil & Bürokratendeutsch:** Verben statt Substantiv-Monster (*„Wir optimieren…“* statt *„Zur Durchführung der Optimierung…“*).
* **Falsche Handlungsfähigkeit (False Agency):** Menschen benennen, die handeln – keine handelnden Abstraktionen (*„Die Daten zeigen…“*).
* **Scharnier-Floskeln:** Streicht mechanische Satzverbinder (*„Darüber hinaus…“*, *„Des Weiteren…“*).
* **Füll-Adverbien & Weichspüler:** Streichen von *wirklich, einfach, tatsächlich, quasi, sozusagen, essenziell, durchaus*.
* **Em-Dash-Inflation:** Gedankenstriche im Fließtext durch klare Punkte oder Kommas ersetzen.
* **Fazit-Slop:** Keine belehrenden Kalendersprüche oder erzwungene Zusammenfassungen am Textende.

---

## Bewertungs-Rubrik (Scoring)

Bewerte jeden Textabschnitt von 1 bis 10 Punkten in folgenden 5 Dimensionen:

| Dimension | Prüffrage |
|-----------|-----------|
| **Direktheit** | Direkte Aussage oder endlose Ankündigung? |
| **Rhythmus** | Lebendig und abwechslungsreich oder monotoner Metronom? |
| **Vertrauen** | Respektiert der Text die Intelligenz der Lesenden? |
| **Authentizität** | Klingt der Text nach einem echten Menschen mit Haltung? |
| **Dichte** | Lässt sich noch ein einziges Wort ohne Sinnverlust streichen? |

> **Score unter 35 / 50 Punkten:** Der Text ist noch zu stark von KI-Mustern geprägt und muss überarbeitet werden.

---

## Beispiele

Ausführliche Vorher-/Nachher-Vergleiche findest du in [`references/examples.md`](references/examples.md).

---

## Danksagung & Credits

Dieses Projekt ist eine deutsche Adaption und Erweiterung von **[stop-slop](https://github.com/hardikpandya/stop-slop)** von [Hardik Pandya](https://hvpandya.com). Danke für die inspirierende Vorlage!

---

## Lizenz

[MIT License](LICENSE) © 2026 Jochen Gererstorfer / Hardik Pandya.  
Frei nutzbar, frei anpassbar, gerne teilen!
