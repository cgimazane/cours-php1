[Retour au cours](../cours.md)

# php

## Introduction

### Définition

PHP Hypertext Preprocessor

### Mots-clés

Fonctions variables

## Utilisation

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

### Variables superglobales

Variables internes qui sont toujours disponibles, quel que soit le contexte

* variables d'environnement : `$_SERVER`
* paramètres d'url : `$_GET`

Et d'autres...

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

#### for

exécuté pour i = 0, 1, ... , 9, soit 10 fois

```php
<?php
  for( $i=0; $i<10; $i++ ) {
    //code
  }
?>
```

#### while

exécuté tant que la condition est vraie

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
* peuvent retourner une valeur
* travaillent sur des copies (on peut forcer par référence avec `&`)
* return

Exemple :

```
  function concat($str1, $str2 = 'rajout') {
    return $str1.$str2;
  }
```

## Bases de données & SQL

## Rappels ?

* CREATE, SELECT, INSERT ...
* ORDER BY ...
* JOIN ...

### Remplissage de la bdd

* utilisation script sql

## Connexion

PDO : Php Data Objects

### Création


```
<?php
try {
$strConnection = 'mysql:host=localhost;dbname=php2';
$db = new PDO($strConnection, 'root', '');
}
catch(PDOException $e) {
    $msg = 'ERREUR PDO dans ' . $e->getFile() . ' L.' . $e->getLine() . ' : ' . $e->getMessage();
    die($msg);
}
```

### Utilisation

```
<?php
//requete #1
$query = 'SELECT * FROM person;';

$stmt = $db->query($query);

$allResults = $stmt->fetchAll();

//requete #2
$query = 'DELETE FROM person WHERE id=1;';

$rowCount = $pdo->exec($query);

//requete #3
$query = 'SELECT * FROM person WHERE name=:nom LIMIT :limite;';

$prep = $pdo->prepare($query);

$prep->bindValue(':limite', 10);
$prep->bindValue(':nom', $name);

$prep->execute();

$allResults = $prep->fetchAll();

?>


[Retour au cours](../cours.md)
