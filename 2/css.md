[Retour au cours](../cours.md)

# css

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
* Positionnement
* Transparence

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

## Référencement
html 
code

link

## Rédaction de votre code

- Toujours bien __terminer__ un style par un ;

- Garder un code propre bien `indenté` (pour faciliter la relecture)

- Donner des noms compréhensibles

- Ne pas hésiter à commenter
	* html `<!-- mon commentaire -->`
	* css ` /* mon commentaire */`

- Ne pas __abuser__ du copier/coller

### Conventions

* une déclaration par ligne
* utiliser des minuscules pour les couleurs

[Retour au cours](../cours.md)
