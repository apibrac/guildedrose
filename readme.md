# Exercice Guilded Rose

## Installation de la librairie de tests

`npm install`

## Lancement des tests

`npm run test` pour tester une fois

`npm run test:watch` pour relancer les tests concernés à chaque fois qu'un fichier est modifié

`npm run test:coverage` pour vérifier la proportion de code testée. Idéalement il faudrait arriver à 100%

## Consignes

### Introduction

Bonjour et bienvenue dans l'équipe de développement Gilded Rose.

Nous sommes une petite auberge située dans une grande ville.

Nous achetons et revendons toutes sortes d'articles. Malheureusement, la qualité de nos articles se dégrade au fur et à mesure que leur date d'expiration approche.

Nous avons un système qui met à jour notre inventaire chaque jour selon les règles suivantes:

- tous les articles ont une propriété `daysToSell` qui indique le nombre de jours restant avant la date d'expiration
- tous les articles ont une propriété `quality` qui indique leur valeur
- pour la majorité des articles, chaque jour, ces deux propriétés perdent une unité

Cas particuliers

- l’article intitulé "Brie de Meaux" augmente en qualité d'une unité chaque jour

### Recommendations générales

Prenez le temps de bien indenter le code pour qu'il soit lisible.
Faites un commit par exercice.

### Exercice 1 : la qualité d’un article n'est jamais supérieure à 50

Ajouter dans le fichier `shop.js` le code correspondant permettant de vérifier la contrainte suivante: "la qualité d’un article n'est jamais supérieure à 50".

Le test correspondant est déjà écrit dans `shop.spec.js` et il est commenté.
Dé-commentez ce test.
Une fois votre code écrit, ce test doit passer.

### Exercice 2 : l'article "Sulfuras"

Ajouter dans le fichier `shop.js` le code correspondant permettant de vérifier la contrainte suivante: l'article "Sulfuras" n'a pas de date limite, et sa qualité est toujours égale à 80.

Les tests correspondants sont déjà écrits dans `shop.spec.js` et ils sont commentés.
Dé-commentez ces tests.
Une fois votre code écrit, ces tests doivent passer.

### Exercice 3 : l'article "Backstage passes"

Ajouter dans le fichier `shop.js` le code correspondant permettant de vérifier la contrainte suivante: la qualité de l'article "Backstage passes" :

- tombe à zéro quand le nombre de jours avant la date d'expiration est inférieur à 0 (quand le concert est passé)
- augmente chaque jour de 3 quand le nombre de jours avant la date d'expiration est inférieur ou égal à 5
- augmente chaque jour de 2 quand le nombre de jours avant la date d'expiration est inférieur ou égal à 10

Le test correspondant est déjà écrit dans `shop.spec.js` et il est commenté.
Dé-commentez ce test.
Une fois votre code écrit, ce test doit passer.

### Exercice 4 : l'article "Conjured"

Ajouter dans le fichier `shop.spec.js` :

- un 9ème article qui a pour nom "Conjured", une qualité égale à 12, et un nombre de jours avant expiration égal à 8
- un test qui vérifie que la qualité de cet article décroit de 2 chaque jour. Dans un premier temps, ce test ne passera pas, c'est normal puisque vous n'avez pas encore écrit le code correspondant dans `shop.js`

Ajoutez ensuite le code permettant de faire passer ce test dans `shop.js`

Bravo, vous avez terminé !
