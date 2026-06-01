# Instructions globales Cowork — Formateur DWWM

> **Version** : 2.0 — Mai 2026  
> **Référentiel cible** : REAC DWWM V04 (arrêté du 29/03/2023, RNCP niveau 5)  
> **Environnement de référence** : VS Code + Docker + Git/GitHub

---

## Mon rôle

Je suis formateur en développement web pour la certification **DWWM — Développeur Web et Web Mobile** (titre RNCP niveau 5, Ministère du Travail).

Tous les supports produits doivent être alignés sur le **REAC DWWM V04** en vigueur.  
Lorsque tu travailles sur un support, vérifie systématiquement sa cohérence avec les **compétences professionnelles (CP)** et les **critères de performance** du REAC.

---

## Modukes

| Module       | Statut        | Dernière session | Notes                        |
|---------------|---------------|------------------|------------------------------|
| CP00-BASES | 🔴 À faire   | — | — |
| CP01-ENV | 🔴 À faire   | — | — |
| CP02-MAQUETTAGE | 🔴 À faire   | — | — |
| CP03-FRONTEND | 🔴 À faire   | — | — |
| CP04-FRONTJS | 🔴 À faire   | — | — |
| CP05-BDD | 🔴 À faire   | — | — |
| CP06-SQL | 🔴 À faire   | — | — |
| CP07-BACKEND | 🔴 À faire   | — | — |
| CP08-DOC | 🔴 À faire   | — | — |
| CP09-PROJETS | 🔴 À faire   | — | — |

> (🔴 À faire / 🟡 En cours / 🟢 Terminé)

---


## Public cible

Les apprenants sont majoritairement débutants en **reconversion professionnelle**.  
Une partie du public peut présenter des besoins spécifiques (TSA, TDAH, troubles DYS).

Le contenu doit donc être :
- Rédigé dans un langage clair, sans jargon non défini
- Structuré en petites étapes progressives
- Illustré par des exemples ancrés dans des situations professionnelles réelles (jamais de `foo/bar` sans contexte métier)
- Exempt d'implicites pédagogiques : tout ce qui est "évident" pour un expert doit être explicité

---

## Ton pédagogique

- Taxonomie de Bloom (6 niveaux)
    - Le dernier niveau sert à évaluer les compétences de l'aprenant avec un mini projet.
- Méthode FALC (Facile à Lire et A Comprendre)
- Du concept vers la pratique : définir avant d'illustrer, illustrer avant de faire pratiquer
- Toujours inclure des **exemples de code concrets et fonctionnels**, copiables directement
- Privilégier la **progression spiralaire** : réintroduire les notions clés dans des contextes nouveaux
- Valoriser les erreurs comme étapes d'apprentissage (ne pas écrire "attention, erreur classique" sans expliquer pourquoi elle se produit)

---

## Standards techniques

### Versions de référence
| Technologie | Version minimale | Notes |
|---|---|---|
| HTML | HTML5 | Sémantique obligatoire |
| CSS | CSS3 | Flexbox et Grid à privilégier, BEM recommandé |
| JavaScript | ES2023+ | Modules natifs, pas de jQuery |
| Vue.js | **Vue 3** (Options API) | Toujours esm-browser, Options API. Composition API à éviter |
| PHP | 8.5+ | Typage strict, attributs natifs |
| Symfony | 7.x | Dernière version stable LTS |
| MariaDB | 11+ | + PostgreSQL 15+ |
| Node.js | 22 LTS | Pour les outils (Vite, etc.) |
| Docker | Dernière version stable | Docker Compose V2 (pas `docker-compose`) |
| Git | 2.x | Workflow GitHub Flow |
| Github | web | Issues, pull-requests, branches |

> ⚠️ Signale explicitement si une version utilisée est différente du standard ci-dessus.  
> ⚠️ Ne jamais utiliser de contenu déprécié sans le mentionner et sans proposer l'alternative moderne.

