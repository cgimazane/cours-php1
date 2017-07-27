[Retour au cours](cours.md)

# php

Langage qui peut être inséré dans les fichiers html dans des balises

```php
<?php ?>
```

## Variables

* Pas de typage des variables
* Identificateur avec un `$` au début (exemple : `$toto`)
* Types existants :
  - integer `$age = 12;`
  - string `$nom = 'toto';`
  - float `$taille = '1.76';`
  - array
  - boolean `$open = true`
  - object

### Chaînes de caractères

* entre `'`
* concaténés par des `.`

### Variables d'environnement

contenues dans `$_SERVER` (variable superglobale);

=> Tester la fonction `phpinfo()`

## Quelques fonctions utiles

d |  f
--- | ---
Fichiers | `include()`/`require()` (_once), ...
Tableau | `in_array()`, `array_gnagna()`, `sort()`, ...
String | `str_gnagna()`, `trim()`, ...
Mixed | `count()`, `gettype()`, `implode()`/`explode()`, `empty()`, `isset()`/`unset()`

Et bien d'autres...

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

## Fonctions

### Ecrire une fonction

* peuvent recevoir des arguments en entrée
* peuvent retourner un valeur
* travaillent sur des copies (on peut forcer par référence avec ```&```)
* return

Exemple :

```
function concat($str1, $str2 = 'rajout') {
     return $str1.$str2;
}
```

=> Ecrire une fonction qui prend en entrée 2 entiers et qui retourne le produit divisé par la somme. L'appeler.

---

## Bases de données & SQL

---


### Rappels ?

* CREATE, SELECT, INSERT ...
* ORDER BY ...
* JOIN ...

---

### Remplissage de la bdd

* utilisation script sql

---

## Les formulaires

* html
* des nouvelles balises

---

### Fonctionnement

1. l'utilisateur entre ses données
2. il appuie sur valider
3. le traitement est déclenché
4. les données sont retournées (à l'utilisateur ou à la bdd) après traitement

---

### Les balises

* ```<form>```
 - attribut ```action``` : la page php contenant le traitement
 - attribut ```method``` : GET (paramètres dans la barre d'adresse) ou POST (paramètres cachés)
* ```<input>```
 - type ```text```
 - type ```password```
 - type ```radio```
 - type ```checkbox```
 - type ```select``` et ses ```option```
 - type ```textarea```
 - type ```submit```
 - type ```hidden```

=> On fait un formulaire de calcul du volume pour un parallélipède rectangle

---

### Autour des formulaires

* autres types d'input
* label (spécification)
* fieldset (regroupement)

---

[Retour au cours](cours.md)
