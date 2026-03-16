# ⚡ Pokémon Clicker

> Un jeu idle/clicker dans l'univers Pokémon, inspiré de Cookie Clicker.
> Cliquez, capturez, prestigez — attrapez les 151 Pokémon de la Génération 1 !

🎮 **[Jouer maintenant](https://moifay.github.io/Pok-Clicker/)**
💜 **[Soutenir le projet](https://subs.twitch.tv/moifay)**

---

## 📋 Table des matières

- [Présentation](#présentation)
- [Fonctionnalités](#fonctionnalités)
- [Structure du projet](#structure-du-projet)
- [Systèmes de jeu](#systèmes-de-jeu)
- [Roadmap](#roadmap)

---

## Présentation

Pokémon Clicker est un jeu de navigateur **gratuit**, **sans publicité**, jouable sur **PC et mobile** sans installation.
Cliquez sur la Pokéball pour gagner des Poké Dollars, achetez des bâtiments, capturez des Pokémon et progressez vers le Prestige.

---

## Fonctionnalités

### 🔴 Pokéball — Bâtiment de base
Chaque Pokéball achetée augmente la valeur de votre clic de +1 ₽.
Trois upgrades dédiées (Pokéball Renforcée, Superball, Hyperball, Masterball) multiplient ce bonus jusqu'à ×120.

### 🏢 51 Bâtiments
Du Centre Pokémon (300 ₽) au DIEU ARCEUS (valeur astronomique).
Chaque bâtiment produit des ₽/seconde automatiquement. Le coût augmente de ×1.15 par achat.
Achat par ×1 / ×10 / ×100 / MAX.

### ⬆️ 148 Améliorations
- **Click flat** — bonus fixe par clic (12 niveaux)
- **Click mult** — multiplicateurs de clic
- **Click ratio** — % du CPS ajouté aux clics
- **Global mult** — multiplicateur de toute la production
- **Bldg mult** — ×2 la production d'un bâtiment spécifique
- **Ev rate** — augmente le taux d'apparition des Pokémon
- **Prestige mult** — multiplie le bonus des Bonbons Rares

### 🐾 151 Pokémon Gen 1 — Système unifié
Tous les Pokémon de Bulbizarre (#1) à Mew (#151) apparaissent aléatoirement toutes les **2 à 5 minutes**.
Cliquez dessus avant qu'ils disparaissent pour déclencher leur effet !

| Rareté | Effet |
|--------|-------|
| ⚪ Commun | Auto-clic pendant 8 secondes |
| 🟢 Peu commun | Auto-clic pendant 13 secondes |
| 🔵 Rare | +25% CPS pendant 30 secondes |
| 🟣 Épique (Starters, Alakazam, Gengar…) | ×5 à ×15 production pendant 8-12s |
| 🟡 Légendaire (Artikodin, Électhor, Sulfura) | ×100 à ×200 pendant 5s |
| ⭐ Ultra (Mewtwo ×666 / Mew ×777) | ×666 ou ×777 pendant 6-7s |

Les multiplicateurs Épique → Ultra s'appliquent **simultanément sur le CPS et les clics**.

### 📖 Pokédex
Grille complète des 151 Pokémon dans l'ordre numérique.
- Pokémon capturé : sprite, nom, rareté colorée, compteur de captures
- Pokémon manquant : numéro + ❓ + rareté visible pour donner envie de le chercher

### 🍬 Prestige
Seuils : #1 = 500 Milliards, ×5 à chaque fois (basé sur les gains légitimes uniquement).
Donne **1 Bonbon Rare 🍬** par prestige → +2% production permanente (multiplicatif).
Les améliorations achetées sont **conservées** après prestige.

**Option Reset Pokédex** : activez le toggle avant le prestige pour remettre à zéro votre Pokédex en échange de taux de rareté boostés (×1.5 à ×6 pour les Pokémon non encore capturés).

### 🌟 Méga Prestige
Déblocable avec 100 Bonbons Rares. Reset total en échange d'un ×10 permanent sur toute la production (cumulatif à chaque Méga Prestige).

### 🛍️ Boutique Bonbons Rares
20 améliorations permanentes achetables avec des Bonbons Rares, conservées après tous les resets.
Exemples : +1% chance d'événement, −5% prix bâtiments, +10% gains hors-ligne, +200% production globale.

### 🔵 Système de Perles *(nouveau)*
Chaque Pokémon capturé remplit une barre de progression selon sa rareté.
Une fois pleine → **1 Perle**.

**Conversion :** 30 Perles → 1 Triple Perle · 10 Triples → 1 Grande Perle

**Boutique Perles** — 10 items temporaires :

| Monnaie | Item | Effet |
|---------|------|-------|
| 🔵 Perles | Encens Pokémon | ×2 fréquence spawn 15 min |
| 🔵 Perles | Miel | Pokémon reste 2× plus longtemps |
| 🔵 Perles | Rappel | Refait apparaître le dernier Pokémon manqué |
| 🔵 Perles | Super Ball | +50% CPS 10 min |
| 💎 Triples | Hyper Ball | +100% CPS 10 min |
| 💎 Triples | Pierre Feu/Eau/Foudre | +80% CPS ou clic 10 min |
| 💎 Triples | Encens Ultra | Prochain spawn = légendaire/ultra garanti |
| ✨ Grandes | Master Ball | +300% CPS 5 min |

Les durées sont **cumulables** (utiliser 2× le même item additionne le temps). Les effets identiques prennent le **maximum** (pas de cumul multiplicatif).

### 🎯 Objectifs Journaliers
3 défis aléatoires renouvelés chaque jour à minuit. Récompenses scalées sur votre production actuelle (= 30 min de CPS).

Types de défis : Clics, Bâtiments achetés, ₽ gagnés, Pokémon sauvages capturés, Légendaire/Ultra capturé, Améliorations achetées, Perles gagnées.

### 🏆 143 Succès
Répartis en catégories : Clics, Gains, CPS, Bâtiments, Pokédex (progression 1→151), Starters spécifiques, Légendaires, Ultra, Méga Prestige, Boutique Bonbons, Pokéball, Hors-ligne et plus.

### 💾 Sauvegarde
- Auto-save toutes les **30 secondes**
- Export / Import en Base64
- Téléchargement `.txt`
- Gains hors-ligne à **50%** de production (max 24h)
- Fallback automatique des anciennes saves

### 🚫 Anti-Autoclicker
Détection sur 3 signaux : rythme trop régulier, >15 clics/s sur 1s, >12 clics/s sur 3s.
Ban 5 minutes avec compte à rebours. Survit au rechargement de page.
L'autoclicker des Pokémon Communs/Peu communs est **légitime** et bypass ce système.

---

## Structure du projet

```
/
├── index.html          # Jeu complet (HTML + CSS + JS en un seul fichier)
├── icon.png            # Icône de l'application
├── Sprites/            # Sprites Pokémon Gen 1
│   ├── 001.png         # Bulbizarre
│   ├── 002.png         # Herbizarre
│   └── ...             # jusqu'à 151.png (Mew)
└── Items/              # Sprites des items (Perles, Balls, Pierres...)
    ├── perle.png
    ├── perle_triple.png
    ├── grande_perle.png
    └── ...
```

---

## Systèmes de jeu

### Formule de coût des bâtiments
```
coût(n) = coût_base × 1.15^n
```

### Formule de prestige
```
Prestige #1 = 500 Milliards ₽ (légitimes)
Prestige #n = 500B × 5^(n-1)
```

### Points de perles par rareté
```
Commun: 2pts | Peu commun: 5pts | Rare: 12pts
Épique: 25pts | Légendaire: 50pts | Ultra: 100pts
→ 100 points = 1 Perle
```

---

## Roadmap

- [ ] Sprites Pokémon remplacent les emojis dans les popups d'événements
- [ ] Sauvegarde cloud liée au compte Discord
- [ ] Génération 2 (Pokémon 152 → 251)
- [ ] Application desktop Electron
- [ ] PWA mobile (icône sur l'écran d'accueil)

---

*Projet développé par [MoiFay](https://subs.twitch.tv/moifay) · Hébergé sur GitHub Pages*
