<!--
Module      : CP00-BASES
Type        : COURS
Versions    : Markdown
REAC        : DWWM V04 — CP1 : Installer et configurer son environnement de travail
Auteur      : Gemini Code Assist
Mise à jour : 2024-05
-->

# 📝 Créer un README de qualité

## 1. Introduction

### Pourquoi ce cours ?
En entreprise, un développeur passe plus de temps à **lire** du code qu'à en écrire. Le fichier `README.md` est la **porte d'entrée** de votre projet. C'est le premier document qu'un collègue ou un recruteur lira pour comprendre votre travail.

### Objectif
À la fin de ce cours, vous saurez rédiger une documentation claire, structurée et professionnelle en utilisant la syntaxe **Markdown**.

---

## 2. Concept 1 : La syntaxe Markdown

### Définition
Le **Markdown** est un langage de balisage léger. Il permet de formater du texte (gras, titres, listes) très simplement, sans utiliser de menus complexes.

### Les balises essentielles

| Résultat visuel | Syntaxe à taper |
| :--- | :--- |
| **Titre Principal** | `# Titre` |
| **Sous-titre** | `## Sous-titre` |
| **Texte en gras** | `**Texte**` |
| **Liste à puces** | `* Élément` |
| **Lien web** | `Texte du lien` |
| **Bloc de code** | \` \` \`langage [votre code] \` \` \` |

> **À retenir** : L'extension du fichier doit toujours être `.md`.

---

## 3. Concept 2 : Le plan type d'un README professionnel

Pour qu'une documentation soit utile, elle doit suivre une structure logique. Voici le plan recommandé pour vos projets DWWM/CDA :

1. **Titre du projet** : Un nom clair et une courte phrase d'accroche.
2. **Auteur** : Votre nom et un lien vers votre profil.
3. **Description** : À quoi sert l'application ? Quel problème résout-elle ?
4. **Technologies utilisées** : Liste des outils (ex: HTML, CSS, JavaScript).
5. **Installation** : Quelles sont les étapes pour lancer le projet sur un nouvel ordinateur ?

---

## 4. Exemple concret

Voici à quoi ressemble le code Markdown pour un projet de **Distributeur de Boissons** :

```markdown
# ☕ Distributeur Automatique Express

* Auteur : **Prénom NOM** - Lien GitHub

Une application web simple pour simuler la commande de boissons chaudes.


## 💻 Technologies
* HTML5 / CSS3
* JavaScript (ES6)
* Git pour le versioning


## 🛠 Installation
1. Cloner le dépôt : `git clone https://github.com/pseudo/projet.git`
2. Ouvrir le fichier `index.html` dans votre navigateur.

```

---

## 5. Résumé (Points clés)

*   **FALC** : Faites des phrases courtes et utilisez des listes pour faciliter la lecture.
*   **Code** : Utilisez toujours les "backticks" (\` \` \`) pour afficher des commandes ou du code.
*   **Utilité** : Un bon README doit permettre à quelqu'un qui ne connaît pas le projet de l'installer en moins de 2 minutes.

---

## 6. Exercice d'application

**Objectif :** Créer votre premier fichier de documentation.

**Consignes :**
1. Créez un dossier nommé `exercice-readme`.
2. À l'intérieur, créez un fichier `README.md`.
3. Rédigez la documentation d'un projet fictif de **"Gestionnaire de Recettes"** en utilisant :
    * Un titre principal.
    * Une liste à puces pour les fonctionnalités.
    * Un bloc de code pour une commande d'installation (ex: `npm install`).
    * Votre nom en gras.

**Critères de réussite :**
* Le fichier s'ouvre correctement avec l'aperçu Markdown de votre éditeur (VS Code).
* La hiérarchie des titres est respectée (# puis ##).

---

## Pour aller plus loin
* Guide officiel Markdown de GitHub
* Outil de test Markdown en ligne
