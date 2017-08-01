[Retour au cours](../cours.md)

## Les formulaires

* html
* des nouvelles balises

---

### Fonctionnement

1. l'utilisateur entre ses données
2. il appuie sur valider
3. le traitement est déclenché
4. les données sont retournées (à l'utilisateur ou à la bdd) après traitement

---

### Les balises

- formulaire : `<form></form>`
 * method : GET (paramètres dans la barre d'adresse) ou POST (paramètres cachés)
 * name
 * action : la page php contenant le traitement

- champ de saisie : `<input />`
 * type
		- type `text`
		- type `password`
		- type `radio`
		- type `checkbox`
		- type `select` et ses `option`
		- type `textarea`
		- type `submit`
		- type `hidden`
 * name
> un name est **unique** dans un form

- liste d'options : `<select></select>`
 * name

- `<option></option>`
 * value

- `<optgroup></optgroup>`
 * label

- `<label></label>`

- `<fieldset></fieldset>`

- `<legend></legend>`

- `<option></option>`


 ### Attributs utiles

 - selected
 - checked
 - disabled
 - readonly

 #### Exemple

 ```html
	<form action="#">
		<label for="filename">Nom du fichier :
			<input type="text" name="filename" placeholder="Nom du fichier" />
		</label>
		<input type="file" name="file" />
		<input type="submit" value="Submit" />
	</form>
```

---

### Autour des formulaires

* autres types d'input
* label (spécification)
* fieldset (regroupement)

[Retour au cours](../cours.md)
