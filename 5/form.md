[Retour au cours](../cours.md)

# Les formulaires

## Introduction

### Définition

c'est quoi un formulaire

### Mots-clés

* html
* des nouvelles balises

## Fonctionnement

1. l'utilisateur entre ses données
2. il appuie sur valider
3. le traitement est déclenché
4. les données sont retournées (à l'utilisateur ou à la bdd) après traitement

## Rédaction

### Les balises

- formulaire : `<form></form>`
  * method : GET (paramètres dans la barre d'adresse) ou POST (paramètres cachés)
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

 ### Autour des formulaires

* autres types d'input

* label (spécification)
  - `<label></label>`

* fieldset (regroupement)
  - `<fieldset></fieldset>`

_NB : unicité de l'attribut name_

 ### Attributs utiles

 - selected
 - checked
 - disabled
 - readonly

 #### Exemple

 ```html
  <form action="result.php" method="post">
    <label for="filename">Nom du fichier :
      <input type="text" name="filename" placeholder="Nom du fichier" />
    </label>
    <input type="file" name="file" />
    <input type="submit" value="Submit" />
  </form>
```

## Récupération

`$_POST`

[Retour au cours](../cours.md)
