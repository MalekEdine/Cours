### ** Le Design Pattern Factory**

---

#### **Introduction au Design Pattern Factory**

Le **Design Pattern Factory** (ou **Factory Method**) est l'un des **patrons de création** les plus couramment utilisés en programmation orientée objet. Il est conçu pour gérer et encapsuler la logique de création d'objets tout en permettant à une application de rester flexible face à des changements ou des extensions.

---

### **Objectif du Factory Pattern**
Le principal objectif est de **déléguer la création des objets** à une méthode dédiée ou à une classe spécialisée appelée **Factory**, plutôt que de la gérer directement dans le code principal. Cela permet :
- **Découplage** : Le code qui utilise les objets n’a pas besoin de connaître leurs classes concrètes.
- **Extensibilité** : Ajouter de nouveaux types d’objets est plus facile.
- **Simplification** : La logique complexe de création d’objets est centralisée.

---

### **Pourquoi utiliser le Factory Pattern ?**
1. **Réduction de la dépendance aux classes concrètes** : En encapsulant la logique de création, on travaille avec des interfaces ou des classes abstraites.
2. **Facilité d’ajout de nouvelles fonctionnalités** : Ajouter un nouveau type d'objet ne nécessite pas de modifier le code client.
3. **Respect des principes SOLID** :
   - **S**ingle Responsibility Principle : La logique de création est isolée dans une classe spécifique.
   - **O**pen/Closed Principle : Le système est ouvert à l’extension mais fermé à la modification.

---

### **Structure du Design Pattern Factory**

1. **Interface ou classe abstraite** : Définit les méthodes ou propriétés communes aux objets créés.
2. **Classes concrètes** : Implémentent ou héritent de l'interface ou classe abstraite.
3. **Classe Factory** : Contient une méthode dédiée à la création d'objets (souvent appelée `create` ou `make`).
4. **Code client** : Appelle la Factory pour obtenir des objets sans se soucier de leur classe concrète.

---

### **Diagramme UML**

```plaintext
+------------------+
|   Product        |  (Interface ou classe abstraite)
+------------------+
| + operation()    |
+------------------+
        ▲
        |
+------------------+     +------------------+
| ConcreteProductA |     | ConcreteProductB |
+------------------+     +------------------+
| + operation()    |     | + operation()    |
+------------------+     +------------------+
        ▲
        |
+------------------+
| Factory          |
+------------------+
| + create(type)   |
+------------------+
```

---

### **Exemple Simple : Création de Formes Géométriques**

#### **Étape 1 : Définir l'interface ou classe abstraite**
```java
// Interface commune pour toutes les formes
interface Forme {
    void dessiner();
}
```

#### **Étape 2 : Implémenter les classes concrètes**
```java
// Classe concrète : Cercle
class Cercle implements Forme {
    @Override
    public void dessiner() {
        System.out.println("Dessin d'un cercle");
    }
}

// Classe concrète : Rectangle
class Rectangle implements Forme {
    @Override
    public void dessiner() {
        System.out.println("Dessin d'un rectangle");
    }
}

// Classe concrète : Triangle
class Triangle implements Forme {
    @Override
    public void dessiner() {
        System.out.println("Dessin d'un triangle");
    }
}
```

#### **Étape 3 : Créer la Factory**
```java
// Classe Factory
class FormeFactory {
    public Forme creerForme(String type) {
        switch (type.toUpperCase()) {
            case "CERCLE":
                return new Cercle();
            case "RECTANGLE":
                return new Rectangle();
            case "TRIANGLE":
                return new Triangle();
            default:
                throw new IllegalArgumentException("Type de forme inconnu : " + type);
        }
    }
}
```

#### **Étape 4 : Utilisation dans le code client**
```java
public class Main {
    public static void main(String[] args) {
        FormeFactory factory = new FormeFactory();

        // Créer des formes via la Factory
        Forme cercle = factory.creerForme("CERCLE");
        Forme rectangle = factory.creerForme("RECTANGLE");
        Forme triangle = factory.creerForme("TRIANGLE");

        // Utiliser les formes
        cercle.dessiner();
        rectangle.dessiner();
        triangle.dessiner();
    }
}
```

