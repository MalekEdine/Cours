# Programme détaillé du Module 2 : Concevoir et développer une application sécurisée organisée en couches

## Cours 1 : Analyse des besoins et maquettage d'une application (UML, etc.)

### Séance 1 : Collecte des besoins fonctionnels et non fonctionnels
- **Objectifs** : Apprendre à identifier et formaliser les besoins d'un projet.
- **Contenu** :
  - Techniques de collecte des besoins : entretiens, questionnaires, ateliers.
  - Différence entre besoins fonctionnels et non fonctionnels.
  - Rédaction de spécifications fonctionnelles détaillées.
  - Introduction à la méthode MoSCoW pour la priorisation des exigences.
- **Exercices** : Création d'un document de spécifications fonctionnelles pour un projet fictif.

### Séance 2 : Introduction aux diagrammes UML
- **Objectifs** : Maîtriser les différents types de diagrammes UML pour la modélisation des applications.
- **Contenu** :
  - Les principaux diagrammes UML : cas d'utilisation, classes, séquence, activité.
  - Utilisation d'UML pour représenter les fonctionnalités d'une application.
  - Outils de modélisation UML (Lucidchart, Visual Paradigm, etc.).
- **Exercices** : Réalisation de diagrammes de cas d'utilisation et de classes pour un projet donné.

### Séance 3 : Maquettage d'interfaces utilisateur et conception de prototypes
- **Objectifs** : Apprendre à créer des maquettes d'interfaces utilisateur.
- **Contenu** :
  - Principes de base de la conception d'interface utilisateur (UI/UX).
  - Utilisation d'outils de maquettage (Figma, Adobe XD, Balsamiq).
  - Création de wireframes et de prototypes interactifs.
  - Itérations et validation des maquettes avec les parties prenantes.
- **Exercices** : Réalisation d'une maquette interactive pour une application web.

### Séance 4 : Étude des scénarios d'utilisation
- **Objectifs** : Comprendre l'importance des scénarios d'utilisation pour les tests et le développement.
- **Contenu** :
  - Définition des scénarios d'utilisation (user stories, user journeys).
  - Rédaction des scénarios d'utilisation avec les critères d'acceptation.
  - Validation des scénarios avec les utilisateurs finaux.
  - Liens entre scénarios d'utilisation et tests fonctionnels.
- **Exercices** : Écriture de user stories et de critères d'acceptation pour une fonctionnalité donnée.

---

## Cours 2 : Développer les composants d'accès aux données relationnelles (SQL)

### Séance 1 : Introduction aux bases de données relationnelles et à SQL
- **Objectifs** : Comprendre les bases de la gestion des données relationnelles et le langage SQL.
- **Contenu** :
  - Concepts de bases de données relationnelles : tables, clés primaires et étrangères.
  - Introduction aux commandes SQL de base : SELECT, INSERT, UPDATE, DELETE.
  - Normalisation des bases de données.
- **Exercices** : Création et manipulation d'une base de données simple avec des commandes SQL de base.

### Séance 2 : Modélisation de bases de données et conception de schémas
- **Objectifs** : Maîtriser la conception de schémas de bases de données.
- **Contenu** :
  - Conception de schémas relationnels avec les diagrammes Entité-Association.
  - Techniques de normalisation pour éviter la redondance des données.
  - Utilisation d'outils de modélisation de bases de données (MySQL Workbench, ERDPlus).
- **Exercices** : Création d'un schéma relationnel pour une application donnée.

### Séance 3 : Techniques de requêtage avancées (jointures, transactions, indexation)
- **Objectifs** : Apprendre à optimiser les requêtes SQL pour de meilleures performances.
- **Contenu** :
  - Jointures : INNER JOIN, LEFT JOIN, RIGHT JOIN, et FULL JOIN.
  - Utilisation des transactions pour garantir l'intégrité des données.
  - Introduction aux index et à leur impact sur les performances.
- **Exercices** : Écriture de requêtes SQL complexes avec jointures et transactions.

### Séance 4 : Optimisation des performances des bases de données
- **Objectifs** : Améliorer les performances des bases de données relationnelles.
- **Contenu** :
  - Analyse des plans d'exécution des requêtes.
  - Optimisation des index et des requêtes SQL.
  - Techniques de mise en cache pour les bases de données.
- **Exercices** : Optimisation des performances d'une base de données existante.

---

## Cours 3 : Développer les composants d'accès aux données non-relationnelles (NoSQL)

### Séance 1 : Introduction aux bases de données NoSQL (MongoDB, Cassandra, etc.)
- **Objectifs** : Comprendre les principes des bases de données NoSQL.
- **Contenu** :
  - Types de bases de données NoSQL : documentaires, colonnes, clé-valeur, graphiques.
  - Comparaison entre les bases de données relationnelles et NoSQL.
  - Cas d'utilisation des bases de données NoSQL.
- **Exercices** : Installation de MongoDB et manipulation de documents.

### Séance 2 : Utilisation de NoSQL pour des applications spécifiques (Big Data, IoT)
- **Objectifs** : Apprendre à utiliser NoSQL dans des contextes spécifiques.
- **Contenu** :
  - Stockage et gestion des données volumineuses (Big Data).
  - Intégration des bases de données NoSQL avec des applications IoT.
  - Techniques de partitionnement et de réplication.
