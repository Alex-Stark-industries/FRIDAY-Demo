# FRIDAY Demo — un chatbot e voice agent gratuito, tutto in locale

🌐 [English](../README.md) · **Italiano** · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [Português](README.pt.md) · [हिन्दी](README.hi.md)

[![Download](https://img.shields.io/badge/Download-Ultima%20release-e91e63?logo=github)](https://github.com/Alex-Stark-industries/FRIDAY-Demo/releases/latest)
[![Licenza](https://img.shields.io/badge/Licenza-MIT-2ea44f)](../LICENSE)
[![Piattaforma](https://img.shields.io/badge/Windows-10%20%2F%2011-0078D6?logo=windows)](https://github.com/Alex-Stark-industries/FRIDAY-Demo/releases/latest)

**Un chatbot e assistente vocale con AI, gratuito, che gira interamente sul tuo
computer.** Scrivi o parla — Friday risponde per iscritto e a voce, con una voce
che scegli tu — **senza account, senza API key, senza abbonamento, senza cloud e
senza telemetria.** Niente di quello che dici viene inviato a un server: il
modello gira in locale tramite [Ollama](https://ollama.com), e la voce funziona
sul dispositivo.

> **Locale. Privato. Gratis.** Scarica l'installer, avvialo e comincia a parlare.
> Friday risponde in **inglese**.

Questo è un assaggio gratuito del più ampio assistente desktop **Friday**.
Mantiene solo due cose — la **chat** e la **modalità vocale avanzata** — e
nient'altro.

---

### In sintesi

- 💬 **Chat** — un modello linguistico locale tramite [Ollama](https://ollama.com), con la risposta che compare parola per parola.
- 🎙️ **Modalità vocale avanzata** — una sfera di particelle a schermo intero, a mani libere, con rilevamento neurale del turno di parola. Tieni premuto **Spazio** o tocca il microfono; lei ascolta, ragiona e ti risponde a voce.
- 🔊 **Sei voci sul dispositivo** — scegli quella che preferisci nell'intestazione. L'audio non lascia mai la tua macchina.
- 💾 **Sessioni salvate** — le conversazioni precedenti restano in locale e si possono ricaricare.
- 🌐 **Voce completamente offline** — il motore vocale (Kokoro) e il runtime sono inclusi; solo il download una tantum dei modelli vocali e i tuoi messaggi verso il tuo Ollama passano dalla rete.
- 🇬🇧 **Sempre in inglese** — qualunque cosa scrivi o dici, Friday risponde in inglese.

---

### Screenshot

<table>
<tr>
<td width="50%">

**Chat** — il nucleo neurale, le diagnostiche live e una conversazione in streaming con il modello locale.
<img src="../docs/screenshots/chat.png" alt="Interfaccia chat di Friday Demo" width="100%">

</td>
<td width="50%">

**Modalità vocale avanzata** — una sfera reattiva a schermo intero con rilevamento neurale del microfono; tieni premuto Spazio o tocca per parlare.
<img src="../docs/screenshots/voice.png" alt="Modalità vocale avanzata di Friday Demo" width="100%">

</td>
</tr>
</table>

---

### Download e installazione

1. Apri la pagina [**Releases**](https://github.com/Alex-Stark-industries/FRIDAY-Demo/releases/latest) e scarica
   `Friday-Voice-Agent-Setup-<versione>.exe`.
2. Avvialo. L'installer è **per singolo utente** — **non servono i permessi di
   amministratore**.
3. Avvia **Friday Voice Agent** dal menu Start (o dal collegamento sul desktop,
   se l'hai richiesto).

> **Primo avvio:** l'installer non ha la firma digitale, quindi Windows
> SmartScreen potrebbe mostrare *"Windows ha protetto il PC"*. Clicca su
> **Ulteriori informazioni → Esegui comunque**. È normale per le app gratuite e
> indipendenti.

Sei alle prime armi? La [**Guida di benvenuto e installazione**](WELCOME.it.md)
ti accompagna passo passo senza dare nulla per scontato.

### Configurazione iniziale (obbligatoria)

Il "cervello" di Friday gira in locale tramite **Ollama**, un motore AI locale e
gratuito:

1. Installa [Ollama](https://ollama.com).
2. Scarica il modello una volta, da terminale:
   ```
   ollama pull qwen2.5:3b
   ```
3. Assicurati che Ollama sia in esecuzione, poi avvia Friday.

La prima volta che apri la voce, vengono scaricati una tantum i modelli vocali
(qualche centinaio di MB); dopodiché funziona per sempre offline.

---

### Documentazione

| Documento | Di cosa parla |
|---|---|
| [Benvenuto e installazione](WELCOME.it.md) | Per principianti, passo passo: installare, avviare, prima chat, prima voce |
| [Changelog](../CHANGELOG.md) | Cosa è cambiato in ogni versione (in inglese) |
| [Licenza](../LICENSE) | MIT — libero utilizzo |

---

### Requisiti di sistema

Friday esegue il modello AI e la voce **sulla tua macchina**, quindi il risultato
dipende dal tuo PC. Questi sono i minimi realistici per il modello incluso
`qwen2.5:3b`.

| | Minimo | Consigliato |
|---|---|---|
| **Sistema operativo** | Windows 10 / 11, 64 bit | Windows 11, 64 bit |
| **CPU** | Qualsiasi processore moderno a 64 bit (x64) | CPU multi-core recente |
| **RAM** | 8 GB | 16 GB |
| **Spazio su disco** | ~4 GB (app ≈0,5 GB · modello ≈2 GB · modelli vocali ≈0,5 GB) | 6 GB+ |
| **GPU** | Nessuna — gira su CPU (voce più lenta) | Una GPU con supporto **WebGPU** (NVIDIA / AMD / Intel recenti) per una voce reattiva |
| **Internet** | Solo per la configurazione iniziale (Ollama, modello, primo download voce) | — |

- **[Ollama](https://ollama.com)** deve essere in esecuzione in locale con
  `qwen2.5:3b` scaricato (`ollama pull qwen2.5:3b`).
- Tutto il resto — chat e voce — funziona offline una volta configurato.
- Con meno RAM o senza GPU, Friday funziona lo stesso; le risposte e la voce
  richiedono solo più tempo.

---

### Privacy in breve

- **Nessun account, nessuna API key, nessuna telemetria, nessuna analitica,
  nessun aggiornamento automatico.**
- Il modello linguistico gira **sulla tua macchina** tramite Ollama.
- La voce (riconoscimento vocale e sintesi vocale) gira **sul dispositivo**.
- L'unico utilizzo della rete è il download una tantum dei modelli vocali e i
  tuoi messaggi che vanno a Ollama sul tuo stesso computer.

---

### Licenza

MIT — libero utilizzo. Vedi [LICENSE](../LICENSE). Il prodotto **Friday** completo di
cui questo è un'anteprima è un'applicazione separata e proprietaria.
