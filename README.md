# TP : Utilisation de Fetch et Affichage Dynamique des Données

## 1. Rappel : Sélecteurs et Événements en JavaScript

### Sélecteurs de base

En JavaScript, on peut sélectionner des éléments HTML avec différentes méthodes :

- `document.getElementById("id")` : sélectionne un élément par son ID.
- `document.querySelector(".classe")` : sélectionne le premier élément correspondant au sélecteur CSS.
- `document.querySelectorAll("div")` : sélectionne tous les éléments correspondants sous forme de `NodeList`.
- `document.getElementsByClassName("classe")` : sélectionne tous les éléments d'une classe (HTMLCollection).
- `document.getElementsByTagName("tag")` : sélectionne tous les éléments d'un type donné.

Exemple :
```js
const bouton = document.getElementById("monBouton");
const elements = document.querySelectorAll(".liste-elements");
```

### Gestion des événements

Les événements permettent d'interagir avec l'utilisateur :

- click : déclenché lors d'un clic.
- change : déclenché lors d'un changement de valeur dans un champ.
- input : déclenché lorsqu'un utilisateur saisit du texte.

#### Ajout d'un événement :

```js
Copier
Modifier
const bouton = document.getElementById("monBouton");

bouton.addEventListener("click", () => {
    alert("Bouton cliqué !");
});
```
## 2. TP : Tester Fetch et Afficher les Données

### Objectif
L'objectif est de récupérer et afficher des données depuis une API en utilisant fetch, ainsi que de permettre des interactions via des boutons et des formulaires.

### Étapes
#### Récupération des données

- À l'aide de fetch, récupérer des posts, des utilisateurs et des tâches depuis JSONPlaceholder.
- Afficher ces données dans des div spécifiques en les structurant sous forme de cartes.

#### Affichage des données

- Mettre à jour le DOM en insérant les résultats sous forme de listes ou de cartes.
- Ajouter un indicateur de chargement lors des requêtes.

#### Ajout d'un post

- Compléter un formulaire avec title, body et userId.
- Envoyer ces données en POST avec fetch.
- Afficher la réponse retournée.

#### Mise à jour et suppression

- Modifier un post existant via PUT.
- Supprimer un post via DELETE.

#### Contraintes
- Utiliser async/await pour gérer les requêtes asynchrones.
- Gérer les erreurs en affichant des messages appropriés.
- Nettoyer les anciennes données avant d'afficher les nouvelles
- Séparez votre code en fichiers distinct
- Créés plusieurs fichiers JS et importez vos fonctions
