# Pokédex Kanto

Projet de web design réalisé par **Richard Dartus**, **Elliot Hallais** et **Emmanuelle Poiffaut**.

Il s'agit d'une application web front-end autour d'un **Pokédex de la 1re génération** (151 Pokémon), construite en HTML/CSS/JavaScript avec **AngularJS**.

<p align="center">
  <img src="img/Pokedex.PNG" alt="Aperçu du projet Pokédex Kanto" width="700">
</p>

## 🎯 Aperçu

Le projet propose :

- Une **page d'accueil** avec ambiance sonore.
- Une **liste de Pokémon** avec chargement progressif.
- Une **recherche** sur le nom, la description et les types.
- Un **tri avancé** (numéro, taille, poids, ordre alphabétique).
- Une **fiche détaillée** par Pokémon.
- Un **comparateur** de statistiques avec graphique radar.
- Une page **À propos** présentant le projet et l'équipe.
- Une page **404** personnalisée.

Les données sont chargées depuis un JSON local en français (`data/pokAPI.json`).

## ✨ Fonctionnalités principales

### 📚 Liste des Pokémon
- Affichage responsive des 151 Pokémon de Kanto.
- Infinite scroll pour limiter le chargement initial.
- Recherche textuelle.
- Tri croissant/décroissant selon plusieurs critères.
- Navigation vers la fiche détaillée.

### 🔍 Fiche Pokémon
- Image, types, taille, poids et description.
- Graphique radar des statistiques de base via Chart.js.
- Navigation vers le Pokémon précédent/suivant.
- Affichage des évolutions.
- Carte des zones de localisation.
- Section de commentaires.
- Avis "expert" personnalisé pour certains Pokémon.

### ⚔️ Comparateur
- Sélection de deux Pokémon.
- Affichage côte à côte.
- Comparaison sur un même graphique radar.

### 👥 À propos
- Présentation du contexte du projet.
- Présentation de l'équipe.
- Effets visuels et parallaxe.

## 🛠️ Stack technique

- **AngularJS 1.x**
- **Angular Route**
- **Bootstrap**
- **duScroll**
- **ngInfiniteScroll**
- **Chart.js**
- **jQuery**

## 📁 Structure du projet

```text
.
├── index.html              # Page d'accueil
├── pokedex.html            # Application principale AngularJS
├── partials/               # Vues (liste, fiche, comparateur, etc.)
├── js/                     # Logique AngularJS et scripts utilitaires
├── css/                    # Styles du projet
├── data/                   # Données JSON, audio, cartes
├── img/                    # Visuels Pokémon et assets
└── Chart.js-2.0-dev/       # Librairie Chart.js embarquée
```

## 🚀 Lancer le projet

Projet statique : pas de build nécessaire.

### Option simple
Ouvrir `index.html` dans un navigateur, puis entrer dans le Pokédex.

### Option recommandée
Servir le dossier avec un petit serveur local pour éviter les soucis de chargement de fichiers selon le navigateur.

Exemple :

```bash
python3 -m http.server 8000
```

Puis ouvrir :

- `http://localhost:8000/index.html`
- `http://localhost:8000/pokedex.html#/liste`

## 🧬 Données

- **151 Pokémon** de la région de **Kanto**.
- Données locales stockées dans `data/pokAPI.json`.
- Commentaires stockés dans `data/comment.json`.

## ⚠️ Limites connues

- L'envoi de commentaires côté front existe, mais la **sauvegarde persistante** ne fonctionne pas réellement sur un hébergement statique.
- Le projet repose sur une stack front-end ancienne (**AngularJS 1.x**).
- Certains comportements ont été pensés pour les navigateurs et contraintes de l'époque du projet.

## 🗂️ Contexte

Ce dépôt archive un projet étudiant orienté **web design**, **responsive design** et **mise en pratique d'AngularJS** autour d'un thème Pokémon.
