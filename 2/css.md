[Retour au cours](../cours.md)

# css

## Introduction

### Définition

Cascading Style Sheets

### Mots-clés

Un style css est composé de :

* un sélecteur
* des règles
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

* on peut sélectionner tous les éléments `h1`

```css
h1 {

}
```
* on peut sélectionner un élément identifié `<div id="boite"></div>` dans la page

```css
#boite {

}
```
* on peut sélectionner tous les éléments identifiés `<div class="menu"></div>` dans la page

```css
.menu {

}
```

### Sélecteur multiple

* on peut sélectionner tous les éléments `h1` et tous les éléments `span`

```css
h1, span {

}
```

### Sélecteur hiérarchique

* on peut sélectionner tous les éléments `span` contenu dans un élément `h1`

```css
h1 span {

}
```
## Les pseudo-trucs

- pseudo-classes : `:hover`, `:nth-child()` ...

- pseudo-éléments : `::firstletter`, `::after` ...

## Les propriétés

* Couleur : color, background-color
* Textes :
	- police : font-family
	- taille : font-size
	- graisse : font-weight
	- alignement : text-align
	- ...
* Dimensions : width, height
* Bordures
* Marges
	- internes : padding
	- externes : margin
* Positionnement
* Transparence
* ...

## Les fonctions

- `transform()`

- `rotate()`

- `linear-gradient()`

- ...

## Utilité

* Création d'interfaces nombreuses
* Création de sites adaptatifs

## Référencement

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
