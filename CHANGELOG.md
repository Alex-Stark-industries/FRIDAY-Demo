# Changelog

## 2.0.1

- Now distributed as a proper **Windows installer** (`Friday-Voice-Agent-Setup-*.exe`)
  instead of a zip — installs per-user with no administrator rights, and adds
  Start-menu and optional desktop shortcuts.
- **Faster startup**: the speech-to-text engine now warms up only when you open
  voice mode, so the app no longer pauses on the heavy model at launch.

## 2.0.0

The free demo grows from a single-screen voice loop into a full **chatbot +
advanced voice** desktop app, with the Friday interface.

- **Chat** with the local model, streamed as she replies.
- **Advanced voice mode** — reactive sphere, hold-Space or tap-to-talk, with
  neural turn detection and barge-in.
- **Six on-device voices**, saved sessions, and a microphone picker.
- **Fully offline voice**: the speech model and runtime are bundled.
- Replies always come back in **English**.
- Distributed as a portable Windows app — unzip and run, no installer needed.

Requires [Ollama](https://ollama.com) running locally with `qwen2.5:3b`.

## 1.0.0

- Initial in-browser voice-loop demo.
