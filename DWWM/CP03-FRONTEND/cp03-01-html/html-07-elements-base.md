# Les Éléments de Contenu de Base (Textes, Listes, Liens, Images)

Maintenant que la structure de votre page (`<header>`, `<main>`, `<footer>`) est en place, nous allons apprendre à y insérer et organiser du contenu concret.

---

## Les Balises de Texte 

Le texte en HTML ne se jette pas au kilomètre. Chaque bloc de texte doit avoir un rôle précis pour être compris par les navigateurs et les outils d'accessibilité.

* **`<p>`** : Le paragraphe standard. Utilisé pour les blocs de texte courants.
* **`<strong>`** : Donne une **forte importance** à un mot ou un groupe de mots (les affiche en gras par défaut).
* **`<em>`** : Met l'**accent** sur un mot (l'affiche en italique par défaut).

⚠️ **Règle d'or :** N'utilisez pas `<strong>` juste pour "mettre en gras". Utilisez-le parce que le mot est important. Le style visuel pur sera géré plus tard par le CSS.

<div style="page-break-after:always;"></div>

## 2. Les Listes 

Les listes permettent d'ordonner des informations. HTML propose deux structures principales. Elles contiennent toutes deux des éléments de liste définis par la balise `<li>` (*List Item*).

### A. La liste à puces / non-ordonnée (`<ul>`)

Utilisée quand l'ordre des éléments n'a pas d'importance (ex: une liste de courses ou un menu de navigation).

```html
<ul>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ul>

```

### B. La liste numérotée / ordonnée (`<ol>`)

Utilisée quand l'ordre est crucial (ex: les étapes d'une recette ou d'un algorithme).

```html
<ol>
  <li>Étape 1 : Créer le fichier index.html</li>
  <li>Étape 2 : Écrire la structure de base</li>
</ol>

```

<div style="page-break-after:always;"></div>

## 3. Les Liens et les Images 

Ces deux balises font la force du web (l'Hypertexte et le Multimédia). Elles utilisent obligatoirement des **attributs** pour fonctionner.

### A. La balise de lien `<a>` (Ancre)

Elle nécessite l'attribut `href` pour indiquer la destination (un autre site ou une page locale).

```html
<a href="https://wikipedia.org">Visiter Wikipédia</a>

<a href="./contact.html">Nous contacter</a>

```

### B. La balise d'image `<img>`

C'est une balise **orpheline**. Elle nécessite deux attributs obligatoires :

* `src` : Le chemin vers le fichier image.
* `alt` : La description textuelle de l'image (pour les robots de recherche et les personnes malvoyantes).

```html
<img src="./images/logo.png" alt="Logo officiel de l'école de code">

```

<div style="page-break-after:always;"></div>

## 4. Exemples de critères de validation

| Structure de Code | Statut | Correction / Pourquoi ? |
| --- | --- | --- |
| `<p>Le site est <strong>génial</strong>.</p>` | ✅ Correct | L'imbrication est propre, la balise `<strong>` est bien fermée avant le `</p>`. |
| `<img src="./photo.jpg">` | ❌ Erreur | Il manque l'attribut `alt`. L'image n'est pas accessible. |
| `<ul>Élément 1</ul>` | ❌ Erreur | Une liste `<ul>` ou `<ol>` ne peut contenir **que** des balises `<li>` directement sous elle. |