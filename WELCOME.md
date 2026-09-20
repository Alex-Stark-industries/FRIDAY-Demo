# Welcome to Friday 👋

This guide gets you from zero to talking with Friday, assuming **nothing**. If
you can download a file and unzip it, you can run Friday.

Friday is a free AI assistant that runs on **your own computer**. You can **type**
to it or **talk** to it, and it answers back — in text and out loud. It needs no
account, no sign-up, and no paid subscription. Friday replies in **English**.

---

## What you need

- A **Windows 10 or 11** PC.
- About **1 GB** of free disk space (a few hundred MB more the first time you use
  the voice).
- An internet connection **for setup only** — once it's set up, the chat and
  voice run offline.

A graphics card (GPU) makes the voice faster, but Friday works without one too.

---

## Step 1 — Install Ollama (Friday's brain)

Friday thinks using a free local AI engine called **Ollama**. You install it once.

1. Go to **https://ollama.com** and click **Download**.
2. Run the installer you downloaded and follow the prompts. That's it — Ollama
   now runs quietly in the background.
3. Open a terminal (press the **Windows key**, type **`cmd`**, press **Enter**)
   and paste this line, then press **Enter**:

   ```
   ollama pull qwen2.5:3b
   ```

   This downloads the AI model Friday uses (about 2 GB). Wait for it to finish —
   you only ever do this once.

> **How do I know Ollama is running?** After installing, look for the Ollama icon
> near the clock in your taskbar. If you don't see it, open the Start menu and
> launch **Ollama**.

---

## Step 2 — Download Friday

1. Go to the [**Releases**](../../releases/latest) page.
2. Under the latest release, download the file named
   **`Friday.Voice.Agent-<version>-win.zip`**.
3. Find the downloaded `.zip` (usually in your **Downloads** folder),
   **right-click it → Extract All… → Extract**. This unzips it into a folder.

> There is **no setup wizard** to click through — Friday is a portable app. The
> folder you just unzipped *is* the app.

---

## Step 3 — Run Friday

1. Open the unzipped folder.
2. Double-click **`Friday Voice Agent.exe`**.

**The first time**, Windows may show a blue box that says *"Windows protected
your PC"*. This happens with all free apps that aren't paid-signed. Just click:

- **More info**
- then **Run anyway**

Friday opens. If Ollama is running, the top of the window says **ALL SYSTEMS
ONLINE (LOCAL)**.

---

## Step 4 — Your first chat

At the bottom of the window there's a box that says **"Message Friday…"**.

- Click it, type something like *"Hi Friday! What can you do?"*, and press
  **Enter**.
- Friday replies in the panel, word by word. If the speaker is on, she also reads
  it aloud. Click **LISTEN** under any reply to hear it again.

---

## Step 5 — Talk to Friday (voice mode)

1. Click the **microphone** button (bottom-left of the message box), or the
   **Voice mode** control, to open the full-screen glowing sphere.
2. **Hold the Space bar** while you speak, then let go — or tap the mic on screen.
3. Friday transcribes what you said, thinks, and **speaks the answer back**.
4. Prefer a different voice? Use the voice control in the header (top-right) to
   pick from **six voices**.
5. Click **✕ EXIT** (top-right) to return to the chat.

> **First voice use** downloads the speech models once (a few hundred MB). After
> that, the voice works fully offline.

---

## Tips & troubleshooting

- **Friday says systems are offline / chat doesn't answer.** Ollama isn't
  running, or the model isn't pulled. Make sure Ollama is open, and that you ran
  `ollama pull qwen2.5:3b` (Step 1).
- **The voice picked the wrong microphone.** Use the **MIC** button in the header
  to choose a different input.
- **The first launch feels slow.** Friday warms up its voice engine when it
  starts, and downloads the speech models on first voice use. Later launches are
  faster.
- **Nothing is sent to the cloud.** Your conversations and voice stay on your
  machine. The only network use is the one-time downloads and your prompts going
  to Ollama on your own PC.

---

Enjoy Friday — and if you like this free taste, it's a small slice of the full
**Friday** desktop assistant.
