[Retour au cours](../cours.md)

# Les formulaires

## Introduction

### Définition

Interaction entre un utilisateur et un site

### Mots-clés

* html & php
* des nouvelles balises

## Fonctionnement

1. l'utilisateur entre ses données
2. il les envoie
3. le traitement est déclenché
4. les données sont retournées (à l'utilisateur ou à la bdd) après traitement

## Rédaction

### Les balises

- formulaire : `<form></form>`
  * method : par quel moyen les données vont être envoyées
    - GET (paramètres dans la barre d'adresse)
    - POST (paramètres cachés)
  * name
  * action : la page php contenant le traitement
- champ de saisie : `<input />`
  * type
    - `text`
    - `password`
    - `radio`
    - `checkbox`
    - `select` et ses `option`
    - `textarea`
    - `submit`
    - `hidden`
  * name
- liste d'options :
  - `<select></select>`
  - `<option></option>`
  - `<optgroup></optgroup>`

_NB : unicité de l'attribut name_

### Autour des formulaires

* autres types d'input

* label (spécification)
  - `<label></label>`

* fieldset (regroupement)
  - `<fieldset></fieldset>`

### Attributs utiles

 - selected
 - checked
 - disabled
 - readonly

#### Exemple

 ```html
  <form action="result.php" method="POST">
    <input type="text" name="name" placeholder="Nom" />
    <label for="age">Age :
      <input type="number" name="age" min="1" />
    </label>
    <input type="submit" value="Submit" />
  </form>
```

## Récupération

Il faut donc récupérer les données envoyées par l'utilisateur.

On sait où les récupérer `$_GET`, `$_POST` ou `$_FILES` grâce à l'attribut `method`

On va donc effectuer le traitement dans la page `result.php`

#### Exemple

```php
$now = new DateTime();
$year = $now->format("Y");

$birthYear = $year - $_POST['age'];

$txt = $_POST['nom'];
$txt .= ' est né en ';
$txt .= $birthYear;
```

[Retour au cours](../cours.md)
