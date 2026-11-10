# 🔐 KI-Tresor-Challenge

**Die KI-Hacking-Challenge für Team-Workshops:** Fünf Chatbots bewachen je ein geheimes Codewort,
mit von Level zu Level stärkerer Abwehr. Die Teams knacken sie im eigenen Tempo.
Hinweise gegen Frust sind eingebaut, und wer gar nicht weiterkommt, tippt `!aufgeben`.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MSchenkl/KI-Tresor-Challenge/blob/main/Tresor_Level.ipynb)
· **Startseite:** [mschenkl.github.io/KI-Tresor-Challenge](https://mschenkl.github.io/KI-Tresor-Challenge/)

| | |
|---|---|
| 👥 Teilnehmer | 3–4 Teams à 2–5 Personen |
| ⏱️ Dauer | 90 Minuten |
| 💻 Technik | Google Colab + Gemini-API (kostenloser Key, keine Installation) |
| 🎓 Vorwissen | keins, es wird nur mit dem Bot gechattet |

## 🪜 Die Level

| Level | Bot | Schutz | Punkte |
|---|---|---|---|
| 1 | Plaudertasche | keiner | 1 |
| 2 | Schweigsame | eine Anweisung im Prompt | 2 |
| 3 | Türsteher | eine Regel („nur mit Mitarbeiternummer“) | 3 |
| 4 | Zensor | ein Python-Filter prüft jede Antwort | 3 |
| 5 | Tresorwächter (**Boss**) | alles zusammen, nicht garantiert knackbar | 6 |

Hinweise und falsche Lösungsversuche kosten je 1 Punkt. Befehle im Chat: `!loesung WORT`, `!hinweis`, `!neu`, `!punkte`, `!aufgeben`.

## 🎯 Was man dabei lernt

- **Wie ein Sprachmodell „denkt“:** Ein Systemprompt ist eine Bitte, kein Gesetz.
- **Prompt Injection:** Wie man eine KI mit Worten austrickst und warum das im Job relevant ist.
- **Sicherheit in Schichten:** Prompt, Regel, Filter und deren jeweilige Schwächen.
- **Social Engineering:** Eine KI prüft Berechtigungen nur, wenn sie das auch kann.
- **Grenzen von KI-Sicherheit:** Auch der beste Schutz ist nie perfekt.

## 📦 Inhalt

| Datei | Wofür | Wer |
|---|---|---|
| [`Tresor_Level.ipynb`](Tresor_Level.ipynb) | **Hauptspiel:** 5 Level mit Hinweisen, Punkten und Notausgang | Teams |
| [`praesentation/index.html`](praesentation/index.html) | 15 Folien mit Timer (<kbd>T</kbd>) und Vollbild (<kbd>F</kbd>) | Beamer |
| [`material/api-key-anleitung.md`](material/api-key-anleitung.md) | Schritt für Schritt: eigenen API-Key erstellen und in Colab hinterlegen | Teilnehmende |
| [`material/moderation.md`](material/moderation.md) | Ablauf, Lösungen und Hinweise je Level, Spickzettel, Troubleshooting | Moderator |
| [`material/punktetafel.html`](material/punktetafel.html) | Live-Rangliste für den Beamer | Moderator |
| [`material/punktetabelle.csv`](material/punktetabelle.csv) | Dieselbe Punktetabelle für Excel | Moderator |
| [`Tresor_Bot_einfach.ipynb`](Tresor_Bot_einfach.ipynb) | **Bonus:** selbst einen Bot bauen, nur Systemprompt | schnelle Teams |
| [`Tresor_Bot.ipynb`](Tresor_Bot.ipynb) | **Bonus:** selbst bauen, mit Ausgabefilter und Wächter-KI | schnelle Teams |
| [`Tresor_Bot_Musterloesung.ipynb`](Tresor_Bot_Musterloesung.ipynb) | Alle Schichten voll ausgebaut | Moderator |
| [`material/szenario-karten.html`](material/szenario-karten.html) | Szenarien und Codewort-Zettel für die Bonusrunde | Moderator |

## 🚀 Schnellstart für Moderatoren

1. [Moderationsleitfaden](material/moderation.md) lesen und die Checkliste abarbeiten. Wichtig: **einen API-Key pro Team** aus einem Projekt **ohne Abrechnung**, und das Spiel **einmal selbst durchspielen**.
2. [Präsentation](praesentation/index.html) und [Punktetafel](material/punktetafel.html) auf dem Beamer-Laptop öffnen.
3. Die Teams öffnen das [Level-Notebook in Colab](https://colab.research.google.com/github/MSchenkl/KI-Tresor-Challenge/blob/main/Tresor_Level.ipynb)
   und legen ihren API-Key unter 🔑 *Secrets* als `GOOGLE_API_KEY` an.

## ⏱️ Ablauf

| Zeit | Phase |
|---|---|
| 0:00 | Einstieg: Wie denkt ein Chatbot? Live-Demo |
| 0:10 | Setup: Notebook öffnen, Key eintragen |
| 0:20 | **Level 1–4** im eigenen Tempo (35 Min.) |
| 0:55 | **Boss** (Level 5) und Bonus (15 Min.) |
| 1:10 | Auswertung: Welcher Trick wirkte warum? |
| 1:20 | Lessons Learned, Transfer, Siegerehrung |

## ⚠️ Hinweis zur Technik

Die Level wurden mit einer simulierten API getestet (Spielstand, Punkte, Filter, Befehle), nicht gegen das echte Modell.
Wie leicht oder schwer die Bots nachgeben, hängt vom Gemini-Modell ab und kann sich ändern.
Spielt deshalb vor dem Workshop alle Level einmal selbst durch. Der Leitfaden erklärt, wie man die Prompts anpasst.

## 🔒 Datenschutz

Das Spiel kommt **ohne echte Personendaten** aus: Szenarien und Codewörter sind erfunden.
Bitte keine echten Passwörter, Kundendaten oder internen Informationen in die Prompts schreiben,
denn alle Eingaben gehen an die Gemini-API.

---

Ein Spin-off der [KI-Team-Challenge](https://github.com/MSchenkl/KI-Team-Challenge) · [mschenkl.github.io](https://mschenkl.github.io)
