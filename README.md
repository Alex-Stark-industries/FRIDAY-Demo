# FRIDAY Demo — a free, local-first chatbot & voice agent

[![Download](https://img.shields.io/badge/Download-Latest%20Release-e91e63?logo=github)](../../releases/latest)
[![License](https://img.shields.io/badge/License-MIT-2ea44f)](LICENSE)
[![Platform](https://img.shields.io/badge/Windows-10%20%2F%2011-0078D6?logo=windows)](../../releases/latest)

**A free AI chatbot and voice assistant that runs entirely on your own computer.**
Type or talk — Friday answers in text and speaks back, in a voice you pick —
with **no account, no API key, no subscription, no cloud, and no telemetry.**
Nothing you say is sent to any server; the model runs locally through
[Ollama](https://ollama.com), and the voice runs on-device.

> **Local. Private. Free.** Download the installer, run it, and start talking.
> Friday replies in **English**.

This is a free taste of the larger **Friday** desktop assistant. It keeps just
two things — the **chat** and the **advanced voice mode** — and nothing else.

---

### Highlights

- 💬 **Chat** — a local language model via [Ollama](https://ollama.com), streamed word by word as she replies.
- 🎙️ **Advanced voice mode** — a full-screen, hands-free particle sphere with neural turn detection. Hold **Space** or tap the mic; she listens, thinks, and speaks the answer back.
- 🔊 **Six on-device voices** — pick the one you like in the header. Audio never leaves your machine.
- 💾 **Saved sessions** — your past conversations are kept locally and reloadable.
- 🌐 **Fully offline voice** — the speech engine (Kokoro) and runtime are bundled; only the one-time speech-model download and your prompts to your own Ollama ever touch the network.
- 🇬🇧 **Always English** — whatever you type or say, Friday answers in English.

---

### Screenshots

<table>
<tr>
<td width="50%">

**Chat** — the neural core, live diagnostics, and a streamed conversation with the local model.
<img src="docs/screenshots/chat.png" alt="Friday Demo chat interface" width="100%">

</td>
<td width="50%">

**Advanced voice mode** — a full-screen reactive sphere with neural mic detection; hold Space or tap to talk.
<img src="docs/screenshots/voice.png" alt="Friday Demo advanced voice mode" width="100%">

</td>
</tr>
</table>

---

### Download & install

1. Open the [**Releases**](../../releases/latest) page and download
   `Friday-Voice-Agent-Setup-<version>.exe`.
2. Run it. The installer is **per-user** — it needs **no administrator rights**.
3. Launch **Friday Voice Agent** from the Start menu (or the desktop shortcut, if
   you asked for one).

> **First launch:** the installer isn't code-signed, so Windows SmartScreen may
> show *"Windows protected your PC"*. Click **More info → Run anyway**. This is
> normal for free, independent apps.

New here? The [**Welcome & Setup guide**](WELCOME.md) walks you through every step
with nothing assumed.

### One-time setup (required)

Friday's "brain" runs locally through **Ollama**, a free local AI engine:

1. Install [Ollama](https://ollama.com).
2. Pull the model once, in a terminal:
   ```
   ollama pull qwen2.5:3b
   ```
3. Make sure Ollama is running, then start Friday.

The first time you open the voice, it downloads its speech models once (a few
hundred MB) and then works offline forever.

---

### Documentation

| Document | What it covers |
|---|---|
| [Welcome & Setup](WELCOME.md) | Beginner, step-by-step: install, run, first chat, first voice |
| [Changelog](CHANGELOG.md) | What changed in each version |
| [License](LICENSE) | MIT — free to use |

---

### System requirements

Friday runs the AI model and the voice **on your own machine**, so what you get
depends on your PC. These are realistic minimums for the bundled `qwen2.5:3b`
model.

| | Minimum | Recommended |
|---|---|---|
| **OS** | Windows 10 / 11, 64-bit | Windows 11, 64-bit |
| **CPU** | Any modern 64-bit (x64) processor | Recent multi-core CPU |
| **RAM** | 8 GB | 16 GB |
| **Free disk** | ~4 GB (app ≈0.5 GB · model ≈2 GB · speech models ≈0.5 GB) | 6 GB+ |
| **GPU** | None — runs on CPU (voice is slower) | A GPU with **WebGPU** support (recent NVIDIA / AMD / Intel) for snappy voice |
| **Internet** | For one-time setup only (Ollama, model, first-voice download) | — |

- **[Ollama](https://ollama.com)** must be running locally with `qwen2.5:3b`
  pulled (`ollama pull qwen2.5:3b`).
- Everything else — chat and voice — runs offline once set up.
- With less RAM or no GPU, Friday still works; replies and speech just take
  longer.

---

### Privacy at a glance

- **No accounts, no API keys, no telemetry, no analytics, no auto-update.**
- The language model runs on **your own machine** through Ollama.
- The voice (speech-to-text and text-to-speech) runs **on-device**.
- The only network use is the one-time speech-model download and your own
  prompts going to Ollama on your own computer.

---

### License

MIT — free to use. See [LICENSE](LICENSE). The larger **Friday** product this
previews is a separate, proprietary application.
