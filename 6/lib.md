[Retour au cours](../cours.md)

# Outils de gestion des dépendances

La plupart des outils comporte :

* Un descripteur de projet qui liste les dépendances
* Un utilitaire en ligne de commande
* Un dépôt central à partir duquel on télécharge les packages (tout en ayant la possibilité de monter des dépôts privés)

L'utilitaire en ligne de commande offre généralement au moins les opérations suivante :

* init : génération d'un descripteur de projet
* install : installer les dépendances
* update : mettre à jour les/des dépendances
* search : rechercher un package

## PHP - COMPOSER/SATIS

Composer permet :

* La gestion efficace des dépendances d'un projet
* La génération des autoloaders (pour éviter de faire des include/require_once partout dans le code)
* L'exécution de script post install et post update

Principe :

* composer.json décrit le projet
* L'exécutable composer lit le fichier composer.json et installe les dépendances dans vendor
* L'utlisateur fait un seul include : vendor/autoload.php
* Dépôt central : [Packagist](https://packagist.org/)
* Dépôt privé : [SATIS](https://github.com/composer/satis)
* Démarrage rapide : [Introduction et Basic usage (getcomposer.org)](https://getcomposer.org/doc/00-intro.md) puis tester [Silex](http://silex.sensiolabs.org/)

## NodeJS - NPM

_NB : ici, on parle de JavaScript qui est exécuté côté serveur_

Principalement utilisé pour :

* Gérer les dépendances NodeJS (express par exemple)
* Gérer l'installation des outils côté serveur (less, grunt mais aussi bower)
* Gérer l'exécution de tâche (`npm start` pour démarrer un serveur)
* Descripteur du projet : package.json
* Dépôt central : [npmjs.com](https://www.npmjs.com/)
* Démarrage rapide : [Tester express](https://www.npmjs.com/package/express)

Remarque :

* Noter la notion d'installation globale (`npm install -g less`)
* Noter aussi l'existence de [Grunt](http://gruntjs.com/getting-started) et Gulp pour en automatiser certaines
tâches (validation du code JavaScript : lint, minification de code : uglify, )

## JavaScript (front-end) - Bower

Principalement utilisé pour gérer les bibliothèques tierces utilisées pour la réalisation du front (AngularJS, jQuery, Leaflet et ses plugins, etc.)

* Descripteur du projet : bower.json
* Dépôt central : [bower.io](http://bower.io/search/)
* Démarrage rapide : [bower.io/#getting-started](http://bower.io/#getting-started)

### Autres exemples

* CMake - C++

* Java - MAVEN/NEXUS

# Quelques exemples de bibliothèques

## Bibliothèques (js)

### Définition

_Bibliothèque_ : un (ou plusieurs) fichier(s) .js déjà codé(s) contenant des méthodes et des propriétés pour l’ajout de fonctionnalités dynamiques (données) à une page HTML

### Liste NON-exhaustive

#### DOM

* JQuery
* Prototype.js

#### UI

* bootstrap
* JQuery UI

#### Visualisation

* echarts
* D3.js

#### Carto

* openlayers
* leaflet

## Ressources (css)

### Définition

_Ressource_ : un (ou plusieurs) fichier(s) .css déjà codé(s) contenant des style pour le design de la page HTML

### Liste NON-exhaustive

* Balloon

* Hue

## Bibliothèques (php)

### Définition

_Bibliothèque_ : un (ou plusieurs) fichier(s) .php déjà codé(s) contenant différentes fonctionnalités

### Liste NON-exhaustive

* phpDocumentor

* SwiftMailer

[Retour au cours](../cours.md)
