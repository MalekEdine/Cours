
# Cours de Java : Les Bases

## Table des Matières
1. [Introduction à Java](#introduction-à-java)
2. [Les Types de Données](#les-types-de-données)
3. [Les Variables](#les-variables)
4. [L'Affectation](#laffectation)
5. [Les Conditions : `if` et `else`](#les-conditions--if-et-else)
6. [Les Instructions `switch case`](#les-instructions-switch-case)
7. [Les Boucles `for`](#les-boucles-for)
8. [Les Fonctions](#les-fonctions)

---

## Introduction à Java
Java est un langage de programmation orienté objet et fortement typé. Il est utilisé pour développer des applications de bureau, mobiles, et web. Les programmes Java sont compilés en bytecode, qui peut être exécuté sur toute machine virtuelle Java (JVM), ce qui rend le langage très portable.

---

## Les Types de Données

En Java, il existe différents types de données qui peuvent être utilisés pour déclarer des variables :

### Types Primitifs
- **`int`** : Représente les entiers (32 bits).
- **`long`** : Représente les grands entiers (64 bits).
- **`float`** : Représente les nombres à virgule flottante (32 bits).
- **`double`** : Représente les nombres à virgule flottante de précision double (64 bits).
- **`char`** : Représente un caractère (16 bits).
- **`boolean`** : Représente une valeur booléenne (`true` ou `false`).

### Types Référencés
- **`String`** : Représente une chaîne de caractères.
- **Tableaux (`array`)** : Représentent une collection d'éléments de même type.

---

## Les Variables

Les variables sont utilisées pour stocker des données en mémoire. En Java, une variable doit être déclarée avant d'être utilisée.

### Déclaration et Initialisation
```java
int age; // Déclaration d'une variable entière
age = 25; // Initialisation de la variable

// Déclaration et initialisation en une ligne
String nom = "Jean";
```

### Conventions de Nommage
- Les noms de variables commencent par une lettre minuscule.
- Les noms peuvent contenir des lettres, des chiffres, des tirets bas `_`, mais ne doivent pas commencer par un chiffre.
- Utiliser le camelCase pour nommer les variables, par exemple `maVariable`.

---

## L'Affectation

L'affectation consiste à donner une valeur à une variable à l'aide de l'opérateur `=`.

### Exemples d'Affectation
```java
int nombre = 10;
double temperature = 36.5;
boolean estVrai = true;
char lettre = 'A';
```

L'opérateur `=` prend la valeur à droite et la stocke dans la variable à gauche.

---

## Les Conditions : `if` et `else`

Les conditions permettent d'exécuter du code en fonction de certaines conditions.

### Structure de base
```java
if (condition) {
    // Code exécuté si la condition est vraie
} else {
    // Code exécuté si la condition est fausse
}
```

### Exemple
```java
int age = 20;
if (age >= 18) {
    System.out.println("Vous êtes majeur.");
} else {
    System.out.println("Vous êtes mineur.");
}
```

### Opérateurs de Comparaison
- `==` : Égal à
- `!=` : Différent de
- `>` : Supérieur à
- `<` : Inférieur à
- `>=` : Supérieur ou égal à
- `<=` : Inférieur ou égal à

### Opérateurs Logiques
- `&&` : ET logique
- `||` : OU logique
- `!` : NON logique

---

## Les Instructions `switch case`

L'instruction `switch` permet de choisir parmi plusieurs options en fonction de la valeur d'une variable.

### Structure de base
```java
switch (expression) {
    case valeur1:
        // Code exécuté si expression == valeur1
        break;
    case valeur2:
        // Code exécuté si expression == valeur2
        break;
    default:
        // Code exécuté si aucune des valeurs ne correspond
}
```

### Exemple
```java
int jour = 2;
switch (jour) {
    case 1:
        System.out.println("Lundi");
        break;
    case 2:
        System.out.println("Mardi");
        break;
    case 3:
        System.out.println("Mercredi");
        break;
    default:
        System.out.println("Jour inconnu");
}
```

---

## Les Boucles `for`

Les boucles permettent d'exécuter du code plusieurs fois.

### Structure de base
```java
for (initialisation; condition; incrémentation) {
    // Code exécuté à chaque itération
}
```

### Exemple
```java
for (int i = 0; i < 5; i++) {
    System.out.println("Itération " + i);
}
```

Dans cet exemple, la boucle s'exécute 5 fois, de `i = 0` à `i < 5`.

---

## Les Fonctions

Les fonctions (ou méthodes) permettent de regrouper du code réutilisable.

### Définition d'une Fonction
```java
public static int addition(int a, int b) {
    return a + b;
}
```

### Appel d'une Fonction
```java
int resultat = addition(5, 10);
System.out.println("Le résultat est : " + resultat);
```

### Types de Retour
- Une fonction peut retourner un type (`int`, `double`, `String`, etc.) ou `void` si elle ne retourne rien.

### Paramètres de Fonction
Les paramètres permettent de passer des valeurs à la fonction. Par exemple, `int a` et `int b` dans l'exemple ci-dessus.

---

## Conclusion

Ce cours couvre les bases de Java. Pour aller plus loin, explorez les concepts tels que les classes, les objets, l'héritage, les interfaces, et la gestion des exceptions.
