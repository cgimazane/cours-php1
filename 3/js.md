[Retour au cours](../cours.md)

# 3.1 js

## Introduction

### Définition

JavaScript

### Mots-clés

JavaScript est un __langage orienté objet__ interprété par le navigateur, sensible à la casse.
Le JavaScript est un langage « client », c'est-à-dire exécuté chez l'utilisateur lorsque la page Web est chargée.
...
Il a pour but de dynamiser les sites Internet.

### Présentation rapide

Dans notre page Web, on a un objet `window` contenant (entre autres) un objet `document` qui contient lui-même tous les éléments html de la page (paragraphes, tableaux...).

## Présentation du langage

### Variables

* Pas de typage des variables
* Déclaration d'une variable par le mot-clé `var`

#### Exemple

```javascript
var age = 12;
var prenom,nom;
prenom = "Leslie";
nom = "Pencuir";
```

### Chaînes de caractères

* entre `"`
* concaténés par des `+`

## Fonctions

### Ecrire une fonction

* peuvent recevoir des arguments en entrée
* peuvent retourner une valeur

#### Exemple

```javascript
function squareRoot(nombre) {
  return Math.sqrt(nombre);
}
```

_NB : Utilisation de l'objet `Math`_

## Quelques fonctions utiles

## Structures

### Boucles

#### for

exécuté pour i = 0, 1, 2, 3, 4, soit 5 fois

```javascript
for (i=0; i<5; i++)
{
  //code
}
```

#### while

exécuté tant que la condition est vraie

```javascript
while (a<b)
{
  //code
}

```

## Evenements

event |
--- | ---
`onload` | après le chargement de la page
`onclick` | lors d'un clic
`onmousemove` | lorsque la souris se déplace
...

#### Exemple

```html
<h1 onmouseover="alert('Vous venez de survoler mon super titre');">Mon super titre</h1>
```
## Ajout

### Directement dans le html ...

```html
<button onclick="maSuperAlerte()">Mon bouton</button>
<script>
function maSuperAlerte() {
  alert('What a magnifique boite de dialogue...');
}
</script>
```

### Dans un fichier à part

#### alert.js

```javascript
function maSuperAlerte() {
  alert('What a magnifique boite de dialogue...');
}
```

#### index.html

```html
<!doctype html>
<html lang="fr">
  <head>
    <script src="js/alert.js"></script>
  </head>
  <body>
    ...
    <button onclick="maSuperAlerte()">Mon bouton</button>
    ...
  </body>
</html>
```

## Rédaction de votre code

- Toujours bien __terminer__ une instruction par un ;

- Garder un code propre bien `indenté` (pour faciliter la relecture)

- Attention aux portées des variables

- Donner des noms compréhensibles

- Ne pas hésiter à commenter
	* html `<!-- mon commentaire -->`
	* css ` /* mon commentaire */`
	* js ` // mon commentaire`

- Ne pas __abuser__ du copier/coller

### Conventions

blabla

[Retour au cours](../cours.md)
