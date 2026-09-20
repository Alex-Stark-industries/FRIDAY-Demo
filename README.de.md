# FRIDAY Demo — ein kostenloser, lokaler Chatbot & Sprachassistent

🌐 [English](README.md) · [Italiano](README.it.md) · [Español](README.es.md) · [Français](README.fr.md) · **Deutsch** · [Português](README.pt.md) · [हिन्दी](README.hi.md)

[![Download](https://img.shields.io/badge/Download-Neueste%20Version-e91e63?logo=github)](../../releases/latest)
[![Lizenz](https://img.shields.io/badge/Lizenz-MIT-2ea44f)](LICENSE)
[![Plattform](https://img.shields.io/badge/Windows-10%20%2F%2011-0078D6?logo=windows)](../../releases/latest)

**Ein kostenloser KI-Chatbot und Sprachassistent, der vollständig auf deinem
eigenen Computer läuft.** Tippen oder sprechen — Friday antwortet als Text und
spricht mit einer Stimme, die du wählst — **ohne Konto, ohne API-Schlüssel, ohne
Abo, ohne Cloud und ohne Telemetrie.** Nichts, was du sagst, wird an einen Server
gesendet: Das Modell läuft lokal über [Ollama](https://ollama.com), und die
Stimme läuft auf dem Gerät.

> **Lokal. Privat. Kostenlos.** Installer herunterladen, starten und losreden.
> Friday antwortet auf **Englisch**.

Dies ist ein kostenloser Vorgeschmack auf den umfangreicheren Desktop-Assistenten
**Friday**. Er behält nur zwei Dinge — den **Chat** und den **erweiterten
Sprachmodus** — und sonst nichts.

---

### Auf einen Blick

- 💬 **Chat** — ein lokales Sprachmodell über [Ollama](https://ollama.com), die Antwort erscheint Wort für Wort.
- 🎙️ **Erweiterter Sprachmodus** — eine bildschirmfüllende Partikelkugel, freihändig, mit neuronaler Sprech-Erkennung. Halte **Leertaste** gedrückt oder tippe aufs Mikro; sie hört zu, denkt nach und antwortet dir laut.
- 🔊 **Sechs Stimmen auf dem Gerät** — wähle im Kopfbereich die, die dir gefällt. Der Ton verlässt niemals deine Maschine.
- 💾 **Gespeicherte Sitzungen** — frühere Gespräche bleiben lokal und lassen sich wieder laden.
- 🌐 **Voll offline-fähige Stimme** — die Sprach-Engine (Kokoro) und die Laufzeit sind enthalten; nur der einmalige Download der Sprachmodelle und deine Anfragen an dein eigenes Ollama gehen über das Netz.
- 🇬🇧 **Immer Englisch** — egal, was du tippst oder sagst, Friday antwortet auf Englisch.

---

### Screenshots

<table>
<tr>
<td width="50%">

**Chat** — der neuronale Kern, Live-Diagnosen und ein gestreamtes Gespräch mit dem lokalen Modell.
<img src="docs/screenshots/chat.png" alt="Chat-Oberfläche von Friday Demo" width="100%">

</td>
<td width="50%">

**Erweiterter Sprachmodus** — eine bildschirmfüllende, reaktive Kugel mit neuronaler Mikro-Erkennung; Leertaste halten oder tippen zum Sprechen.
<img src="docs/screenshots/voice.png" alt="Erweiterter Sprachmodus von Friday Demo" width="100%">

</td>
</tr>
</table>

---

### Download & Installation

1. Öffne die Seite [**Releases**](../../releases/latest) und lade
   `Friday-Voice-Agent-Setup-<Version>.exe` herunter.
2. Führe sie aus. Der Installer ist **pro Benutzer** — er **braucht keine
   Administratorrechte**.
3. Starte **Friday Voice Agent** über das Startmenü (oder die
   Desktop-Verknüpfung, falls angefordert).

> **Erster Start:** Der Installer ist nicht signiert, daher zeigt Windows
> SmartScreen eventuell *„Der Computer wurde durch Windows geschützt“*. Klicke auf
> **Weitere Informationen → Trotzdem ausführen**. Das ist bei kostenlosen,
> unabhängigen Apps normal.

Neu hier? Die [**Willkommens- und Einrichtungsanleitung**](WELCOME.de.md) führt
dich Schritt für Schritt, ohne etwas vorauszusetzen.

### Einmalige Einrichtung (erforderlich)

Das „Gehirn“ von Friday läuft lokal über **Ollama**, eine kostenlose lokale
KI-Engine:

1. Installiere [Ollama](https://ollama.com).
2. Lade das Modell einmalig in einem Terminal:
   ```
   ollama pull qwen2.5:3b
   ```
3. Stelle sicher, dass Ollama läuft, und starte dann Friday.

Beim ersten Öffnen der Stimme werden die Sprachmodelle einmalig heruntergeladen
(ein paar hundert MB); danach läuft alles für immer offline.

---

### Dokumentation

| Dokument | Inhalt |
|---|---|
| [Willkommen & Einrichtung](WELCOME.de.md) | Für Einsteiger, Schritt für Schritt: installieren, starten, erster Chat, erste Stimme |
| [Changelog](CHANGELOG.md) | Was sich in jeder Version geändert hat (auf Englisch) |
| [Lizenz](LICENSE) | MIT — freie Nutzung |

---

### Systemanforderungen

Friday führt das KI-Modell und die Stimme **auf deiner eigenen Maschine** aus, das
Ergebnis hängt also von deinem PC ab. Dies sind realistische Mindestwerte für das
enthaltene Modell `qwen2.5:3b`.

| | Minimum | Empfohlen |
|---|---|---|
| **Betriebssystem** | Windows 10 / 11, 64-Bit | Windows 11, 64-Bit |
| **CPU** | Jeder moderne 64-Bit-Prozessor (x64) | Aktuelle Mehrkern-CPU |
| **RAM** | 8 GB | 16 GB |
| **Freier Speicher** | ~4 GB (App ≈0,5 GB · Modell ≈2 GB · Sprachmodelle ≈0,5 GB) | 6 GB+ |
| **GPU** | Keine — läuft auf der CPU (Stimme langsamer) | Eine GPU mit **WebGPU**-Unterstützung (aktuelle NVIDIA / AMD / Intel) für eine flotte Stimme |
| **Internet** | Nur für die einmalige Einrichtung (Ollama, Modell, erster Stimmen-Download) | — |

- **[Ollama](https://ollama.com)** muss lokal laufen, mit heruntergeladenem
  `qwen2.5:3b` (`ollama pull qwen2.5:3b`).
- Alles andere — Chat und Stimme — läuft nach der Einrichtung offline.
- Mit weniger RAM oder ohne GPU funktioniert Friday trotzdem; Antworten und
  Stimme dauern nur länger.

---

### Datenschutz auf einen Blick

- **Keine Konten, keine API-Schlüssel, keine Telemetrie, keine Analyse, keine
  automatischen Updates.**
- Das Sprachmodell läuft **auf deiner eigenen Maschine** über Ollama.
- Die Stimme (Spracherkennung und Sprachausgabe) läuft **auf dem Gerät**.
- Die einzige Netznutzung ist der einmalige Download der Sprachmodelle und deine
  eigenen Anfragen an Ollama auf deinem eigenen Computer.

---

### Lizenz

MIT — freie Nutzung. Siehe [LICENSE](LICENSE). Das vollständige Produkt
**Friday**, das hier in der Vorschau gezeigt wird, ist eine separate, proprietäre
Anwendung.
