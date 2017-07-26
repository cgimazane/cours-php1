# Introduction

[intro](intro.md)

# Usages

## Mise en place (et vérification) de l'environnement

WAMP

* Windows (environnement)
* Apache (serveur web)
* MySql (serveur de base de données)
  - que l'on remplacera par PostgreSQL
* PHP (scripts)

## Généralités sur les développements

### Qui est un bon développeur ?

1. Il prend le temps d'organiser (de façon logique et évidente) et de commenter (et documenter) son code

_NB : un commentaire de code n'est pas une paraphrase du code_

2. Il arrive à garder une cohérence et une structure solide tout au long de ses développements

3. Il sait limiter le nombre de caractères qu'il a à écrire et minimiser les dépendances

4. Il sait limiter la taille de ses fichiers (en ligne et en colonne)

5. Il ne reste pas dans son coin sans chercher (sur Internet au pire)

6. Il sait chercher intelligemment de l'aide sur le web

7. Il a un niveau d'anglais correct mais code en une seule langue

8. Il crée du code intelligible et robuste et respecte les bonnes pratiques :

- des noms de variables explicites : on dit "révélateur d'intention"

#### Exemple

on évite ~~`toto`~~ ou ~~`plop`~~, on va préférer `couleurProduit` à `cp`

- des fonctions qui ne font qu'une seule chose avec des noms descriptifs (utilisation de verbes d'action)

#### Exemple

on va avoir des noms de fonctions comme `getCouleurProduit()` et `getCouleurComplementaire()` plutôt que ~~`getCouleurProduitAndCouleurComplementaire()`~~

9. Il écrit des tests relatifs à ce qu'il a rédigé

### En gros

Le bon développeur est soigné, lisible, explicite, organisé, ouvert, critique, logique et anglophone...

### Organisation de vos données

- Créer des noms de fichiers simples/lisibles
  * Jamais plus de 20 caractères
  * Pas de caractères spéciaux

- Vérifier les extensions de fichiers

- Créer des noms de dossiers simples
  * Ne pas faire des chemins trop longs

- Avoir une hiérarchie simple

#### Exemple

```
+--monProjetWeb
|  +--css
|    +--style.css
|  +--images
|    +--drapeau.png
|  +--index.html
|  +--cv.html
|  +--presentation.html
```

## Outils de vérification du code

lint
validator
firebug

---

# html

[html](html.md)

# Réalisation du travail

Tout au long de la session, réalisation d'un projet sur votre équipe : création d'une page avec la présentation de votre équipe

# css

[css](css.md)


# Amélioration de notre page

* Reprise de la page avec la présentation de votre équipe (deux fois mieux)

# js

[js](js.md)

# Amélioration de notre page

* Reprise de la page en ajoutant de l'interaction

# php

[php](php.md)
