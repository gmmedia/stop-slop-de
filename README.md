# Stop Slop (DE) 🇩🇪

**Ein KI-Skill und Regelwerk, um deutsche Texte von typischen KI-Schreibmustern, leeren Floskeln und künstlichem Tonfall zu befreien.**

Basierend auf dem englischen Original [stop-slop](https://github.com/hardikpandya/stop-slop) von [Hardik Pandya](https://hvpandya.com), von Grund auf adaptiert und erweitert für die Besonderheiten der deutschen Sprache.

---

## Warum eine deutsche Version?

KI-generiertes Deutsch leidet unter ganz spezifischen Problemen, die englische Prompts nicht abfangen:

1. **Räusper-Floskeln:** *„In der heutigen, schnelllebigen Welt…“*, *„Fakt ist:“*, *„Es ist wichtig zu beachten, dass…“*
2. **Hölzern übersetzter Business-Jargon:** *„Tief in Daten eintauchen“* (dive into), *„Herausforderungen navigieren“* (navigate), *„die Marktlandschaft“* (landscape).
3. **Extremer Nominalstil & Passiv:** Sätze ersticken in Substantiven (*-ung, -heit, -keit*) und unpersönlichen Floskeln (*„Hierbei lässt sich feststellen…“*), statt aktiv zu sagen, wer was tut.
4. **Künstliche Dramatik:** *„Nicht X, sondern Y“*-Gegensätze, pseudo-tiefe Staccato-Sätze (*„Punkt.“*, *„Lass das sacken.“*) und ständige Gedankenstriche (`—`).

`stop-slop-de` trainiert Sprachmodelle darauf, diese Muster zu erkennen, radikal zu kürzen und menschlich, präzise und direkt zu formulieren.

---

## Aufbau des Repositories

```
stop-slop-de/
├── SKILL.md              # Die 8 Kernregeln & Checkliste für KI-Agenten
├── references/
│   ├── phrases.md        # Verbotene Phrasen, Füllwörter & deutsche KI-Floskeln
│   ├── structures.md     # Zu vermeidende Satzmuster, Nominalstil & Passiv-Regeln
│   └── examples.md       # Vorher-/Nachher-Beispiele aus der Praxis
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

* **Räusper-Einstiege:** Keine Ankündigungen vor der eigentlichen Aussage. Sofort zur Sache kommen.
* **Formelhafte Kontraste:** Keine *„Nicht X, sondern Y“*-Scheingegensätze. Direkt die Kernaussage treffen.
* **Nominalstil:** Verben statt Substantiv-Monster (*„Wir optimieren…“* statt *„Zur Durchführung der Optimierung…“*).
* **Falsche Handlungsfähigkeit (False Agency):** Menschen benennen, die handeln – keine handelnden Abstraktionen (*„Die Daten zeigen…“*).
* **Füll-Adverbien & Weichspüler:** Streichen von *wirklich, einfach, tatsächlich, quasi, sozusagen, essenziell*.
* **Em-Dash-Inflation:** Gedankenstriche im Fließtext durch klare Punkte oder Kommas ersetzen.

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
