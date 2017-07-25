# Introduction

## Mise en situation

Langages utlisés :

* html ( Hypertext Markup Language )
* css ( Cascading Style Sheets )
* php ( PHP: Hypertext Preprocessor )

Machines utilisées :

* un client
* un serveur

Logiciels utilisés :

* un navigateur
* un serveur web
* un éditeur de texte
* un sgbd
* ...

## Présentation fonctionnement site

### Site statique

Le site est une simple page que l'utilisateur peut lire et avec laquelle il n'aura aucune interaction.

### Site dynamique

Existence de sites dynamiques qui vont "communiquer" avec l'uilisateur

## Remarque importante

Vous n'êtes pas seul à lire votre code : bien indenter et commenter son code

# Les langages

## html

C'est un __standard__

C'est le __"fond"__ du document

* description de données
* structuration de la page
* organisation de contenu
* utilisation de html5

_NB : Langage interprété par le navigateur_

## css

C'est un standard

C'est la __"forme"__ du document

* mise en forme des données
  - couleur
  - taille
  - police
* indépendant du html

_NB : Langage interprété par le navigateur_

## Démonstration

Dans votre navigateur, taper www.csszengarden.com/cdn avec cdn < 222

Exemples : 191, 209, 167, 126, 112, 048, 012, 001

## php

* poo
* page dynamique
  - tests
  - boucles
  - fonctions
  - ...

_NB : Langage traité par le serveur_


# Mise en place (et vérification) de l'environnement

WAMP

* Windows (environnement)
* Apache (serveur web)
* MySql (serveur de base de données)
  - que l'on remplacera par PostgreSQL
* PHP (scripts)


# html

## Les bases du html

### Les balises

* elles définissent un rôle (et pas de mise en forme)
* elles ont les noms écrits en minuscules
* elles s'ouvrent et se referment
* elles peuvent avoir des attributs ( ```"``` est utilisé pour définir les valeur des attributs )
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
    <link rel="stylesheet" href="style.css">
  </head>
  <body>
    ...
    <!-- Le contenu de votre page -->
    ...
  </body>
  </html>
  ```

* doctype
* html avec un attribut (zone racine)
  - head (entête contenant les metadonnées)
    + meta
    + title
    + link
  - body
    + le contenu du document

Existence de standards à respecter.

### Liste de balises bloc (non-exhaustive)

* les blocs "neutres" : ```<div>blabla</div>``` : pour désigner les différentes parties du documents
* les titres : ```<h1>Mon super titre</h1>``` (h2, ..., h6) : pour organiser la page
* les paragraphes : ```<p>ouh encore un beau paragraphe !</p>```
* les listes : ```<ul>``` (non-numérotée) ou ```<ol>``` (numérotée)
* les éléments de listes : ```<li>```
* les tableaux : ```<table>```
  - avec des lignes : ```<tr>```
  - avec des cellules : ```<td>```
* ...

### Liste de balises en ligne

* ```<strong>``` , ```<em>``` : accentuation
* ```<a>``` : les liens
  - href : destination du lien
* ```<img>```
* ```<span>``` : l'équivalent de div
* ...

# Le projet

Tout au long de la session, réalisation d'un projet sur votre équipe

## Généralités

### Qui est un bon développeur ?

Tout bon développeur prend le temps d'organiser et de commenter son code

Tout bon développeur sait limiter le nombre de caractères qu'il a à écrire

Tout bon développeur ne reste pas dans son coin sans chercher (sur Internet au pire)

Tout bon développeur sait chercher intelligemment de l'aide sur le web

### Rédaction de votre code

- Toujours bien vérifier que si une balise est ouverte, elle __doit__ être fermée

- Certaines balises sont __auto-fermantes__ (`<img />`, `<br />`)

- Toujours bien __terminer__ un style par un ;

- Garder un code propre bien `indenté` (pour faciliter la relecture)

- Ne pas hésiter à commenter
  * html `<!-- mon commentaire -->`
  * css ` /* mon commentaire */`

- Ecrire le contenu de la page dans le corps du document (`<body></body>`)

- Remplir correctement l'entête (`<head></head>`) de votre document
  * titre
  * encodage
  * auteur
  * ...

- Ne pas __abuser__ du copier/coller

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

## Première page

* Création d'une page avec la présentation de votre équipe


# css

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

* on peut sélectionner tous les éléments h1

```css
h1 {

}
```
* on peut sélectionner un élément identifié ```<div id="boite"></div>``` dans la page

```css
#boite {

}
```
* on peut sélectionner un élément identifié ```<div class="menu"></div>``` dans la page

```css
.menu {

}
```

### Sélecteur multiple

* on peut sélectionner un élément h1 ou un élément span

```css
h1, span {

}
```

### Sélecteur hiérarchique

* on peut sélectionner un élément span dans un élément h1

```css
h1 span {

}
```

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

## Utilité

* Création d'interfaces nombreuses
* Création de sites adaptatifs


# Amélioration de notre page

* Reprise de la page avec la présentation de votre équipe (deux fois mieux)

---

# PHP

Langage inséré dans les fichiers html dans des balises

```php
<?php ?>
```

## Variables

* Pas de typage des variables
* Identificateur avec un ```$``` au début (exemple : ```$toto```)
* Types existants :
  - integer ```$age = 12;```
  - string ```$nom = 'toto';```
  - float ```$taille = '1.76';```
  - array
  - boolean ```$open = true```
  - object

### Chaînes de caractères

* entre ```'```
* concaténés par des ```.```

## Structures

### Conditionelles

```php
<?php
	if (condition_a){
		//code
	}elseif(condition_b){
		//code
	}else{
		//code
	}
?>
```
### Boucles

#### for (exécuté pour i = 0, 1, ... , 9, soit 10 fois)

```php
<?php
	for( $i=0; $i<10; $i++ ) {
		 //code
	}
?>
```

#### while

```php
<?php
while( condition ) {
     // code à exécuter tant que la condition est vraie
}
?>
```
