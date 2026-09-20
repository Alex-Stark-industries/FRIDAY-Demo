# Willkommen bei Friday 👋

🌐 [English](WELCOME.md) · [Italiano](WELCOME.it.md) · [Español](WELCOME.es.md) · [Français](WELCOME.fr.md) · **Deutsch** · [Português](WELCOME.pt.md) · [हिन्दी](WELCOME.hi.md)

Diese Anleitung bringt dich von null bis zum Gespräch mit Friday, ohne **irgend­
etwas** vorauszusetzen. Wenn du eine Datei herunterladen kannst, kannst du Friday
starten.

Friday ist ein kostenloser KI-Assistent, der auf **deinem eigenen Computer**
läuft. Du kannst ihm **schreiben** oder mit ihm **sprechen**, und er antwortet —
als Text und laut. Kein Konto, keine Anmeldung, kein kostenpflichtiges Abo. Friday
antwortet auf **Englisch**.

---

## Was du brauchst

- Einen PC mit **Windows 10 oder 11** (64-Bit).
- **8 GB RAM** oder mehr (16 GB sind angenehm). Friday führt die KI auf deiner
  eigenen Maschine aus, daher zählt der Arbeitsspeicher.
- Etwa **4 GB freien Speicherplatz** insgesamt: die App selbst (~0,5 GB), das
  KI-Modell, das du einmal herunterlädst (~2 GB), und die Sprachmodelle, die beim
  ersten Sprach-Einsatz geladen werden (~0,5 GB).
- Eine Internetverbindung **nur für die Einrichtung** — danach laufen Chat und
  Stimme offline.

Eine Grafikkarte (GPU) mit **WebGPU**-Unterstützung (jede aktuelle NVIDIA-, AMD-
oder Intel-GPU) macht die Stimme schnell — aber Friday funktioniert auch ohne, nur
langsamer. Auf einem schwächeren PC läuft trotzdem alles; Antworten und Stimme
dauern nur etwas länger.

> Du kennst die Daten deines PCs nicht? Drücke die **Windows-Taste**, tippe
> **„Info über deinen PC“** und öffne es — dort stehen Windows-Version, Prozessor
> und installierter RAM.

---

## Schritt 1 — Ollama installieren (Fridays Gehirn)

Friday denkt mithilfe einer kostenlosen lokalen KI-Engine namens **Ollama**. Du
installierst sie einmalig.

1. Gehe auf **https://ollama.com** und klicke auf **Download**.
2. Starte den heruntergeladenen Installer und folge den Anweisungen. Fertig —
   Ollama läuft nun unauffällig im Hintergrund.
3. Öffne ein Terminal (drücke die **Windows-Taste**, tippe **`cmd`**, drücke
   **Enter**) und füge diese Zeile ein, dann **Enter**:

   ```
   ollama pull qwen2.5:3b
   ```

   Damit wird das von Friday genutzte KI-Modell heruntergeladen (etwa 2 GB). Warte,
   bis es fertig ist — das machst du nur einmal.

> **Woran erkenne ich, dass Ollama läuft?** Suche nach der Installation das
> Ollama-Symbol neben der Uhr in der Taskleiste. Siehst du es nicht, öffne das
> Startmenü und starte **Ollama**.

---

## Schritt 2 — Friday herunterladen

1. Gehe auf die Seite [**Releases**](../../releases/latest).
2. Lade unter der neuesten Version die Datei namens
   **`Friday-Voice-Agent-Setup-<Version>.exe`** herunter.

---

## Schritt 3 — Friday installieren & starten

1. Öffne die gerade heruntergeladene Datei (meist im Ordner **Downloads**).

   **Beim ersten Mal** zeigt Windows eventuell ein blaues Feld mit *„Der Computer
   wurde durch Windows geschützt“*. Das passiert bei allen kostenlosen, nicht
   kostenpflichtig signierten Apps. Klicke einfach auf:

   - **Weitere Informationen**
   - dann **Trotzdem ausführen**

2. Der Installer öffnet sich. Er installiert **nur für dich** und **braucht kein
   Administratorkennwort**. Klicke dich durch **Weiter → Installieren →
   Fertigstellen**. (Unterwegs kannst du „Desktop-Symbol erstellen“ ankreuzen,
   falls du eins möchtest.)
3. Starte **Friday Voice Agent** — über das **Startmenü**, das **Desktop-Symbol**
   oder indem du „Friday Voice Agent starten“ auf dem letzten Installer-Bildschirm
   angehakt lässt.

Friday öffnet sich. Wenn Ollama läuft, steht oben im Fenster **ALL SYSTEMS ONLINE
(LOCAL)**.

> **Zum späteren Deinstallieren:** Öffne die Windows-**Einstellungen → Apps**,
> suche *Friday Voice Agent* und klicke auf **Deinstallieren**.

---

## Schritt 4 — Dein erster Chat

Am unteren Rand des Fensters gibt es ein Feld mit **„Message Friday…“**.

- Klicke hinein, tippe etwas wie *„Hi Friday! What can you do?“* und drücke
  **Enter**.
- Friday antwortet im Bereich Wort für Wort. Ist der Ton an, liest sie die Antwort
  auch laut vor. Klicke unter einer Antwort auf **LISTEN**, um sie erneut zu hören.

---

## Schritt 5 — Mit Friday sprechen (Sprachmodus)

1. Klicke auf die **Mikrofon**-Schaltfläche (unten links am Nachrichtenfeld) oder
   auf die **Voice mode**-Steuerung, um die bildschirmfüllende leuchtende Kugel zu
   öffnen.
2. **Halte die Leertaste gedrückt**, während du sprichst, und lass dann los — oder
   tippe auf das Mikro auf dem Bildschirm.
3. Friday schreibt mit, was du gesagt hast, denkt nach und **antwortet dir laut**.
4. Lieber eine andere Stimme? Nutze die Stimmen-Steuerung im Kopfbereich (oben
   rechts), um aus **sechs Stimmen** zu wählen.
5. Klicke auf **✕ EXIT** (oben rechts), um zum Chat zurückzukehren.

> **Beim ersten Sprach-Einsatz** werden die Sprachmodelle einmalig heruntergeladen
> (ein paar hundert MB). Danach läuft die Stimme vollständig offline.

---

## Tipps & Fehlerbehebung

- **Friday sagt, die Systeme seien offline / der Chat antwortet nicht.** Ollama
  läuft nicht, oder das Modell wurde nicht geladen. Stelle sicher, dass Ollama
  offen ist und du `ollama pull qwen2.5:3b` ausgeführt hast (Schritt 1).
- **Die Stimme hat das falsche Mikrofon gewählt.** Nutze die **MIC**-Schaltfläche
  im Kopfbereich, um einen anderen Eingang zu wählen.
- **Der erste Start wirkt langsam.** Friday wärmt beim Start ihre Sprach-Engine
  auf und lädt die Sprachmodelle beim ersten Sprach-Einsatz. Spätere Starts sind
  schneller.
- **Nichts wird in die Cloud gesendet.** Deine Gespräche und deine Stimme bleiben
  auf deiner Maschine. Die einzige Netznutzung sind die einmaligen Downloads und
  deine Anfragen an Ollama auf deinem eigenen PC.

---

Viel Spaß mit Friday — und wenn dir dieser kostenlose Vorgeschmack gefällt: Er ist
nur ein kleiner Teil des vollständigen Desktop-Assistenten **Friday**.
