# FRIDAY Demo — un chatbot et agent vocal gratuit, 100 % local

🌐 [English](README.md) · [Italiano](README.it.md) · [Español](README.es.md) · **Français** · [Deutsch](README.de.md) · [Português](README.pt.md) · [हिन्दी](README.hi.md)

[![Télécharger](https://img.shields.io/badge/T%C3%A9l%C3%A9charger-Derni%C3%A8re%20version-e91e63?logo=github)](../../releases/latest)
[![Licence](https://img.shields.io/badge/Licence-MIT-2ea44f)](LICENSE)
[![Plateforme](https://img.shields.io/badge/Windows-10%20%2F%2011-0078D6?logo=windows)](../../releases/latest)

**Un chatbot et assistant vocal doté d'IA, gratuit, qui fonctionne entièrement
sur votre propre ordinateur.** Écrivez ou parlez — Friday répond par écrit et à
voix haute, avec une voix que vous choisissez — **sans compte, sans clé d'API,
sans abonnement, sans cloud et sans télémétrie.** Rien de ce que vous dites n'est
envoyé à un serveur : le modèle s'exécute en local via
[Ollama](https://ollama.com), et la voix fonctionne sur l'appareil.

> **Local. Privé. Gratuit.** Téléchargez l'installeur, lancez-le et commencez à
> parler. Friday répond en **anglais**.

Ceci est un avant-goût gratuit de l'assistant de bureau **Friday**, plus complet.
Il ne garde que deux choses — le **chat** et le **mode vocal avancé** — et rien
d'autre.

---

### L'essentiel

- 💬 **Chat** — un modèle de langage local via [Ollama](https://ollama.com), la réponse s'affichant mot à mot.
- 🎙️ **Mode vocal avancé** — une sphère de particules en plein écran, mains libres, avec détection neuronale du tour de parole. Maintenez **Espace** ou touchez le micro ; elle écoute, réfléchit et vous répond à voix haute.
- 🔊 **Six voix sur l'appareil** — choisissez celle que vous préférez dans l'en-tête. L'audio ne quitte jamais votre machine.
- 💾 **Sessions enregistrées** — vos conversations précédentes sont conservées en local et rechargeables.
- 🌐 **Voix entièrement hors ligne** — le moteur vocal (Kokoro) et l'environnement d'exécution sont inclus ; seuls le téléchargement unique des modèles vocaux et vos messages vers votre propre Ollama passent par le réseau.
- 🇬🇧 **Toujours en anglais** — quoi que vous écriviez ou disiez, Friday répond en anglais.

---

### Captures d'écran

<table>
<tr>
<td width="50%">

**Chat** — le cœur neuronal, les diagnostics en direct et une conversation en streaming avec le modèle local.
<img src="docs/screenshots/chat.png" alt="Interface de chat de Friday Demo" width="100%">

</td>
<td width="50%">

**Mode vocal avancé** — une sphère réactive en plein écran avec détection neuronale du micro ; maintenez Espace ou touchez pour parler.
<img src="docs/screenshots/voice.png" alt="Mode vocal avancé de Friday Demo" width="100%">

</td>
</tr>
</table>

---

### Téléchargement et installation

1. Ouvrez la page [**Releases**](../../releases/latest) et téléchargez
   `Friday-Voice-Agent-Setup-<version>.exe`.
2. Lancez-le. L'installeur est **par utilisateur** — il **ne nécessite aucun droit
   administrateur**.
3. Démarrez **Friday Voice Agent** depuis le menu Démarrer (ou le raccourci sur le
   bureau, si vous l'avez demandé).

> **Premier lancement :** l'installeur n'est pas signé numériquement, donc Windows
> SmartScreen peut afficher *« Windows a protégé votre ordinateur »*. Cliquez sur
> **Informations complémentaires → Exécuter quand même**. C'est normal pour les
> applications gratuites et indépendantes.

Nouveau ici ? Le [**guide de bienvenue et d'installation**](WELCOME.fr.md) vous
accompagne étape par étape sans rien présupposer.

### Configuration initiale (obligatoire)

Le « cerveau » de Friday s'exécute en local via **Ollama**, un moteur d'IA local
et gratuit :

1. Installez [Ollama](https://ollama.com).
2. Téléchargez le modèle une fois, dans un terminal :
   ```
   ollama pull qwen2.5:3b
   ```
3. Vérifiez qu'Ollama est en cours d'exécution, puis lancez Friday.

La première fois que vous ouvrez la voix, les modèles vocaux se téléchargent une
seule fois (quelques centaines de Mo) ; ensuite, tout fonctionne hors ligne pour
toujours.

---

### Documentation

| Document | Contenu |
|---|---|
| [Bienvenue et installation](WELCOME.fr.md) | Pour débutants, étape par étape : installer, lancer, premier chat, première voix |
| [Changelog](CHANGELOG.md) | Ce qui a changé à chaque version (en anglais) |
| [Licence](LICENSE) | MIT — utilisation libre |

---

### Configuration requise

Friday exécute le modèle d'IA et la voix **sur votre propre machine**, donc le
résultat dépend de votre PC. Voici les minimums réalistes pour le modèle inclus
`qwen2.5:3b`.

| | Minimum | Recommandé |
|---|---|---|
| **Système** | Windows 10 / 11, 64 bits | Windows 11, 64 bits |
| **Processeur** | Tout processeur 64 bits (x64) moderne | CPU multicœur récent |
| **RAM** | 8 Go | 16 Go |
| **Espace libre** | ~4 Go (app ≈0,5 Go · modèle ≈2 Go · modèles vocaux ≈0,5 Go) | 6 Go+ |
| **GPU** | Aucun — s'exécute sur le CPU (voix plus lente) | Un GPU avec prise en charge **WebGPU** (NVIDIA / AMD / Intel récents) pour une voix réactive |
| **Internet** | Uniquement pour la configuration initiale (Ollama, modèle, premier téléchargement vocal) | — |

- **[Ollama](https://ollama.com)** doit être en cours d'exécution en local avec
  `qwen2.5:3b` téléchargé (`ollama pull qwen2.5:3b`).
- Tout le reste — chat et voix — fonctionne hors ligne une fois configuré.
- Avec moins de RAM ou sans GPU, Friday fonctionne quand même ; les réponses et la
  voix prennent simplement plus de temps.

---

### Confidentialité en un coup d'œil

- **Aucun compte, aucune clé d'API, aucune télémétrie, aucune analyse, aucune mise
  à jour automatique.**
- Le modèle de langage s'exécute **sur votre propre machine** via Ollama.
- La voix (reconnaissance et synthèse vocales) s'exécute **sur l'appareil**.
- Le seul usage réseau est le téléchargement unique des modèles vocaux et vos
  propres messages allant vers Ollama sur votre propre ordinateur.

---

### Licence

MIT — utilisation libre. Voir [LICENSE](LICENSE). Le produit **Friday** complet
dont ceci est un aperçu est une application distincte et propriétaire.
