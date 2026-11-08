# 🔐 KI-Tresor-Challenge

**Die KI-Hacking-Challenge für Team-Workshops:** Jedes Team baut per Vibecoding einen Chatbot,
der in seinem Szenario hilfreich ist und trotzdem sein geheimes Codewort nie verrät.
Danach versuchen die anderen Teams, es ihm zu entlocken.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MSchenkl/KI-Tresor-Challenge/blob/main/Tresor_Bot.ipynb)
· **Startseite:** [mschenkl.github.io/KI-Tresor-Challenge](https://mschenkl.github.io/KI-Tresor-Challenge/)

| | |
|---|---|
| 👥 Teilnehmer | 3–4 Teams à 2–5 Personen |
| ⏱️ Dauer | 90 Minuten |
| 💻 Technik | Google Colab + Gemini-API (kostenloser Key, keine Installation) |
| 🎓 Vorwissen | keins: Fortgeschrittene bekommen Bonusaufgaben |

## 🎯 Was man dabei lernt

- **Wie ein Sprachmodell „denkt“:** Ein Systemprompt ist eine Bitte, kein Gesetz.
- **Prompt Injection:** Wie man eine KI mit Worten austrickst und warum das im Job relevant ist.
- **Sicherheit in Schichten:** Prompt + Python-Filter + Wächter-KI, jeweils mit Stärken und Schwächen.
- **Sicherheit vs. Nützlichkeit:** Ein Bot, der alles ablehnt, ist auch nutzlos.
- **Vibecoding:** In 25 Minuten einen funktionierenden Bot bauen, ohne Python zu können.

## 📦 Inhalt

| Datei | Wofür | Wer |
|---|---|---|
| [`Tresor_Bot.ipynb`](Tresor_Bot.ipynb) | Team-Notebook: Grundgerüst mit schwachem Prompt, Ausgabefilter, Wächter-KI, Chat-Modus, Logbuch | Teams |
| [`Tresor_Bot_Musterloesung.ipynb`](Tresor_Bot_Musterloesung.ipynb) | Alle drei Schichten voll ausgebaut, auch als Boss-Level | Moderator |
| [`praesentation/index.html`](praesentation/index.html) | 15 Folien, mit Timer (<kbd>T</kbd>) und Vollbild (<kbd>F</kbd>) | Beamer |
| [`material/moderation.md`](material/moderation.md) | Ablauf, Regeln, Prüffragen, Angriffs-Spickzettel, Troubleshooting | Moderator |
| [`material/szenario-karten.html`](material/szenario-karten.html) | 6 Szenario-Karten plus zufällige Codewort-Zettel zum Drucken | Moderator |
| [`material/punktetafel.html`](material/punktetafel.html) | Live-Rangliste für den Beamer | Moderator |
| [`material/punktetabelle.csv`](material/punktetabelle.csv) | Dieselbe Punktetabelle für Excel | Moderator |

## 🚀 Schnellstart für Moderatoren

1. [Moderationsleitfaden](material/moderation.md) lesen und die Checkliste abarbeiten, vor allem **einen API-Key pro Team**.
2. [Szenario-Karten](material/szenario-karten.html) drucken. Die Codewörter werden bei jedem Öffnen neu gewürfelt.
3. [Präsentation](praesentation/index.html) und [Punktetafel](material/punktetafel.html) auf dem Beamer-Laptop öffnen.
4. Die Teams öffnen das [Team-Notebook in Colab](https://colab.research.google.com/github/MSchenkl/KI-Tresor-Challenge/blob/main/Tresor_Bot.ipynb)
   und legen ihren API-Key unter 🔑 *Secrets* als `GOOGLE_API_KEY` an.

## ⏱️ Ablauf

| Zeit | Phase |
|---|---|
| 0:00 | Einstieg: Wie denkt ein Chatbot? Live-Demo |
| 0:10 | Szenario-Karte und Codewort ziehen |
| 0:15 | **Bauphase** (25 Min.) |
| 0:40 | Nützlichkeits-Check |
| 0:45 | **Angriffsphase** im Ringtausch (20 Min.) |
| 1:05 | Auswertung und Bonus-Abstimmung |
| 1:20 | Lessons Learned und Transfer |

## 🔒 Datenschutz

Das Spiel kommt **ohne echte Personendaten** aus: Szenarien und Codewörter sind erfunden.
Bitte keine echten Passwörter, Kundendaten oder internen Informationen in die Prompts schreiben,
denn alle Eingaben gehen an die Gemini-API.

---

Ein Spin-off der [KI-Team-Challenge](https://github.com/MSchenkl/KI-Team-Challenge) · [mschenkl.github.io](https://mschenkl.github.io)
