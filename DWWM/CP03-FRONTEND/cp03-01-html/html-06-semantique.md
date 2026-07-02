# L’Importance de la Sémantique en HTML (SEO & Accessibilité)

Avant de donner du style à un site avec le CSS, il faut lui donner du **sens**. C’est le rôle de la **sémantique**. En HTML, **utiliser la bonne balise au bon endroit est la règle la plus importante du développement web**.

---

## 1. Qu'est-ce que la sémantique ? 

Développer de manière sémantique, c'est choisir une balise HTML pour **ce qu'elle signifie** et non pour son apparence visuelle.

* **Une approche non sémantique :** Utiliser des `<div>` ou des `<span>` partout en modifiant leur taille en CSS. Les machines (Google, robots) ne comprennent pas ce que contient la page.
* **Une approche sémantique :** Utiliser `<nav>` pour un menu, `<article>` pour une actualité, `<time>` pour une date. Chaque élément est clairement identifié.

### Les deux piliers majeurs de la sémantique :

#### A. L'Accessibilité (A11y)

Les personnes non-voyantes ou malvoyantes utilisent un logiciel appelé **lecteur d'écran** (comme NVDA ou VoiceOver) qui lit le code HTML à haute voix.

* Si le site utilise `<nav>`, le logiciel dit : *"Zone de navigation"*. L'utilisateur peut sauter directement au menu.
* Si le site utilise `<div class="menu">`, le logiciel dit simplement : *"Division"*. L'utilisateur est perdu.

#### B. Le Référencement Naturel (SEO)

Les robots des moteurs de recherche (les *crawlers*) parcourent votre code pour comprendre le sujet de votre page. Un site sémantique permet d'indexer correctement vos informations, ce qui fait monter votre site dans les résultats de recherche.

---

## 2. Appliquer : Tableau des principales balises sémantiques

Voici le guide des balises structurelles HTML5 à utiliser pour organiser vos pages.

| Balise HTML | Rôle sémantique (Ce qu'elle indique) | Bonne pratique d'utilisation |
| --- | --- | --- |
| **`<header>`** | L'en-tête d'une page ou d'une section. | Contient souvent le logo, le titre principal et la navigation. |
| **`<nav>`** | La zone de navigation principale du site. | Doit contenir les liens majeurs (les menus de premier niveau). |
| **`<main>`** | Le contenu central et unique de la page. | **Unique** : il ne peut y en avoir qu'un seul "visible" par page web. |
| **`<section>`** | Un bloc thématique dans la page. | Doit presque toujours commencer par un titre (`<h2>` à `<h6>`). |
| **`<article>`** | Un contenu autonome et indépendant. | Peut être extrait du site et partagé sans perdre son sens (ex: article de blog, produit). |
| **`<aside>`** | Un contenu secondaire ou lié de loin. | Utilisé pour les barres latérales, les publicités ou les définitions. |
| **`<footer>`** | Le pied de page. | Contient les mentions légales, les droits d'auteur ou les liens de contact. |
| **`<time>`** | Une date ou une heure précise. | Aide les moteurs de recherche à dater précisément un événement ou un article. |

---

## 3. Analyser : Le piège visuel (Niveau 4 - Bloom)

⚠️ **Règle d'or absolue : Le HTML donne du sens, le CSS donne le style.**

Il ne faut jamais choisir une balise pour la façon dont le navigateur l'affiche par défaut.

* **Exemple :** La balise `<h1>` affiche le texte en très grand et en gras.
* *L'erreur :* Utiliser un `<h1>` au milieu d'un paragraphe juste parce qu'on veut que ce mot soit écrit en grand.
* *La bonne pratique :* Utiliser une balise neutre `<span>` (ou `<strong>` si le mot est important) et modifier sa taille avec CSS.



---

## 4. TP: Corriger un code 

Regardez ce comparatif entre un code valide et un code inaccessible.

### Code Non Sémantique (À éviter ❌)

```html
<div class="mon-en-tete">
  <span class="mon-gros-titre">Mon Blog</span>
  <div class="les-liens">
    <a href="#">Accueil</a> | <a href="#">Articles</a>
  </div>
</div>

```

### Code Sémantique (Standard Professionnel ✅)

```html
<header>
  <h1>Mon Blog</h1>
  <nav>
    <ul>
      <li><a href="#">Accueil</a></li>
      <li><a href="#">Articles</a></li>
    </ul>
  </nav>
</header>

```