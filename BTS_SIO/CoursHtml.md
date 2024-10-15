Voici le **cours complet** pour la **Session 1 : Introduction à HTML** avec des explications, des exemples de code et des exercices pratiques.

---

## **Session 1 : Introduction à HTML**

### **Objectif** : Comprendre la structure de base d'une page web et apprendre à créer une page simple en HTML.

---

### **1. Qu'est-ce que HTML ?**
**HTML** signifie **HyperText Markup Language**. C’est le langage utilisé pour structurer et présenter du contenu sur le web. HTML ne s'occupe que de la structure d'une page web, tandis que le style (aspect visuel) est géré par CSS.

- **HyperText** : Les liens entre différentes pages.
- **Markup Language** : Le balisage pour structurer le contenu (titres, paragraphes, images, etc.).

---

### **2. Structure de base d'une page HTML**

Voici la structure minimale d'une page HTML :
```html
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ma Première Page</title>
</head>
<body>
    <h1>Bienvenue sur ma première page HTML</h1>
    <p>Ceci est mon premier paragraphe en HTML.</p>
</body>
</html>
```

#### **Explication :**
- `<!DOCTYPE html>` : Indique au navigateur qu'il s'agit d'une page HTML5.
- `<html>` : La balise qui contient tout le contenu de la page.
- `<head>` : La section où on met les informations sur la page (comme le titre).
- `<meta charset="UTF-8">` : Déclare l’encodage des caractères (UTF-8 est le plus commun).
- `<meta name="viewport" content="width=device-width, initial-scale=1.0">` : Rend la page responsive pour les appareils mobiles.
- `<title>` : Définit le titre de la page (ce qui apparaît dans l’onglet du navigateur).
- `<body>` : Contient le contenu visible de la page (texte, images, liens, etc.).

---

### **3. Balises de base en HTML**

#### **Les titres (`<h1>` à `<h6>`) :**
Les balises de titre vont de `<h1>` (le plus important) à `<h6>` (le moins important).
```html
<h1>Ce titre est très important (h1)</h1>
<h2>Ce titre est un peu moins important (h2)</h2>
<h3>Un titre encore moins important (h3)</h3>
```

#### **Les paragraphes (`<p>`) :**
Les paragraphes sont définis avec la balise `<p>`.
```html
<p>Ceci est un paragraphe de texte.</p>
```

#### **Les images (`<img>`) :**
Pour insérer une image, on utilise la balise `<img>`. Elle n’a pas de balise de fermeture.
```html
<img src="https://www.example.com/image.jpg" alt="Description de l'image" width="300">
```
- `src` : Lien vers l'image.
- `alt` : Texte alternatif si l'image ne charge pas.
- `width` : La largeur de l'image.

#### **Les liens (`<a>`) :**
Pour ajouter des liens, on utilise la balise `<a>`.
```html
<a href="https://www.example.com">Visitez ce site web</a>
```
- `href` : Lien vers lequel redirige l’utilisateur.

---

### **4. Création d'une page HTML simple**

Voici un exemple de page HTML complète avec tous les éléments de base :
```html
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Page Web Simple</title>
</head>
<body>
    <h1>Bienvenue sur ma première page HTML</h1>
    <p>Je découvre le HTML et c'est passionnant !</p>

    <h2>Une liste de mes passe-temps</h2>
    <ul>
        <li>La lecture</li>
        <li>Le cinéma</li>
        <li>Les jeux vidéo</li>
    </ul>

    <h2>Voici une image</h2>
    <img src="https://www.example.com/image.jpg" alt="Une belle image" width="300">

    <h2>Découvrez mon site préféré :</h2>
    <a href="https://www.example.com">Cliquez ici pour visiter !</a>
</body>
</html>
```

#### **Explication supplémentaire** :
- **Listes non ordonnées** (`<ul>`, `<li>`) : Pour créer des listes à puces.
  ```html
  <ul>
      <li>Élément 1</li>
      <li>Élément 2</li>
  </ul>
  ```
- **Listes ordonnées** (`<ol>`, `<li>`) : Pour créer des listes numérotées.
  ```html
  <ol>
      <li>Premier élément</li>
      <li>Deuxième élément</li>
  </ol>
  ```

---

### **5. Exercice pratique**

#### **Exercice 1 : Créer votre première page HTML**
1. Créez un fichier HTML nommé `index.html`.
2. Utilisez la structure de base d'une page HTML.
3. Ajoutez les éléments suivants dans le `<body>` :
   - Un titre principal (`<h1>`) avec votre nom.
   - Un paragraphe (`<p>`) qui explique pourquoi vous voulez apprendre le HTML.
   - Une image (utilisez une URL d'image en ligne).
   - Une liste non ordonnée de trois de vos films préférés.
   - Un lien (`<a>`) vers votre site web ou un site que vous aimez.

**Exemple de résultat attendu :**
```html
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ma première page HTML</title>
</head>
<body>
    <h1>Bonjour, je suis [Votre nom]</h1>
    <p>Je veux apprendre le HTML pour créer de beaux sites web.</p>

    <h2>Mes films préférés</h2>
    <ul>
        <li>Inception</li>
        <li>Interstellar</li>
        <li>Le Seigneur des Anneaux</li>
    </ul>

    <h2>Voici une image cool :</h2>
    <img src="https://www.example.com/image.jpg" alt="Image cool" width="300">

    <h2>Visitez mon site préféré :</h2>
    <a href="https://www.example.com">Cliquez ici</a>
</body>
</html>
```

#### **Exercice 2 : Formulaire simple**
1. Créez une nouvelle page HTML nommée `formulaire.html`.
2. Ajoutez un formulaire avec les éléments suivants :
   - Un champ texte pour entrer un nom.
   - Un champ pour entrer un e-mail.
   - Un bouton de soumission.

**Exemple de formulaire simple :**
```html
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Formulaire Simple</title>
</head>
<body>
    <h1>Formulaire de contact</h1>
    <form action="#">
        <label for="name">Nom :</label>
        <input type="text" id="name" name="name"><br><br>

        <label for="email">E-mail :</label>
        <input type="email" id="email" name="email"><br><br>

        <button type="submit">Envoyer</button>
    </form>
</body>
</html>
```

---

### **Récapitulatif :**
- **HTML** est utilisé pour structurer une page web.
- Les éléments de base incluent des titres (`<h1>` à `<h6>`), des paragraphes (`<p>`), des images (`<img>`), des liens (`<a>`), et des listes (`<ul>`, `<ol>`, `<li>`).
- Une page web HTML est composée d'une structure de base (`<!DOCTYPE html>`, `<html>`, `<head>`, `<body>`).

---

### **Prochain cours :**
Dans la session 2, nous allons approfondir la structure d'une page avec des balises sémantiques et explorer les tableaux et les formulaires.