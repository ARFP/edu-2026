# Mon CV en ligne

L'objectif de cette suite d'exercices est de créer la structure complète de votre premier site web professionnel : **Votre CV numérique**.

> [!IMPORTANT] Objectifs pédagogiques
>
> **À la fin de ce module HTML, vous serez capable de :**
> * **Créer l'infrastructure** d'une page web valide aux normes internationales (W3C).
> * **Configurer les informations cachées** d'un site pour qu'il s'affiche correctement sur les ordinateurs et sur les téléphones portables.
> * **Structurer un document** en utilisant les balises sémantiques modernes pour rendre votre site accessible à tous (A11y) et visible sur les moteurs de recherche (SEO).
> * **Intégrer du contenu varié** de manière propre : des textes, des images de profil, des listes d'expériences et des liens vers vos réseaux professionnels.
> * **Organiser des données** complexes sous forme de tableau pour afficher vos compétences techniques.
> * **Construire une zone de contact** interactive avec des champs de saisie sécurisés pour permettre aux recruteurs de vous écrire.

--- 

> [!WARNING] Attention
>
> Pour cette suite d'exercices, l'utilisation du CSS est **strictement interdite**. 
> Vous serez évalué sur la structure HTML uniquement.
> 
>  À la fin de chaque exercice, votre code doit être propre et textuel. Ne vous inquiétez pas si le rendu visuel dans le navigateur est très simple et sans couleurs : c'est tout à fait normal ! Le design et les décors arriveront juste après avec le [module CSS](#).

--- 

## Bloc 0 : Préparation
 

## Bloc 1 : L'Infrastructure

### Exercice 1 : La naissance du projet

* **Objectif :** Créer l'environnement de travail et le fichier de base.
* **Consigne :** Créez un dossier nommé `mon-cv`. À l'intérieur, créez le fichier `index.html`. Écrivez la structure minimale obligatoire de la page (`<!DOCTYPE html>`, `<html>`, `lang="fr"`).

### Exercice 2 : Configurer l'entête

* **Objectif :** Configurer le `<head>` sans meta.
* **Consigne :** Dans le `<head>`, ajoutez le titre de l'onglet sous la forme : `Prénom Nom - Développeur Web`.

### Exercice 3 : Préparer le terrain (Les Meta)

* **Objectif :** Configurer les métadonnées de base.
* **Consigne :** Ajoutez la balise pour l'encodage en `UTF-8` et une balise `description` qui résume votre profil en deux phrases (ex: "Développeur web en formation, passionné par...").

### Exercice 4 : Le test du téléphone

* **Objectif :** Rendre l'en-tête compatible mobile.
* **Consigne :** Ajoutez la balise `viewport`. *(Note pédagogique : Les apprenants ne verront pas de changement visuel immédiat, mais vous validerez cette étape en inspectant leur code en mode mobile).*

---

## Bloc 2 : Le Contenu et la Structure (Exercices 5 à 10)

### Exercice 5 : Les fondations visuelles (`<body>`)

* **Objectif :** Poser les trois zones sémantiques principales.
* **Consigne :** Dans le `<body>`, créez les trois grands blocs de votre page : l'en-tête du CV, la zone principale pour votre parcours, et le pied de page pour vos coordonnées.

### Exercice 6 : Structurer les grandes sections (Sémantique 1)

* **Objectif :** Utiliser les balises de structure au bon endroit.
* **Consigne :** * Dans l'en-tête, placez un `<h1>` avec votre nom.
* Dans la zone principale, créez trois zones `<section>` : "À propos", "Expériences" et "Formations". Donnez un titre `<h2>` à chaque section.
* Dans le pied de page, insérez un paragraphe avec vos droits d'auteur.



### Exercice 7 : Remplir le CV (Éléments de contenu)

* **Objectif :** Manipuler les listes, les liens et les images.
* **Consigne :** * Dans "À propos" : Ajoutez votre photo (balise `<img>` avec un `alt` descriptif complet).
* Dans "Expériences" : Créez une liste à puces (`<ul>`) pour énumérer vos anciens postes.
* Dans le pied de page : Ajoutez un lien hypertexte (`<a>`) vers votre profil LinkedIn ou votre GitHub.



### Exercice 8 : Préciser le texte (Sémantique 2)

* **Objectif :** Utiliser les balises sémantiques textuelles avancées.
* **Consigne :** * Entourez toutes les dates de vos expériences avec la balise `<time>` et son attribut `datetime` (ex: `<time datetime="2026-06">Juin 2026</time>`).
* Utilisez la balise `<strong>` pour mettre en valeur les compétences clés au milieu de vos paragraphes.



### Exercice 9 : Le tableau des compétences (Les Tableaux)

* **Objectif :** Organiser des données complexes.
* **Consigne :** À la suite de vos expériences, créez une nouvelle section "Compétences Techniques". Construisez un tableau (`<table>`) à deux colonnes : à gauche le langage (ex: HTML5), à droite votre niveau auto-évalué (ex: Maîtrisé). N'oubliez pas les balises `<thead>` et `<tbody>`.

### Exercice 10 : Le formulaire de contact (Les Formulaires)

* **Objectif :** Créer une zone d'interaction complète.
* **Consigne :** Tout en bas de votre page, créez une section "Me contacter". Construisez un formulaire contenant : un champ texte pour le nom, un champ de type email, une zone de texte (`<textarea>`) pour le message, et un bouton d'envoi. Veillez à lier chaque `<label>` à son `<input>` avec l'attribut `id`.

---

## 🎉 Résultat à la fin du module HTML :

L'apprenant possède :
- Un fichier `index.html` 
- Un fichier `contact.html`

Ces 2 fichiers sont complets, parfaitement valides au validateur W3C, Le contenu est entièrement sémantique et accessible. Le site est visuellement brut de décoffrage (police par défaut, éléments les uns sous les autres), ce qui créera une immense frustration positive, parfaite pour lancer le module CSS !