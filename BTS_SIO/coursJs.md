# Syllabus JavaScript : 15 Séances de Formation

---

## Séance 1 : Introduction au JavaScript
**Objectifs** : Comprendre l’histoire de JavaScript, son utilité, et son intégration dans les pages web.
- Présentation de JavaScript, son histoire et sa place dans le développement web.
- Introduction aux concepts de base : HTML, CSS et JavaScript dans le contexte du navigateur.
- Structure d’un programme JavaScript.
- **Exercice** : Insérer JavaScript dans une page HTML avec des balises `<script>`.
- **TP** : Créer une première alerte ("Hello, World!") pour comprendre le fonctionnement basique de JavaScript dans le navigateur.

---

## Séance 2 : Les Variables et les Types de Données
**Objectifs** : Savoir déclarer et utiliser des variables, comprendre les différents types de données.
- Les variables : `var`, `let` et `const`.
- Types de données primitifs : `string`, `number`, `boolean`, `undefined`, `null`.
- **Exercice** : Déclarer des variables et expérimenter avec les différents types de données.
- **TP** : Créer un petit programme qui utilise différents types de variables pour afficher des informations sur l’utilisateur (nom, âge, est connecté).

---

## Séance 3 : Opérateurs et Expressions
**Objectifs** : Apprendre à manipuler les données avec des opérateurs.
- Opérateurs arithmétiques (`+`, `-`, `*`, `/`, `%`).
- Opérateurs de comparaison (`==`, `===`, `!=`, `!==`, `<`, `>`, `<=`, `>=`).
- Opérateurs logiques (`&&`, `||`, `!`).
- **Exercice** : Utiliser les opérateurs pour résoudre de petits problèmes de calcul.
- **TP** : Créer un programme de calculatrice simple avec des variables, qui additionne, soustrait, multiplie et divise deux nombres.

---

## Séance 4 : Les Structures de Contrôle : Les Conditions
**Objectifs** : Apprendre à contrôler le flux du programme avec des conditions.
- La structure `if`, `else if`, `else`.
- Les conditions imbriquées et l’opérateur ternaire.
- **Exercice** : Écrire des conditions pour vérifier l’âge d’un utilisateur et afficher un message personnalisé.
- **TP** : Créer un programme qui vérifie si un utilisateur peut accéder à un contenu selon son âge.

---

## Séance 5 : Les Boucles
**Objectifs** : Apprendre à répéter des actions avec les boucles.
- Introduction aux boucles : `for`, `while`, et `do...while`.
- **Exercice** : Utiliser une boucle `for` pour afficher une série de nombres.
- **TP** : Créer un programme qui affiche la table de multiplication d’un nombre donné.

---

## Séance 6 : Les Fonctions
**Objectifs** : Comprendre l’utilité des fonctions et savoir les créer et les appeler.
- Déclaration d’une fonction avec `function`.
- Paramètres et valeurs de retour.
- Fonctions anonymes et fonctions fléchées (`=>`).
- **Exercice** : Créer des fonctions simples (saluer un utilisateur, additionner deux nombres).
- **TP** : Créer une fonction pour calculer la moyenne de trois notes d’un élève.

---

## Séance 7 : Manipulation des Tableaux
**Objectifs** : Savoir créer et manipuler des tableaux (arrays).
- Création et accès aux éléments d’un tableau.
- Boucles et tableaux : `for` et `for...of`.
- Méthodes de tableau importantes : `push()`, `pop()`, `shift()`, `unshift()`, `length`.
- **Exercice** : Créer un tableau et effectuer des manipulations de base.
- **TP** : Créer un programme qui enregistre des prénoms d’élèves et les affiche en ordre.

---

## Séance 8 : Manipulation des Objets
**Objectifs** : Introduction aux objets en JavaScript.
- Création et manipulation d’un objet.
- Accès et modification des propriétés.
- Boucles et objets : `for...in`.
- **Exercice** : Créer un objet représentant un élève avec des propriétés (nom, âge, classe).
- **TP** : Construire un programme qui affiche les informations de l’élève de manière dynamique.

---

## Séance 9 : Fonctions Avancées et Contexte (`this`)
**Objectifs** : Apprendre les concepts avancés des fonctions et comprendre le contexte `this`.
- Fonction constructeur pour créer des objets.
- Utilisation du mot-clé `this`.
- **Exercice** : Créer un constructeur pour des objets « Éleve » avec des méthodes.
- **TP** : Créer un constructeur « Éleve » avec des méthodes pour saluer et afficher les informations.

---

## Séance 10 : Introduction au DOM (Document Object Model)
**Objectifs** : Comprendre et manipuler le DOM avec JavaScript.
- Sélection d’éléments dans le DOM : `getElementById`, `querySelector`.
- Modifier le contenu et le style d’un élément.
- **Exercice** : Sélectionner et modifier des éléments d’une page HTML.
- **TP** : Créer une page simple et manipuler le contenu du DOM en réponse à des actions utilisateur.

---

## Séance 11 : Événements en JavaScript
**Objectifs** : Gérer les événements pour interagir avec l’utilisateur.
- Les principaux événements : `click`, `mouseover`, `keydown`, `keyup`.
- Gestion d’événements avec `addEventListener`.
- **Exercice** : Créer des boutons avec des événements pour afficher des messages.
- **TP** : Créer un jeu de clic simple, où un message s’affiche à chaque clic sur un bouton.

---

## Séance 12 : Manipulation Avancée du DOM et Création d’Éléments
**Objectifs** : Créer et manipuler dynamiquement des éléments HTML.
- Créer, ajouter, supprimer des éléments avec `createElement`, `appendChild`, `removeChild`.
- **Exercice** : Ajouter dynamiquement une liste de courses sur la page.
- **TP** : Créer une mini-application de « to-do list » avec des éléments ajoutés et supprimés au clic.

---

## Séance 13 : Gestion du Local Storage
**Objectifs** : Stocker et récupérer des données dans le `localStorage`.
- Introduction au `localStorage` et `sessionStorage`.
- Stocker, récupérer, et supprimer des données.
- **Exercice** : Sauvegarder des préférences d’un utilisateur.
- **TP** : Améliorer la « to-do list » pour qu’elle soit sauvegardée dans le `localStorage`.

---

## Séance 14 : Introduction à la Programmation Asynchrone avec les Promesses
**Objectifs** : Découvrir la gestion asynchrone en JavaScript.
- Concepts de base : synchronisation vs asynchronisation.
- Introduction aux promesses : création et utilisation.
- **Exercice** : Simuler une requête asynchrone.
- **TP** : Créer une fonction simulant un chargement de données avec une promesse.

---

## Séance 15 : Introduction à Fetch et API REST
**Objectifs** : Apprendre à faire des requêtes HTTP pour obtenir des données d’une API.
- Utiliser `fetch` pour récupérer des données.
- Gérer les réponses avec `then` et `catch`.
- **Exercice** : Utiliser `fetch` pour obtenir des données d’une API publique.
- **TP** : Créer une application simple qui affiche des informations météorologiques d’une API.

---

## Projet Final
**Objectifs** : Consolidation de tous les acquis.
- Les élèves choisissent un projet : une mini-application de météo, un gestionnaire de tâches, ou un portfolio interactif.
- **Exigences** : Utilisation du DOM, des événements, du `localStorage`, et de `fetch`.
- **Présentation** : Chaque élève présente son projet final.

---
