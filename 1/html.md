[Retour au cours](../cours.md)

# html

## Introduction

### Définition

HyperText Markup Language

### Mots-clés

Un __élément__ html	:

* est représenté par des __balises__
* peut avoir des __attributs__

## Les bases du html

### Les balises

* elles définissent un rôle (et pas de mise en forme)
* elles sont écrites en minuscules
* elles s'ouvrent et se referment
* elles peuvent avoir des attributs ( `"` est utilisé pour définir les valeur des attributs )
* elles sont de deux types
	- "bloc" : elles créent un bloc "autonome"
	- en ligne : elles servent à donner de l'intérêt à ce qu'elles concernent

#### Exemples

* un paragraphe

```html
<p>quel beau paragraphe !</p>
```

* un lien

```html
<a href="http://www.ign.fr">lien vers ign</a>
```

* un saut de ligne

```html
<hr />
```

* autre :

```html
<div>wow ma <strong>magnifique</strong> div !</div>
```

### La page de base

```html
<!doctype html>
<html lang="fr">
  <head>
    <meta charset="utf-8">
    <title>Titre de la page</title>
  </head>
  <body>
    <!-- Le contenu de votre page -->
  </body>
</html>
```

* doctype
* html avec un attribut (zone racine)
	- head (entête contenant les metadonnées)
		+ meta
		+ title
	- body
		+ le contenu du document

Existence de standards à respecter.

### Liste de balises bloc (non-exhaustive)

* les blocs "neutres" : `<div>blabla</div>` : pour désigner les différentes parties du document
* les titres : `<h1>Mon super titre</h1>` (h2, ..., h6) : pour organiser la page
* les paragraphes : `<p>ouh encore un beau paragraphe !</p>`
* les listes : `<ul>` (non-numérotée) ou `<ol>` (numérotée)
* les éléments de listes : `<li>`
* les tableaux : `<table>`
	- avec des lignes : `<tr>`
	- avec des cellules : `<td>`

Et d'autres...

### Liste de balises en ligne

* `<strong>` , `<em>` : accentuation
* `<a>` : les liens
	- href : destination du lien
* `<img>`
* `<span>` : l'équivalent de div

Et d'autres encore...

### Liste d'attributs standards
* `class` : pour définir les classes de l'objet que l'on utilisera plus tard
* `id` : pour donner un identifiant unique à une balise
* `title` : permet de donner un titre pour un objet
* `style` : permet d'intégrer un style css à l'objet

## Rédaction de votre code

- Toujours bien vérifier que si une balise est ouverte, elle __doit__ être fermée

- Certaines balises sont __auto-fermantes__ (`<img />`, `<br />`)

- Garder un code propre bien `indenté` (pour faciliter la relecture)

- Ne pas hésiter à commenter
	* html `<!-- mon commentaire -->`

- Ecrire le contenu de la page dans le corps du document (`<body></body>`)

- Remplir correctement l'entête (`<head></head>`) de votre document

- Ne pas __abuser__ du copier/coller

[Retour au cours](../cours.md)