**Résultat :**
```plaintext
Dessin d'un cercle
Dessin d'un rectangle
Dessin d'un triangle
```

---

### **Exemple Avancé : Système de Paiement**

#### **Problème**
Un site de commerce électronique doit gérer différents modes de paiement : **Carte Bancaire**, **PayPal**, et **Cryptomonnaie**. Le système doit rester flexible pour ajouter de nouveaux modes de paiement à l’avenir.

#### **Solution avec le Factory Pattern**

##### **Étape 1 : Interface de paiement**
```java
interface Paiement {
    void effectuerPaiement(double montant);
}
```

##### **Étape 2 : Implémentation des modes de paiement**
```java
class PaiementCarte implements Paiement {
    @Override
    public void effectuerPaiement(double montant) {
        System.out.println("Paiement de " + montant + "€ par carte bancaire.");
    }
}

class PaiementPayPal implements Paiement {
    @Override
    public void effectuerPaiement(double montant) {
        System.out.println("Paiement de " + montant + "€ via PayPal.");
    }
}

class PaiementCrypto implements Paiement {
    @Override
    public void effectuerPaiement(double montant) {
        System.out.println("Paiement de " + montant + "€ en cryptomonnaie.");
    }
}
```

##### **Étape 3 : Classe Factory**
```java
class PaiementFactory {
    public Paiement creerPaiement(String type) {
        switch (type.toUpperCase()) {
            case "CARTE":
                return new PaiementCarte();
            case "PAYPAL":
                return new PaiementPayPal();
            case "CRYPTO":
                return new PaiementCrypto();
            default:
                throw new IllegalArgumentException("Type de paiement inconnu : " + type);
        }
    }
}
```

##### **Étape 4 : Utilisation dans le code client**
```java
public class Main {
    public static void main(String[] args) {
        PaiementFactory factory = new PaiementFactory();

        // Choix du mode de paiement
        Paiement paiement = factory.creerPaiement("CARTE");
        paiement.effectuerPaiement(100.0);

        paiement = factory.creerPaiement("PAYPAL");
        paiement.effectuerPaiement(50.0);

        paiement = factory.creerPaiement("CRYPTO");
        paiement.effectuerPaiement(200.0);
    }
}
```

**Résultat :**
```plaintext
Paiement de 100.0€ par carte bancaire.
Paiement de 50.0€ via PayPal.
Paiement de 200.0€ en cryptomonnaie.
```

---

### **Avantages et Inconvénients**

#### **Avantages**
1. **Flexibilité** : Ajout de nouveaux types d’objets sans modifier le code existant.
2. **Centralisation** : La logique de création est centralisée dans la Factory.
3. **Découplage** : Le code client dépend uniquement des interfaces ou classes abstraites.

#### **Inconvénients**
1. **Complexité accrue** : Ajout d’une couche supplémentaire.
2. **Maintenance** : La Factory peut devenir difficile à gérer si le nombre de types d’objets explose.

---

### **Bonnes Pratiques**
1. **Utilisez une Factory si** :
   - La logique de création est complexe ou répétitive.
   - Vous avez besoin de gérer des familles d’objets.
2. **Évitez les chaînes `if/else` ou `switch/case` massives dans la Factory** :
   - Si le nombre de types devient trop important, envisagez des **Abstract Factory** ou des **Registries**.
3. **Testez extensivement la Factory** pour éviter les erreurs de création (ex. : type invalide).

---

### **Cas d’utilisation courants**
1. **Systèmes de paiement ou de facturation.**
2. **Création d’éléments d’interface utilisateur (boutons, menus).**
3. **Gestion des ressources (chargement d’images, sons, fichiers).**
4. **Jeux vidéo** :
   - Création d’unités, de personnages ou d’objets divers

---

