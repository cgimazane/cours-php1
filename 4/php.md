[Retour au cours](../cours.md)

# 4.1 php

## Introduction

### Définition

PHP Hypertext Preprocessor

### Mots-clés

Dynamisation du site

* __traitement__ des données

* récupération des données dans la __bdd__

* possibilité d'__automatisation__

## Utilisation

```php
<?php
  // mon code
?>
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
* concaténées par des `.`

### Variables superglobales

Variables internes qui sont toujours disponibles, quel que soit le contexte

* variables d'environnement : `$_SERVER`
* paramètres d'url : `$_GET`

Et d'autres...

## Fonctions

### Ecrire une fonction

* peuvent recevoir des arguments en entrée
* peuvent retourner une valeur
* travaillent sur des copies (on peut forcer par référence avec `&`)

#### Exemple :

```php
  function concat($str1, $str2 = 'rajout') {
    return $str1.$str2;
  }
```

## Quelques fonctions utiles

d |	f
--- | ---
Fichiers | `include()`/`require()` (_once), ...
Tableau | `in_array()`, `array_gnagna()`, `sort()`, ...
String | `str_gnagna()`, `trim()`, ...
Mixed | `count()`, `gettype()`, `implode()`/`explode()`, `empty()`, `isset()`/`unset()`

Et bien d'autres...

## Structures

### Conditionelles

```php
if (condition_a){
  //code
}elseif(condition_b){
  //code
}else{
  //code
}
```
### Boucles

#### for

exécuté pour i = 0, 1, ... , 9, soit 10 fois

```php
for( $i=0; $i<10; $i++ ) {
  //code
}
```

#### while

exécuté tant que la condition est vraie

```php
while( condition ) {
  // code à exécuter tant que la condition est vraie
}
```

## Bases de données

## Rappels SQL

* CREATE, SELECT, INSERT
* ORDER BY
...

### Remplissage de la bdd

Créer les tables et les remplir.

## Connexion

PDO : Php Data Objects

### Création

```php
try {
  $strConnection = 'pgsql:host=localhost;dbname=php1';
  $db = new PDO($strConnection, user, password);
}catch(PDOException $e) {
  $msg = 'ERREUR PDO dans ' . $e->getFile() . ' L.' . $e->getLine() . ' : ' . $e->getMessage();
  die($msg);
}
```

### Utilisation

```php
/** 1er type de requete **/
$query = 'SELECT * FROM personne;';

$stmt = $db->query($query);

$allResults = $stmt->fetchAll();

/** 2nd type de requete **/
$query = 'DELETE FROM personne WHERE nom="Honnette";';

$rowCount = $db->exec($query);

/** 3eme type de requete **/
$query = 'SELECT * FROM personne WHERE nom=:nom LIMIT :limite;';

$prep = $db->prepare($query);

$prep->bindValue(':limite', 1 );
$prep->bindValue(':nom', "Patamob" );

$prep->execute();

$allResults = $prep->fetchAll();
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
	* php ` // mon commentaire`

[Retour au cours](../cours.md)
