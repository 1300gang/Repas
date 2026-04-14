# Planificateur Famille

Application web de planification des repas hebdomadaires avec génération automatique de liste de courses, orientée **batch cooking** pour 4 personnes.

## Fonctionnalités

- **Planning hebdomadaire** — assigner des recettes aux déjeuners et dîners de chaque jour
- **Batch cooking** — certains repas partagent la même préparation sur plusieurs jours (évite le double comptage des ingrédients)
- **Remplissage aléatoire** — génère un planning en un clic selon les thèmes configurés par jour
- **Liste de courses** — agrège automatiquement les ingrédients des recettes + les produits essentiels, regroupés par rayon
- **Suivi des achats** — cocher les articles au fur et à mesure (avec barré visuel)
- **Estimation du coût** — total estimé basé sur les recettes sélectionnées
- **Gestion des recettes** — ajout de recettes personnalisées avec ingrédients, coût et rayon
- **Gestion des produits** — liste des essentiels récurrents (petit-déjeuner, desserts, ménage…)
- **Export / Import** — sauvegarde en JSON et restauration
- **Copie pour Notion / Google Keep** — formatage adapté pour coller ailleurs

## Stack technique

- HTML5 / CSS3 / JavaScript vanilla (aucune dépendance, aucun build)
- Persistance via `localStorage` (schéma v4)
- Fonctionne directement en ouvrant `index.html` dans un navigateur

## Structure

```
index.html   # SPA complète (UI + logique JS embarquée)
style.css    # Styles (responsive, mobile-first, 2 colonnes sur grands écrans)
data.js      # Données par défaut : ~55 recettes, essentiels, config semaine
```

## Lancement

```
Ouvrir index.html dans un navigateur — aucune installation requise.
```

## Utilisation rapide

1. Configurer le planning (choisir les recettes ou cliquer **Remplir le planning**)
2. Cocher les produits essentiels nécessaires
3. Cliquer **Générer** pour créer la liste de courses
4. Cocher les articles pendant les courses
5. Optionnel : **Exporter** les données ou **Copier pour Notion**

## Recettes par défaut

55+ recettes réparties par thème (Indien, Américain, Français, Asiatique, Africain, Sud-Américain, Italien) avec type Midi ou Soir, coût estimé et ingrédients par rayon.
