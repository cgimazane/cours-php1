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
``

[Retour au cours](cours.md)