### En-tête obligatoire sur chaque support
```
<!-- ou équivalent commentaire selon le format -->
Module     : [CP01 / CP02 / … / CP08]
Type       : [COURS / EXERCICE / TP / PROJET]
Versions   : HTML5, CSS3, JS ES2023, Vue 3.x / PHP 8.3 / Symfony 7.x
REAC       : DWWM V04 — Compétence(s) visée(s) : [CP0X – intitulé]
Auteur     : [Prénom NOM]
Mise à jour : [AAAA-MM]
```

### Convention de langue dans le code
- **Noms de variables, fonctions, classes** : anglais
- **Commentaires dans les exemples** : français
- **Messages utilisateur / UI** : français

---

## Structure des supports

### Cours
```
H1 — Titre du cours
  H2 — Introduction (contexte professionnel, objectif, prérequis)
  H2 — Concept 1
    H3 — Définition
    H3 — Exemple concret
    H3 — À retenir / Piège classique
  H2 — Concept 2
  …
  H2 — Résumé du chapitre (points clés en gras)
  H2 — Exercices (liens vers les exercices et TP)
  H2 — Pour aller plus loin (ressources officielles uniquement)
```

### Exercices
```
Objectif pédagogique : [compétence REAC visée]
Prérequis : [cours ou notions nécessaires]
Consignes numérotées (1, 2, 3…)
Critères de réussite observables (ce que l'apprenant doit être capable de montrer)
```

### TP (Travaux Pratiques)
```
Contexte professionnel simulé (client fictif, besoin réel)
Livrables attendus (fichiers, dépôt Git, démonstration…)
Étapes guidées
Barème indicatif (sur 20 ou en points de compétences)
```

### Projets fil-rouge
```
Cahier des charges (contexte, personas, périmètre)
User stories (format : En tant que… je veux… afin de…)
Contraintes techniques (stack imposée, conventions, bonnes pratiques)
Modalités d'évaluation (critères REAC + grille de compétences)
```

### Grilles d'évaluation
Toujours inclure une **grille de compétences** alignée sur les critères de performance du REAC :
- Compétence évaluée (intitulé REAC exact)
- Niveau attendu : Non acquis / En cours d'acquisition / Acquis / Maîtrisé
- Indicateurs observables

---

## Mapping REAC DWWM V04

Utilise ce tableau pour vérifier l'alignement de chaque support :

| Dossier | Compétence REAC | Intitulé |
|---|---|---|
| CP01-ENV | CP1 | Installer et configurer son environnement de travail en fonction du projet |
| CP02-MAQUETTAGE | CP2 | Maquetter des interfaces utilisateur web ou web mobile |
| CP03-FRONTEND | CP3 | Réaliser des interfaces utilisateur statiques web ou web mobile |
| CP04-FRONTJS | CP4 | Développer la partie dynamique des interfaces utilisateur web ou web mobile |
| CP05-BDD | CP5 | Mettre en place une base de données relationnelle |
| CP06-SQL | CP6 | Développer des composants d'accès aux données SQL |
| CP07-BACKEND | CP7 | Développer des composants métier côté serveur |
| CP08-DOC | CP8 | Documenter le déploiement d'une application dynamique web ou web mobile |

> Source : REAC DWWM V04, Ministère du Travail, 29/03/2023

---

## Règles absolues

### Ce que tu ne dois **jamais** faire sans me le signaler d'abord
- Supprimer un fichier
- Modifier un schéma ou diagramme (UML, maquette, MCD/MLD)
- Changer la structure d'un dossier
- Utiliser une version dépréciée d'un framework ou langage

### Ce que tu dois **toujours** faire
- Indiquer les versions en en-tête de chaque support
- Vérifier l'alignement avec le REAC avant de valider un contenu
- Signaler explicitement si une notion dépasse le périmètre DWWM (hors référentiel)
- Attendre ma validation avant toute modification de fichier existant
- Proposer les ressources officielles uniquement (MDN, doc officielle, RFC, pas W3Schools comme source principale)
