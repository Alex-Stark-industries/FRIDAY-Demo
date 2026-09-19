# FRIDAY Demo — Voice Agent

A **free, fully local** AI chatbot and voice assistant for Windows. Type or talk,
and Friday answers in text and speaks back — running **entirely on your own
machine**. No accounts, no API keys, no cloud, no telemetry.

This is a free taste of the larger **Friday** desktop assistant: it keeps just
the **chat** and the **advanced voice mode**, and nothing else.

> Friday talks in **English**.

---

## Download & run

1. Go to the [**Releases**](../../releases) page and download
   `Friday Voice Agent-<version>-win.zip`.
2. Unzip it anywhere.
3. Run **`Friday Voice Agent.exe`**.

> The app isn't code-signed, so Windows SmartScreen may show *"Windows protected
> your PC"* on first launch. Click **More info → Run anyway**. This is normal for
> free, independent apps.

### One-time setup (required)

Friday's "brain" runs locally through **Ollama** — a free local AI engine:

1. Install [Ollama](https://ollama.com).
2. Pull the model once (in a terminal):
   ```
   ollama pull qwen2.5:3b
   ```
3. Make sure Ollama is running, then start Friday.

The first time you use the voice, it downloads its speech models once (a few
hundred MB) and then works offline.

---

## What it does

- **Chat** — type a message and Friday replies, streamed as she "thinks".
- **Advanced voice mode** — a full-screen reactive sphere; hold **Space** or tap
  the mic to talk, and she speaks her answer back.
- **Six voices** — pick the one you like.
- **Sessions** — your past conversations are saved locally.

Everything stays on your machine. The only network use is the one-time model
downloads and your prompts going to Ollama on your own computer.

---

## Requirements

- **Windows 10 / 11**
- **[Ollama](https://ollama.com)** running locally with `qwen2.5:3b` pulled
- A machine with a GPU makes the voice snappy; it still works without one, just
  slower.

---

## License

MIT — free to use. The larger **Friday** product this previews is a separate,
proprietary application.
