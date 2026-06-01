```markdown
Module      : CP00-BASES / CP01-ENV (Partie 1)
Type        : PLAN DE COURS DÉTAILLÉ
Versions    : Git 2.x, Docker V2, Markdown
REAC        : DWWM V04 — Compétences transversales & CP1
Auteur      : [Votre Prénom NOM]
Mise à jour : 2026-06

```

---

## Module 1 : Fondations, Algorithmique et Versioning

Ce module pose les bases de la logique de programmation, de la gestion de version et de la conteneurisation. Toutes les pratiques sont ancrées dans des contextes professionnels réels.

---

## Chapitre 1 : L'Environnement et le Versioning (Fil Rouge - Partie 1)

### 1. Cours : Introduction à Git et au Markdown

* **Introduction** : Contexte collaboratif en entreprise. Pourquoi versionner son code ? Qu'est-ce que la méthode FALC pour documenter ?


* **Concept 1 : Le flux Git local**
* *Définition* : Le répertoire de travail, la zone d'index (Staging Area), et le dépôt local (Repository).
* *À retenir* : Un commit est un instantané immuable du code.


* **Concept 2 : La syntaxe Markdown**
* *Définition* : Format textuel léger pour rédiger des documentations claires (`#`, `##`, ``, `*`).





### 2. Démo : Premier dépôt et premier README

* Création d'un dossier de projet sur le poste de travail.
* Initialisation avec `git init`.
* Création d'un fichier `README.md` décrivant un projet fictif de **Gestion d'utilisateurs**.


* Utilisation des commandes `git status`, `git add README.md`, et `git commit -m "doc: initialisation du projet"`.

### 3. Exercice d'application

* **Objectif** : Maîtriser le cycle de commit local.
* **Consignes** :
1. Créer un fichier `CONTRIBUTING.md` dans le dossier précédent.
2. Rédiger à l'intérieur les règles de nommage des fichiers en Markdown.
3. Indexer le fichier et valider le commit avec un message explicite.


* **Critères de réussite** : La commande `git log` doit afficher deux commits distincts et propres.

---

## Chapitre 2 : Les Variables et les Structures Conditionnelles

### 1. Cours : Stocker et Choisir

* **Introduction** : Comment un ordinateur mémorise une information et prend une décision selon un contexte métier.


* **Concept 1 : Les variables et types de données**
* *Définition* : Espaces mémoires nommés stockant des chaînes de caractères (String), des nombres (Integer/Float) ou des booléens (True/False).




* **Concept 2 : Les structures conditionnelles (Si... Sinon)**
* *Définition* : Permet d'aiguiller le comportement du programme selon la valeur d'une condition.





### 2. Démo : Algorithme du Distributeur de Boissons

* Écriture d'un algorithme en pseudo-code pour l'**Application distributeur de boissons** :


```text
VARIABLE stockBoisson : Entier <- 5
VARIABLE prixBoisson : Réel <- 1.50
VARIABLE argentInsere : Réel <- 2.00

SI stockBoisson > 0 ALORS
    SI argentInsere >= prixBoisson ALORS
        AFFICHER "Boisson distribuée"
        VARIABLE monnaieARendre : Réel <- argentInsere - prixBoisson
        AFFICHER "Monnaie à rendre : " + monnaieARendre
    SINON
        AFFICHER "Montant insuffisant"
    FIN SI
SINON
    AFFICHER "Produit épuisé"
FIN SI

```


### 3. Exercice d'application
*   **Objectif** : Manipuler les variables et les conditions.
*   **Consignes** :
    1. Écrire le pseudo-code pour le système de **Gestion d'utilisateurs**[cite: 2].
    2. Créer une variable `ageUtilisateur` et une variable `estBanni` (booléen).
    3. Écrire la condition : si l'utilisateur a plus de 18 ans et n'est pas banni, afficher "Accès autorisé". Sinon, afficher "Accès refusé".
*   **Critères de réussite** : Le pseudo-code doit couvrir tous les cas de figure possibles (mineur, majeur banni, majeur non banni).

---

## Chapitre 3 : Les Structures Répétitives (Boucles)

### 1. Cours : Automatiser les tâches répétitives
*   **Introduction** : Éviter la répétition manuelle de lignes de code identiques.
*   **Concept 1 : La boucle "Tant Que" (While)**
    *   *Définition* : Répète un bloc de code tant qu'une condition reste vraie[cite: 2].
