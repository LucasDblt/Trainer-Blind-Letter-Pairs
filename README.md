# 🧠 Trainer Blindfold 3x3

Un outil web simple et complet pour s'entraîner à la mémorisation du Rubik's Cube en aveugle (3BLD). Il permet de générer des paires de lettres pour les Arrêtes (Edges) et les Coins (Corners) en respectant vos contraintes de groupes (buffers).

## ✨ Fonctionnalités

* **Gestion intelligente des groupes :** Ne propose jamais deux lettres appartenant au même groupe (pièce/sticker) selon votre propre configuration.
* **Connexion Google Sheets :** Affiche vos propres mots mémotechniques associés aux paires.
* **Mode Flashcard :** Affiche la paire, vous laisse deviner, puis affiche la réponse.
* **Mode Cycle (Deck) :** Passe en revue toutes les paires disponibles une fois avant de recommencer (pas de doublons).
* **Mode Métronome :** Défilement automatique pour travailler la vitesse.
* **Filtres avancés :** Possibilité d'imposer une lettre précise en 1ère ou 2ème position.

---

## 🚀 Comment lier votre liste de mots (Google Sheets)

Pour que l'outil affiche vos mots sous les paires, suivez ces étapes (à faire une seule fois) :

1.  Ouvrez un **Google Sheet** vierge.
2.  Collez vos paires dans la **Colonne A** et vos mots dans la **Colonne B** (sans en-têtes).
    * *Exemple : `AB` en A1, `Abeille` en B1.*
3.  Allez dans **Fichier > Partager > Publier sur le web**.
4.  Dans le menu déroulant "Page Web", choisissez **"Valeurs séparées par des tabulations (.tsv)"**.
5.  Cliquez sur **Publier** et copiez le lien généré.
6.  Collez ce lien dans la case en haut de l'outil Trainer Blindfold.
    * *Le lien est sauvegardé automatiquement dans votre navigateur pour les prochaines fois.*

---

## 🎮 Les Modes de Jeu

### 1. Mode Standard (Par défaut)
Appuyez sur `ESPACE`. Une paire aléatoire s'affiche. Idéal pour l'exécution pure.

### 2. Mode Flashcard (Vérif)
Cochez la case **"Flashcard"**.
* **1er appui :** Affiche la paire (ex: `AB`).
* **2ème appui :** Affiche le mot réponse en jaune (ex: `Abeille`).
* **3ème appui :** Passe à la paire suivante.

### 3. Mode Cycle (Exhaustif)
Cochez la case **"Cycle"**.
L'outil va piocher dans la liste sans jamais remettre une paire déjà vue tant que la liste n'est pas finie. Un compteur en bas à droite (ex: `15 / 420`) vous indique où vous en êtes.

### 4. Mode Métronome (Auto)
Cochez la case **"Métronome"**.
Les paires défilent toutes seules selon la vitesse réglée avec le curseur. Appuyez sur `ESPACE` pour mettre en pause.

---

## 🔍 Filtres et Personnalisation

* **Arrêtes / Coins :** Cliquez sur les boutons en haut pour changer de mode.
* **Zone "Groupes" :** C'est ici que vous définissez quelles lettres sont incompatibles (votre buffer et les stickers d'une même pièce).
    * *Fonctionnement :* Les lettres collées ensemble sont considérées comme un groupe unique. Séparez les groupes par un espace.
* **Zone "Imp" (Imposé) :** Force l'apparition d'une lettre spécifique.
    * Le menu déroulant permet de choisir sa place :
        * `*` : N'importe où.
        * `1` : En première position uniquement.
        * `2` : En deuxième position uniquement.

---

## 🛠 Installation locale

Si vous ne souhaitez pas utiliser la version en ligne :
1.  Téléchargez le fichier `index.html`.
2.  Ouvrez-le simplement avec n'importe quel navigateur (Chrome, Firefox, Safari).
3.  Pas besoin d'internet (sauf pour charger le Google Sheet la première fois).
