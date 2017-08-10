[Retour au cours](../cours.md)

# 2.1 css

## Introduction

### Définition

Cascading Style Sheets

### Mots-clés

Un __style__ css est composé de :

* un __sélecteur__
* des __règles__
	- à mettre entre { }
	- à terminer par un ;

#### Exemple

```css
h1 {
  font-family: Arial;
  color: #0f5;
}
```

## Les sélecteurs

### Sélecteur simple

* on sélectionne tous les éléments `h1`

```css
h1 {

}
```
* on sélectionne l'élément identifié `<div id="boite"></div>` dans la page

```css
#boite {

}
```
* on sélectionne tous les éléments identifiés `<div class="menu"></div>` dans la page

```css
.menu {

}
```

### Sélecteur multiple

* on sélectionne tous les éléments `h1` et tous les éléments `span`

```css
h1, span {

}
```

### Sélecteur hiérarchique

* on sélectionne tous les éléments `span` contenu dans un élément `h1`

```css
h1 span {

}
```

## Les propriétés

* Couleur : `color`, `background-color`
* Textes :
	- police : `font-family`
	- taille : `font-size`
	- graisse : `font-weight`
	- alignement : `text-align`
* Dimensions : `width`, `height`
* Bordures : `border`
* Marges
	- internes : `padding`
	- externes : `margin`
* Transparence

### Le positionnement `position`

* `static` est la valeur par défaut de tous les éléments
* `relative` se comporte de la même façon que `static` mais les propriétés `top`, `right`, `bottom` et `left` vont le déplacer
* `fixed` est positionné par rapport a la fenêtre du navigateur, ce qui signifie qu'il reste toujours à la même place même si la page défile
* `absolute` se comporte comme `fixed` mais par rapport à l'élément parent le plus proche

Possibilté de faire flotter (en les sortant du flux) des éléments avec `float` 

## Les pseudo-trucs

- pseudo-classes
	+ `:hover`
	+ `:nth-child()`

- pseudo-éléments
	+ `::firstletter`
	+ `::after`

## Les fonctions

- `transform()`

- `rotate()`

- `linear-gradient()`

## Utilité

* Création d'interfaces nombreuses
* Création de sites adaptatifs

## Ajout

### Directement dans le html ...

```html
<div style="border-top: 3px double #0000ff;border-bottom: 1px solid #ff0000;color: #00ff00;">Ma div</div>
```

### Dans un fichier à part

#### style.css

```css
#maDiv {
  border-top: 3px double #0000ff;
  border-bottom: 1px solid #ff0000;
  color: #00ff00;
}
```

#### index.html

```html
<!doctype html>
<html lang="fr">
  <head>
    <link rel="stylesheet" href="css/style.css">
  </head>
  <body>
    ...
    <div id="maDiv">Ma div</div>
    ...
  </body>
</html>
```

## Rédaction de votre code

- Toujours bien __terminer__ un style par un ;

- Garder un code propre bien `indenté` (pour faciliter la relecture)

- Donner des noms compréhensibles

- Ne pas hésiter à commenter
	* html `<!-- mon commentaire -->`
	* css ` /* mon commentaire */`

- Ne pas __abuser__ du copier/coller

- Une seule déclaration par ligne

[Retour au cours](../cours.md)
