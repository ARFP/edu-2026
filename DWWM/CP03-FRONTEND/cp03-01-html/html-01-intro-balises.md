# Introduction au HTML 

Avant de se jeter dans le codage d'une page web, il est indispensable de comprendre le fonctionnement de base du langage **HTML** (*HyperText Markup Language*).

> [!NOTE] 
> 
> #### Objectifs pédagogiques
> À la fin de cette première partie, vous serez capable de :
> * **Expliquer le rôle du HTML** : Comprendre la différence entre un langage de programmation (logique) et un langage de balisage (structure).
> * **Décoder l'anatomie d'une balise** : Identifier et utiliser correctement une balise ouvrante, un contenu et une balise fermante.
> * **Manipuler les deux types de balises** : Faire la différence entre une balise paire (conteneur) et une balise orpheline (auto-fermante).
> * **Ajouter des options avec les attributs** : Configurer une balise en lui ajoutant des informations complémentaires sous la forme `nom="valeur"`.
> * **Respecter l'imbrication du code** : Emboîter plusieurs balises les unes dans les autres sans faire d'erreur de fermeture.
> * **Créer un fichier HTML de base valide** : Écrire la structure de départ obligatoire de n'importe quel site web (`<!DOCTYPE html>`, `<html>`, `<head>`, `<body>`).

--- 


## Le Système de Balises et d'Attributs

HTML n'est pas un langage de programmation, mais un **langage de balisage**. Il sert à structurer et à donner du sens à votre contenu.

---

### 1. Anatomie d'une Balise (Niveau 1 & 2 - Bloom)

Pour construire une page web, on utilise des **balises** (ou *tags* en anglais). Elles indiquent au navigateur la nature du contenu (texte, titre, image, lien).

Une balise standard se compose de trois éléments :

1. **La balise ouvrante** (`<p>`) : Elle indique où commence l'élément.
2. **Le contenu** : Le texte ou la ressource à afficher.
3. **La balise fermante** (`</p>`) : Elle indique où se termine l'élément (marquée par un slash `/`).

```text
 <p>  Bonjour le monde !  </p>
  │           │            │
  ▼           ▼            ▼
Balise     Contenu      Balise
ouvrante               fermante

```

---

### 2. Les deux types de balises

Il existe deux catégories de balises en HTML :

#### A. Les balises paires (Conteneurs)

Elles entourent un contenu et nécessitent obligatoirement une balise ouvrante et une balise fermante.

* **Exemple :** `<h1>Mon titre</h1>`.

#### B. Les balises orphelines (Auto-fermantes)

Elles n'entourent aucun texte. Elles servent à insérer un élément ou une instruction à un endroit précis. Elles n'ont pas de balise fermante.

* **Exemple :** `<img src="photo.jpg" alt="Ma photo">`.

---

### 3. Les Attributs

Un **attribut** permet d'ajouter des informations complémentaires ou des configurations à une balise. Il se place **toujours dans la balise ouvrante** et s'écrit sous la forme : `nom="valeur"`.

```text
<a href="https://google.com"> Visiter Google </a>
    │           │
    ▼           ▼
 Nom de      Valeur de
l'attribut  l'attribut

```

#### Les attributs les plus courants :


| Nom de l'attribut | Balise(s) concernée(s) | Description | Exemple |
| --- | --- | --- | --- |
| **`href`** | `<a>`, `<link>` | Indique l'adresse ou le chemin de la page ou du fichier vers lequel on veut aller. | `<a href="https://google.com">` |
| **`src`** | `<img>`, `<script>`, `<iframe>` | Indique le chemin du fichier multimédia ou du script à charger sur la page. | `<img src="./photo.jpg">` |
| **`alt`** | `<img>` | Donne une description de l'image. Obligatoire pour l'accessibilité (A11y) et le robot Google (SEO). | `<img src="logo.png" alt="Logo de l'école">` |
| **`id`** | Universel | Donne un nom unique à une balise. Interdit d'utiliser le même `id` deux fois sur la même page. | `<p id="paragraphe-important">` |
| **`class`** | Universel | Donne un nom à un groupe de balises. Permet de cibler plusieurs éléments en CSS ou en JavaScript. | `<li class="liste-item">` |
| **`data-*`** | Universel | Permet de cacher une information technique (comme un prix, un ID) pour la donner à un script JavaScript. | `<button data-prix="1.50">` |


---

### 4. Structure globale d'un document

Toutes ces balises s'emboîtent pour former un document HTML valide. Voici l'arbre de structure que vous devez créer au début de chaque projet :

```html
<!DOCTYPE html>
<html lang="fr">
  <head>
  </head>
  
  <body>
  </body>

</html>
```

La balise `<html>` est l'élément racine de la page. Comme en XML ou en SGML, ce modèle impose un prologue (`<!DOCTYPE>`) suivi d'une balise unique qui englobe tout le reste. En web, on dit que `<html>` est la racine de **l'arbre DOM**.

| Élément | Rôle | 
| --- | --- | 
| **`<!DOCTYPE html>`** | Indique au navigateur que le fichier utilise HTML5. |
| **`<html lang="fr">`** | Conteneur de toute la page. L'attribut `lang` indique la langue pour les traducteurs et les lecteurs d'écran. | 
| **`<head>`** | Informations (cachées) de la page | 
| **`<body>`** | Corps (visible) de la page |
| **Imbrication** | Une balise ouverte à l'intérieur d'une autre doit être fermée avant sa balise parente : `<p> Texte <strong>important</strong> </p>`. | 

## Ressources

- [Apprendre le HTML sur MDN](https://developer.mozilla.org/fr/docs/Web/HTML)
- [Apprendre le HTML sur GraphikArt](https://grafikart.fr/formations/html)