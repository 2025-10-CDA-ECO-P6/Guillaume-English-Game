# English Game Project
# The English Game - Front-end Integration

Intégration front-end d'une plateforme de challenge inter-écoles d'anglais.

## 📋 Description

**The English Game** est une plateforme permettant aux étudiants de participer à un challenge inter-écoles pour améliorer leur niveau d'anglais. Ce projet est une intégration statique réalisée à partir d'une maquette Figma fournie.

## 🛠️ Technologies utilisées

- **HTML5** sémantique
- **SCSS** (Sass) avec architecture modulaire
- **Git** pour le versionnement
- **GitHub Pages** pour l'hébergement

## 📁 Structure du projet

```
english-game/
├── index.html
├── css/
│   └── main.css          ← Fichier compilé (généré automatiquement)
├── scss/
│   ├── main.scss          ← Point d'entrée SCSS
│   ├── _variables.scss    ← Variables (couleurs, espacements, breakpoints)
│   ├── _mixins.scss       ← Mixins réutilisables
│   ├── _reset.scss        ← Reset CSS
│   └── components/
│       ├── _header.scss
│       ├── _hero.scss
│       ├── _cards.scss
│       ├── _schedule.scss
│       ├── _project.scss
│       ├── _learning.scss
│       └── _footer.scss
├── assets/
│   └── images/            ← Images et icônes
└── README.md
```

## 🎨 Choix techniques

### Architecture SCSS modulaire

Le projet suit une architecture en composants séparés. Chaque section de la page possède son propre fichier SCSS, importé dans `main.scss`. Cette approche facilite la maintenance et la lisibilité du code.

### Nommage BEM

La convention **BEM** (Block Element Modifier) a été utilisée pour nommer les classes CSS :
- **Block** : `.header`
- **Element** : `.header__nav`
- **Modifier** : `.header__link--active`

### Variables centralisées

Les couleurs, espacements et breakpoints sont définis dans `_variables.scss` en suivant le design system officiel fourni dans le brief (palette `$primary`, `$secondary`, `$neutral`).

### Responsive mobile-first

Le site est conçu avec une approche mobile-first. Les adaptations desktop sont gérées via des mixins de media queries définis dans `_mixins.scss`.

## 📐 Design system

Couleurs principales utilisées :

| Variable | Valeur | Usage |
|----------|--------|-------|
| `$primary700` | `#0f878f` | Header |
| `$primary950` | `#083c44` | Hero, Footer |
| `$primary500` | `#07d3d3` | Schedule |
| `$neutral100` | `#f5f5f5` | Cards, Learning |
| `$secondary300` | `#ffd34a` | Bouton Learning |

## 🚀 Installation et lancement

### Prérequis

- [Node.js](https://nodejs.org/) (pour npm)
- [Sass](https://sass-lang.com/) : `npm install -g sass`

### Lancer le projet

```bash
# Cloner le repo
git clone git@github.com:2025-10-CDA-ECO-P6/Guillaume-English-Game.git

# Aller dans le dossier
cd Guillaume-English-Game

# Compiler le SCSS
sass scss/main.scss css/main.css

# Ouvrir index.html dans le navigateur
```

### Mode watch (développement)

```bash
sass scss/main.scss css/main.css --watch
```

## 📊 Critères d'évaluation

| Critère | Statut |
|---------|--------|
| HTML sémantique | ✅ |
| Architecture SCSS modulaire | ✅ |
| Variables centralisées | ✅ |
| Nommage BEM cohérent | ✅ |
| Accessibilité minimale (aria-label, alt) | ✅ |
| Responsive mobile/desktop | 🔄 En cours |
| Conformité maquette | 🔄 En cours |
| Versionning Git | ✅ |
| README structuré | ✅ |

## 🌐 Démo

[Voir le site en ligne](https://2025-10-cda-eco-p6.github.io/Guillaume-English-Game/)

## 👤 Auteur

**Guillaume** - CDA ECO P6 2025-10