# 🔑 API-Key einrichten (für Teilnehmende)

Für den Workshop braucht jede Gruppe einen **eigenen** kostenlosen Gemini-API-Key.
Bitte **vor dem Workshop** einrichten und einmal testen.

**Jede Gruppe braucht ihren eigenen Gemini-API-Key.** Das kostenlose Minutenlimit gilt pro Google-Projekt:
Teilen sich mehrere Gruppen einen Key, bremsen sie sich gegenseitig aus (Fehler 429).

## 🔑 Neuen Key erstellen (ca. 2 Minuten)

1. [aistudio.google.com/apikey](https://aistudio.google.com/apikey) öffnen und mit einem Google-Konto anmelden.
2. Auf **„API-Schlüssel erstellen“** (*Create API key*) klicken.
3. Als Projekt **ein neues Projekt** wählen. Kein bestehendes Projekt mit Abrechnung verwenden und **keine Abrechnung einrichten**, sonst kommt später Fehler 402 („Guthaben leer“).
4. Den Key mit dem Kopieren-Symbol kopieren. **Nicht teilen, nicht fotografieren, nicht in Chats posten.**

## 📥 Key in Colab hinterlegen

1. Links in Colab auf das **🔑-Symbol (Secrets)** klicken.
2. **„Neues Secret hinzufügen“**: Name genau `GOOGLE_API_KEY`, Wert = der kopierte Key.
3. Den Schalter **Notebook-Zugriff** einschalten.
4. Die Setup-Zelle unten ausführen. Erwartet: `Verbindung steht ✅`.

## 🛟 Wenn es nicht klappt

| Meldung | Lösung |
|---|---|
| „Kein Secret GOOGLE_API_KEY gefunden“ | Name genau `GOOGLE_API_KEY`? *Notebook-Zugriff* eingeschaltet? |
| 402 / „prepayment credits are depleted“ | Key stammt aus einem Projekt mit Abrechnung. Neuen Key in einem **neuen Projekt ohne Abrechnung** anlegen. |
| 429 / „Zu viele Anfragen“ | Minutenlimit erreicht. Kurz warten, das Notebook versucht es selbst erneut. |
| 503 / 504 | Google ist ausgelastet. 1–2 Minuten warten. |

Nach dem Workshop den Key in AI Studio wieder **löschen**.

---

Zurück zur [Startseite](../README.md) · [Level-Notebook in Colab](https://colab.research.google.com/github/MSchenkl/KI-Tresor-Challenge/blob/main/Tresor_Level.ipynb)