- **Exercices** : Création d'une base de données NoSQL pour une application IoT.

### Séance 3 : Mise en œuvre de la gestion de données non structurées
- **Objectifs** : Manipuler des données non structurées avec des bases NoSQL.
- **Contenu** :
  - Stockage des documents JSON dans MongoDB.
  - Indexation et recherche de données non structurées.
  - Sécurisation et gestion des droits d'accès aux données.
- **Exercices** : Développement d'une API REST pour manipuler des données non structurées.

---

## Cours 4 : Développer la persistance des données avec SPRING

### Séance 1 : Introduction au framework SPRING pour le développement JAVA
- **Objectifs** : Comprendre l'architecture et les composants du framework Spring.
- **Contenu** :
  - Introduction à Spring Core, Spring Boot et Spring Data.
  - Configuration d'un projet Spring Boot.
  - Injection de dépendances avec Spring.
- **Exercices** : Création d'une application Spring Boot simple.

### Séance 2 : Utilisation de Spring Data JPA pour la persistance des données
- **Objectifs** : Gérer la persistance des données avec Spring Data JPA.
- **Contenu** :
  - Mapping objet-relationnel avec JPA.
  - Création d'entités et de référentiels.
  - Requêtage avec les méthodes de Spring Data JPA.
- **Exercices** : Développement d'un service CRUD avec Spring Data JPA.

### Séance 3 : Gestion des transactions et du mapping objet-relationnel
- **Objectifs** : Maîtriser les transactions et le mapping objet-relationnel en Java.
- **Contenu** :
  - Configuration des transactions dans Spring.
  - Utilisation des annotations pour le mapping JPA.
  - Optimisation des requêtes avec les critères JPA.
- **Exercices** : Implémentation de la gestion des transactions pour une application Spring.

---

## Cours 5 : Développer l'architecture micro-service

### Séance 1 : Principes de l'architecture micro-service (modularité, indépendance)
- **Objectifs** : Comprendre les concepts fondamentaux des micro-services.
- **Contenu** :
  - Avantages et inconvénients de l'architecture micro-services.
  - Différences entre monolithes et micro-services.
  - Techniques de découpage des services.
- **Exercices** : Découpage d'une application monolithique en micro-services.

### Séance 2 : Implémentation de micro-services avec SPRING Boot
- **Objectifs** : Développer des micro-services avec Spring Boot.
- **Contenu** :
  - Création de micro-services avec Spring Boot.
  - Utilisation de Spring Cloud pour la gestion des micro-services.
  - Mise en œuvre de la découverte des services.
- **Exercices** : Développement de plusieurs micro-services interconnectés.

### Séance 3 : Communication inter-services (REST, messaging)
- **Objectifs** : Mettre en place la communication entre micro-services.
- **Contenu** :
  - Communication via API REST et gestion des appels HTTP.
  - Utilisation de systèmes de messaging (RabbitMQ, Kafka).
  - Gestion de la résilience et des erreurs (circuit breaker).
- **Exercices** : Implémentation de la communication entre deux micro-services avec REST.

---

## Cours 6 : Sécuriser une application avec SPRING

### Séance 1 : Introduction à la sécurité des applications web
- **Objectifs** : Comprendre les principes de sécurité pour les applications web.
- **Contenu** :
  - Principales menaces : injection SQL, XSS, CSRF.
  - Authentification et autorisation.
  - Chiffrement des données sensibles.
- **Exercices** : Implémentation de l'authentification de base sur une application web.

### Séance 2 : Utilisation de Spring Security pour sécuriser les applications
- **Objectifs** : Apprendre à sécuriser les applications avec Spring Security.
- **Contenu** :
  - Configuration de Spring Security dans un projet.
  - Mise en place de l'authentification (Basic, JWT).
  - Gestion des rôles et des autorisations.
- **Exercices** : Sécurisation d'une API REST avec Spring Security.

### Séance 3 : Sécurisation des micro-services
- **Objectifs** : Protéger les micro-services avec des techniques de sécurité modernes.
- **Contenu** :
  - Sécurisation des communications inter-services.
  - Utilisation de OAuth2 pour l'autorisation des services.
  - Intégration de Keycloak ou d'un autre serveur d'authentification.
- **Exercices** : Mise en œuvre de la sécurisation sur un projet de micro-services.

---

## Cours 7 : Développer des tests unitaires

### Séance 1 : Introduction aux tests unitaires avec JUnit
- **Objectifs** : Maîtriser les bases du testing en Java.
- **Contenu** :
  - Rôle et avantages des tests unitaires.
  - Utilisation de JUnit pour écrire et exécuter les tests.
  - Création de tests pour les méthodes Java.
- **Exercices** : Écriture de tests unitaires pour une classe Java donnée.

### Séance 2 : Utilisation de Mockito pour les tests de services
- **Objectifs** : Apprendre à tester les services avec des mocks.
- **Contenu** :
  - Principe du mocking et de l'injection de dépendances dans les tests.
  - Utilisation de Mockito pour simuler les comportements.
  - Tests des services Spring avec Mockito.
- **Exercices** : Création de tests de services avec Mockito.
