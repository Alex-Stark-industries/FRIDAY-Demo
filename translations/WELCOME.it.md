# Benvenuto in Friday 👋

🌐 [English](../WELCOME.md) · **Italiano** · [Español](WELCOME.es.md) · [Français](WELCOME.fr.md) · [Deutsch](WELCOME.de.md) · [Português](WELCOME.pt.md) · [हिन्दी](WELCOME.hi.md)

Questa guida ti porta da zero a parlare con Friday, senza dare **nulla** per
scontato. Se sai scaricare un file, sai avviare Friday.

Friday è un assistente AI gratuito che gira sul **tuo computer**. Puoi
**scrivergli** o **parlargli**, e lui risponde — per iscritto e a voce. Non serve
alcun account, nessuna registrazione e nessun abbonamento a pagamento. Friday
risponde in **inglese**.

---

## Cosa ti serve

- Un PC con **Windows 10 o 11** (64 bit).
- **8 GB di RAM** o più (16 GB sono comodi). Friday esegue l'AI sulla tua
  macchina, quindi la memoria conta.
- Circa **4 GB di spazio libero** su disco in totale: l'app stessa (~0,5 GB), il
  modello AI che scarichi una volta (~2 GB) e i modelli vocali scaricati al primo
  uso della voce (~0,5 GB).
- Una connessione internet **solo per la configurazione** — una volta impostato,
  chat e voce funzionano offline.

Una scheda grafica (GPU) con supporto **WebGPU** (qualsiasi GPU NVIDIA, AMD o
Intel recente) rende la voce veloce — ma Friday funziona anche senza, solo più
lentamente. Su un PC meno potente funziona tutto lo stesso; risposte e voce
richiedono solo un po' più di tempo.

> Non sei sicuro delle caratteristiche del tuo PC? Premi il **tasto Windows**,
> scrivi **"Informazioni sul PC"** e aprilo — mostra la versione di Windows, il
> processore e la RAM installata.

---

## Passo 1 — Installa Ollama (il cervello di Friday)

Friday ragiona usando un motore AI locale e gratuito chiamato **Ollama**. Lo
installi una volta sola.

1. Vai su **https://ollama.com** e clicca **Download**.
2. Avvia l'installer scaricato e segui le istruzioni. Fatto — ora Ollama gira in
   silenzio in background.
3. Apri un terminale (premi il **tasto Windows**, scrivi **`cmd`**, premi
   **Invio**) e incolla questa riga, poi premi **Invio**:

   ```
   ollama pull qwen2.5:3b
   ```

   Questo scarica il modello AI che usa Friday (circa 2 GB). Aspetta che finisca —
   lo fai una volta sola.

> **Come faccio a sapere se Ollama è in esecuzione?** Dopo l'installazione, cerca
> l'icona di Ollama vicino all'orologio nella barra delle applicazioni. Se non la
> vedi, apri il menu Start e avvia **Ollama**.

---

## Passo 2 — Scarica Friday

1. Vai alla pagina [**Releases**](https://github.com/Alex-Stark-industries/FRIDAY-Demo/releases/latest).
2. Sotto l'ultima release, scarica il file chiamato
   **`Friday-Voice-Agent-Setup-<versione>.exe`**.

---

## Passo 3 — Installa e avvia Friday

1. Apri il file appena scaricato (di solito nella cartella **Download**).

   **La prima volta**, Windows potrebbe mostrare un riquadro blu che dice
   *"Windows ha protetto il PC"*. Succede con tutte le app gratuite senza firma a
   pagamento. Clicca semplicemente:

   - **Ulteriori informazioni**
   - poi **Esegui comunque**

2. Si apre l'installer. Installa **solo per te** e **non serve la password di
   amministratore**. Clicca **Avanti → Installa → Fine**. (Se vuoi, puoi spuntare
   "Crea un'icona sul desktop" lungo il percorso.)
3. Avvia **Friday Voice Agent** — dal **menu Start**, dall'**icona sul desktop**,
   oppure lasciando spuntato "Avvia Friday Voice Agent" nell'ultima schermata
   dell'installer.

Friday si apre. Se Ollama è in esecuzione, in alto nella finestra compare **ALL
SYSTEMS ONLINE (LOCAL)**.

> **Per disinstallare in seguito:** apri **Impostazioni → App** di Windows, cerca
> *Friday Voice Agent* e clicca **Disinstalla**.

---

## Passo 4 — La tua prima chat

In fondo alla finestra c'è una casella che dice **"Message Friday…"**.

- Cliccala, scrivi qualcosa come *"Hi Friday! What can you do?"* e premi
  **Invio**.
- Friday risponde nel pannello, parola per parola. Se l'audio è attivo, legge
  anche la risposta ad alta voce. Clicca **LISTEN** sotto una risposta per
  riascoltarla.

---

## Passo 5 — Parla con Friday (modalità vocale)

1. Clicca il pulsante del **microfono** (in basso a sinistra della casella
   messaggi), o il comando **Voice mode**, per aprire la sfera luminosa a schermo
   intero.
2. **Tieni premuta la barra spaziatrice** mentre parli, poi rilasciala — oppure
   tocca il microfono sullo schermo.
3. Friday trascrive quello che hai detto, ragiona e **ti risponde a voce**.
4. Preferisci una voce diversa? Usa il comando delle voci nell'intestazione (in
   alto a destra) per scegliere tra **sei voci**.
5. Clicca **✕ EXIT** (in alto a destra) per tornare alla chat.

> **Al primo uso della voce** vengono scaricati una volta i modelli vocali
> (qualche centinaio di MB). Dopodiché la voce funziona completamente offline.

---

## Consigli e risoluzione dei problemi

- **Friday dice che i sistemi sono offline / la chat non risponde.** Ollama non è
  in esecuzione, o il modello non è stato scaricato. Assicurati che Ollama sia
  aperto e di aver eseguito `ollama pull qwen2.5:3b` (Passo 1).
- **La voce ha scelto il microfono sbagliato.** Usa il pulsante **MIC**
  nell'intestazione per scegliere un altro ingresso.
- **Il primo avvio sembra lento.** Friday scalda il motore vocale all'avvio e
  scarica i modelli vocali al primo uso della voce. Gli avvii successivi sono più
  veloci.
- **Niente viene inviato al cloud.** Le tue conversazioni e la voce restano sulla
  tua macchina. L'unico utilizzo della rete è il download una tantum e i tuoi
  messaggi che vanno a Ollama sul tuo PC.

---

Buon divertimento con Friday — e se questo assaggio gratuito ti piace, è una
piccola fetta dell'assistente desktop **Friday** completo.
