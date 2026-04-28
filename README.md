# Pokédex Kanto

Projet de web design réalisé par **Richard Dartus**, **Elliot Hallais** et **Emmanuelle Poiffaut**.

Il s'agit d'une application web front-end autour d'un **Pokédex de la 1re génération** (151 Pokémon), construite en HTML/CSS/JavaScript avec **AngularJS**.

![Aperçu du projet](img/Pokedex.PNG)

## Aperçu

Le projet propose :

- une **page d'accueil** avec ambiance sonore
- une **liste de Pokémon** avec chargement progressif
- une **recherche** sur le nom, la description et les types
- un **tri avancé** (numéro, taille, poids, ordre alphabétique)
- une **fiche détaillée** par Pokémon
- un **comparateur** de statistiques avec graphique radar
- une page **À propos** présentant le projet et l'équipe
- une page **404** personnalisée

Les données sont chargées depuis un JSON local en français (`data/pokAPI.json`).

## Fonctionnalités principales

### Liste des Pokémon
- affichage responsive des 151 Pokémon de Kanto
- infinite scroll pour limiter le chargement initial
- recherche textuelle
- tri croissant/décroissant selon plusieurs critères
- navigation vers la fiche détaillée

### Fiche Pokémon
- image, types, taille, poids et description
- graphique radar des statistiques de base via Chart.js
- navigation vers le Pokémon précédent/suivant
- affichage des évolutions
- carte des zones de localisation
- section de commentaires
- avis "expert" personnalisé pour certains Pokémon

### Comparateur
- sélection de deux Pokémon
- affichage côte à côte
- comparaison sur un même graphique radar

### À propos
- présentation du contexte du projet
- présentation de l'équipe
- effets visuels et parallaxe

## Stack technique

- **AngularJS 1.x**
- **Angular Route**
- **Bootstrap**
- **duScroll**
- **ngInfiniteScroll**
- **Chart.js**
- **jQuery**

## Structure du projet

```text
.
├── index.html              # page d'accueil
├── pokedex.html            # application principale AngularJS
├── partials/               # vues (liste, fiche, comparateur, etc.)
├── js/                     # logique AngularJS et scripts utilitaires
├── css/                    # styles du projet
├── data/                   # données JSON, audio, cartes
├── img/                    # visuels Pokémon et assets
└── Chart.js-2.0-dev/       # librairie Chart.js embarquée
```

## Lancer le projet

Projet statique : pas de build nécessaire.

### Option simple
Ouvrir `index.html` dans un navigateur, puis entrer dans le Pokédex.

### Option recommandée
Servir le dossier avec un petit serveur local pour éviter les soucis de chargement de fichiers selon le navigateur.

Exemples :

```bash
python3 -m http.server 8000
```

Puis ouvrir :

- `http://localhost:8000/index.html`
- ou directement `http://localhost:8000/pokedex.html#/liste`

## Données

- **151 Pokémon** de la région de **Kanto**
- données locales stockées dans `data/pokAPI.json`
- commentaires stockés dans `data/Comment.json`

## Limites connues

- l'envoi de commentaires côté front existe, mais la **sauvegarde persistante** ne fonctionne pas réellement sur un hébergement statique
- le projet repose sur une stack front-end ancienne (**AngularJS 1.x**)
- certains comportements ont été pensés pour les navigateurs et contraintes de l'époque du projet

## Contexte

Ce dépôt archive un projet étudiant orienté **web design**, **responsive design** et **mise en pratique d'AngularJS** autour d'un thème Pokémon.