*   **Concept 2 : La boucle "Pour" (For)**
    *   *Définition* : Répète un bloc de code un nombre de fois déterminé à l'avance[cite: 2].

### 2. Démo : Remplissage automatique du distributeur
*   Pseudo-code simulant le chargement de canettes dans l'**Application distributeur de boissons**[cite: 2] :
```text
VARIABLE capaciteMax : Entier <- 10
VARIABLE canettesActuelles : Entier <- 3

TANT QUE canettesActuelles < capaciteMax
    canettesActuelles <- canettesActuelles + 1
    AFFICHER "Ajout d'une canette. Total : " + canettesActuelles
FIN TANT QUE
AFFICHER "Le distributeur est plein."

```

### 3. Exercice d'application

* **Objectif** : Utiliser une boucle pour parcourir ou générer des données.
* **Consignes** :
1. Écrire l'algorithme pour le **Système de réservation de trajets**.


2. Un conducteur propose 4 places dans son véhicule.
3. Simuler l'affichage du message "Place numéro X disponible" pour chaque place de 1 à 4 à l'aide d'une boucle "Pour".


* **Critères de réussite** : L'affichage doit s'arrêter strictement à la 4ème place.

---

## Travail Pratique (TP) : Logique de l'Application Distributeur de Boissons

### Contexte professionnel simulé

La société "Automate-Express" demande de concevoir la logique algorithmique de son nouveau distributeur de boissons connecté. Vous devez modéliser la sélection, le paiement et le rendu de monnaie défensif (anticiper les erreurs de saisie).

### Livrables attendus

* Un fichier `ALGORITHME.md` rédigé en Markdown contenant le pseudo-code complet.


* Un dépôt Git local contenant l'historique des modifications.



### Étapes guidées

1. **Initialisation** : Créer le fichier et documenter le contexte en Markdown. Faire un premier commit Git.


2. **Saisie utilisateur** : Déclarer les variables pour le choix de la boisson (Café = 1, Thé = 2, Eau = 3), le prix associé, et la monnaie insérée par le client.


3. **Vérification de sécurité** : Si la monnaie insérée est négative ou nulle, afficher une erreur et stopper le programme (Style défensif).


4. **Calcul et Rendu** : Gérer le calcul de la monnaie à rendre à l'aide des structures conditionnelles apprises.


5. **Sauvegarde** : Valider le TP avec un commit final nommé `feat: algorithme complet du distributeur`.



### Barème indicatif (Sur 20 points)

* Structure du Markdown claire et lisible (FALC) : 4 points


* Utilisation correcte et typage logique des variables : 4 points


* Gestion de la sécurité (Style défensif sur les entrées) : 4 points


* Exactitude de la logique de rendu de monnaie : 5 points


* Utilisation correcte des commits Git : 3 points



---

## Mini-Projet : Système de Validation d'Identifiants (Gestion d'utilisateurs)

### Description de la tâche (Niveau 6 de Bloom - Créer)

Pour clôturer ce premier module, les apprenants doivent concevoir un algorithme autonome de sécurité pour le système de **Gestion d'utilisateurs**. L'algorithme doit bloquer un compte après 3 tentatives infructueuses de connexion.

### Spécifications

1. Le programme possède un `identifiantCorrect` et un `motDePasseCorrect` enregistrés en mémoire.
2. Une boucle doit permettre à l'utilisateur de tenter de se connecter jusqu'à **3 fois maximum**.
3. À chaque tentative, si les saisies correspondent, afficher "Connexion réussie" et quitter la boucle.
4. Si les saisies sont fausses, décrémenter le nombre d'essais restants et afficher "Identifiants incorrects. Il vous reste X essais".
5. Si le nombre d'essais atteint 0, afficher "Compte verrouillé par sécurité".



### Grille d'évaluation du Mini-Projet

| Niveau d'acquisition | Indicateurs Observables |
| --- | --- |
| **Non acquis** | L'algorithme ne gère pas le décompte des essais ou boucle à l'infini. |
| **En cours d'acquisition** | La boucle fonctionne mais les messages de sécurité ou les variables ne sont pas cohérents. |
| **Acquis** | Le compte se bloque exactement après 3 essais erronés. Le code est commit sur Git. |
| **Maîtrisé** | Le style défensif est appliqué (gestion des saisies vides) et le README est parfaitement documenté. |