[Retour au cours](../cours.md)

# Généralités sur les développements

## Qui est un bon développeur ?

1. Il prend le temps d'organiser (de façon logique et évidente) ses développements

2. Il sait se concentrer sur la tâche qu'il fait (et non une qu'il faudra faire plus tard)

3. Il sait commenter (et documenter) son code correctement

_NB : un commentaire de code n'est pas une paraphrase du code_

4. Il arrive à garder une cohérence et une structure solide tout au long de ses développements

5. Il sait limiter le nombre de caractères qu'il a à écrire et minimiser les dépendances

6. Il sait limiter la taille de ses fichiers (en ligne et en colonne)

7. Il ne reste pas dans son coin sans chercher (sur Internet au pire)

8. Il sait chercher intelligemment de l'aide sur le web

9. Il a un niveau d'anglais correct mais code en une seule langue

10. Il crée du code intelligible et robuste et respecte les bonnes pratiques :

- des noms de variables explicites : on dit "révélateurs d'intention"

#### Exemple

on évite ~~`toto`~~ ou ~~`plop`~~, on va préférer `couleurProduit` à ~~`cp`~~

- des fonctions qui _ne font qu'une seule chose_ avec des __noms descriptifs__ (utilisation de verbes d'action)

#### Exemple

on va avoir des noms de fonctions comme `getCouleurProduit()` et `getCouleurComplementaire()` plutôt que ~~`getCouleurProduitAndCouleurComplementaire()`~~ qui est, en plus, beaucoup trop long...

11. Il écrit des tests relatifs à ce qu'il a rédigé

### En gros

Le bon développeur est soigné, lisible, endurant, explicite, organisé, ouvert, critique, appliqué, logique, anglophone...
Pas mal !

Il connait aussi des "principes" simples :
* KISS : Keep It Simple, Stupid
* DRY : Don't Repeat Yourself
...

## Organisation de vos données

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
| +--css
|  +--style.css
| +--js
|  +--date.js
| +--img
|  +--drapeau.png
| +--index.php
| +--cv.html
| +--presentation.html
```

## Outils

### Vérification

#### html

* Markup Validation Service

#### css

* CSS Validation Service

#### js

* Lint

#### php

* phpcs
* phpcpd

#### Autres outils

* addons navigateur

### Documentation

* phpdoc

[Retour au cours](../cours.md)
