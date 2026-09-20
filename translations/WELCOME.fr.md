# Bienvenue sur Friday 👋

🌐 [English](../WELCOME.md) · [Italiano](WELCOME.it.md) · [Español](WELCOME.es.md) · **Français** · [Deutsch](WELCOME.de.md) · [Português](WELCOME.pt.md) · [हिन्दी](WELCOME.hi.md)

Ce guide vous mène de zéro jusqu'à parler avec Friday, sans **rien** présupposer.
Si vous savez télécharger un fichier, vous savez lancer Friday.

Friday est un assistant IA gratuit qui fonctionne sur **votre propre ordinateur**.
Vous pouvez lui **écrire** ou lui **parler**, et il répond — par écrit et à voix
haute. Aucun compte, aucune inscription, aucun abonnement payant. Friday répond en
**anglais**.

---

## Ce qu'il vous faut

- Un PC sous **Windows 10 ou 11** (64 bits).
- **8 Go de RAM** ou plus (16 Go, c'est confortable). Friday exécute l'IA sur
  votre propre machine, donc la mémoire compte.
- Environ **4 Go d'espace libre** au total : l'application elle-même (~0,5 Go), le
  modèle d'IA que vous téléchargez une fois (~2 Go) et les modèles vocaux
  téléchargés à la première utilisation de la voix (~0,5 Go).
- Une connexion internet **pour la configuration uniquement** — une fois
  configuré, le chat et la voix fonctionnent hors ligne.

Une carte graphique (GPU) avec prise en charge de **WebGPU** (n'importe quel GPU
NVIDIA, AMD ou Intel récent) rend la voix rapide — mais Friday fonctionne aussi
sans, simplement plus lentement. Sur un PC modeste, tout fonctionne quand même ;
les réponses et la voix prennent juste un peu plus de temps.

> Vous ne connaissez pas les caractéristiques de votre PC ? Appuyez sur la
> **touche Windows**, tapez **« À propos de votre PC »** et ouvrez-la — elle
> affiche la version de Windows, le processeur et la RAM installée.

---

## Étape 1 — Installez Ollama (le cerveau de Friday)

Friday réfléchit grâce à un moteur d'IA local et gratuit appelé **Ollama**. Vous
l'installez une seule fois.

1. Allez sur **https://ollama.com** et cliquez sur **Download**.
2. Lancez l'installeur téléchargé et suivez les instructions. Voilà — Ollama
   tourne désormais discrètement en arrière-plan.
3. Ouvrez un terminal (appuyez sur la **touche Windows**, tapez **`cmd`**, appuyez
   sur **Entrée**) et collez cette ligne, puis appuyez sur **Entrée** :

   ```
   ollama pull qwen2.5:3b
   ```

   Cela télécharge le modèle d'IA utilisé par Friday (environ 2 Go). Attendez la
   fin — vous ne le faites qu'une seule fois.

> **Comment savoir si Ollama tourne ?** Après l'installation, cherchez l'icône
> Ollama près de l'horloge dans la barre des tâches. Si vous ne la voyez pas,
> ouvrez le menu Démarrer et lancez **Ollama**.

---

## Étape 2 — Téléchargez Friday

1. Allez sur la page [**Releases**](https://github.com/Alex-Stark-industries/FRIDAY-Demo/releases/latest).
2. Sous la dernière version, téléchargez le fichier nommé
   **`Friday-Voice-Agent-Setup-<version>.exe`**.

---

## Étape 3 — Installez et lancez Friday

1. Ouvrez le fichier que vous venez de télécharger (généralement dans le dossier
   **Téléchargements**).

   **La première fois**, Windows peut afficher un cadre bleu indiquant *« Windows
   a protégé votre ordinateur »*. Cela arrive avec toutes les applis gratuites non
   signées. Cliquez simplement sur :

   - **Informations complémentaires**
   - puis **Exécuter quand même**

2. L'installeur s'ouvre. Il installe **juste pour vous** et **ne demande aucun mot
   de passe administrateur**. Cliquez sur **Suivant → Installer → Terminer**. (Vous
   pouvez cocher « Créer une icône sur le bureau » en chemin si vous le
   souhaitez.)
3. Lancez **Friday Voice Agent** — depuis le **menu Démarrer**, l'**icône du
   bureau**, ou en laissant cochée « Lancer Friday Voice Agent » sur le dernier
   écran de l'installeur.

Friday s'ouvre. Si Ollama tourne, le haut de la fenêtre affiche **ALL SYSTEMS
ONLINE (LOCAL)**.

> **Pour désinstaller plus tard :** ouvrez **Paramètres → Applications** de
> Windows, trouvez *Friday Voice Agent* et cliquez sur **Désinstaller**.

---

## Étape 4 — Votre premier chat

En bas de la fenêtre se trouve un champ indiquant **« Message Friday… »**.

- Cliquez dessus, tapez quelque chose comme *« Hi Friday! What can you do? »* et
  appuyez sur **Entrée**.
- Friday répond dans le panneau, mot à mot. Si le son est activé, il lit aussi la
  réponse à voix haute. Cliquez sur **LISTEN** sous une réponse pour la réécouter.

---

## Étape 5 — Parlez à Friday (mode vocal)

1. Cliquez sur le bouton **micro** (en bas à gauche du champ de message), ou sur
   la commande **Voice mode**, pour ouvrir la sphère lumineuse en plein écran.
2. **Maintenez la barre d'espace** pendant que vous parlez, puis relâchez — ou
   touchez le micro à l'écran.
3. Friday transcrit ce que vous avez dit, réfléchit et **vous répond à voix
   haute**.
4. Vous préférez une autre voix ? Utilisez la commande des voix dans l'en-tête (en
   haut à droite) pour choisir parmi **six voix**.
5. Cliquez sur **✕ EXIT** (en haut à droite) pour revenir au chat.

> **La première utilisation de la voix** télécharge une fois les modèles vocaux
> (quelques centaines de Mo). Ensuite, la voix fonctionne entièrement hors ligne.

---

## Astuces et dépannage

- **Friday indique que les systèmes sont hors ligne / le chat ne répond pas.**
  Ollama n'est pas lancé, ou le modèle n'a pas été téléchargé. Vérifiez qu'Ollama
  est ouvert et que vous avez exécuté `ollama pull qwen2.5:3b` (Étape 1).
- **La voix a choisi le mauvais micro.** Utilisez le bouton **MIC** dans l'en-tête
  pour choisir une autre entrée.
- **Le premier lancement semble lent.** Friday préchauffe son moteur vocal au
  démarrage et télécharge les modèles vocaux à la première utilisation de la voix.
  Les lancements suivants sont plus rapides.
- **Rien n'est envoyé au cloud.** Vos conversations et votre voix restent sur votre
  machine. Le seul usage réseau est le téléchargement unique et vos messages
  allant vers Ollama sur votre propre PC.

---

Profitez de Friday — et si cet avant-goût gratuit vous plaît, ce n'est qu'une
petite part de l'assistant de bureau **Friday** complet.
