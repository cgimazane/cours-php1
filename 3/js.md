[Retour au cours](../cours.md)

# 3.1 js

## Introduction

### Définition

JavaScript

### Mots-clés

JavaScript est un __langage orienté objet__ interprété par le navigateur, sensible à la casse.

Il a pour but de dynamiser les sites Internet.

### Présentation rapide

Dans notre page Web, on a un objet `window` contenant (entre autres) un objet `document` qui contient lui-même tous les éléments html de la page (paragraphes, tableaux...).

## Présentation du langage

### Variables

* Pas de typage des variables
* Déclaration d'une variable par le mot-clé `var`
* Types existants :
	- string
	- number
	- array
	- boolean
	- object

#### Exemple

```javascript
var age = 12;
var prenom,nom;
prenom = "Leslie";
nom = "Pencuir";
document.getElementById("bienvenue").innerHTML = "Bienvenue " + prenom + " " + nom + " !";
```

### Chaînes de caractères

* entre `"`
* concaténées par des `+`

## Fonctions

### Ecrire une fonction

* peuvent recevoir des arguments en entrée
* peuvent retourner une valeur

#### Exemple

```javascript
function cube(nombre) {
  return nombre * nombre * nombre;
}
```

## Quelques fonctions utiles

d |	f
--- | ---
Tableau | `pop()`, `push()`, `shift()`, ...
String | `length`, `indexOf()`, ...
Numbers | `parseInt()`, `Math.pow()`, ...

Et d'autres...

## Structures

### Conditionelles

```javascript
if (var1==var2)
{
  //code
}else{
  //code
}
```

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

event | def
--- | ---
`onload` | après le chargement de la page
`onclick` | lors d'un clic
`onmousemove` | lorsque la souris se déplace

Et bien d'autres...

#### Exemple

```html
<h1 onmouseover="alert('Vous venez de survoler mon super titre');">Mon super titre</h1>
```

On peut également utiliser `addEventListener`

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

- Utilisation du camelCase pour nommer variables et fonctions

[Retour au cours](../cours.md)
