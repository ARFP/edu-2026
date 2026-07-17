# Série 3 – Dynamiser le module « Compte Utilisateur » avec JavaScript

## REAC DWWM 2023 – CP3

### Compétences

Développer la partie dynamique des interfaces utilisateur.

### Objectifs de la série

Cette troisième série a pour objectif d'ajouter de l'interactivité aux interfaces développées lors des séries précédentes.

Vous allez :

- Manipuler le DOM (Document Object Model) 
- Gérer les événements utilisateurs 
- Valider les formulaires 
- Stocker des données localement 
- Simuler des échanges avec une API 
- Gérer l'état d'un utilisateur connecté

### Prérequis

- [Série 1](./exos-01-01-utilisateurs-html) terminée (HTML)
- [Série 2](./exos-01-02-utilisateurs-css) terminée (CSS)
- Notions de JavaScript ES2023 
    - Entrainez-vous avec les [exercices d'introduction](https://arfp.github.io/tp/web/javascript/)

### Contraintes

- JavaScript natif
- Aucun framework 
- Approche modulaire
- Respect de l'accessibilité
- Code commenté

---

# Exercice 1 – Afficher un message de bienvenue

## Objectif pédagogique

Manipuler le DOM.

## Consignes

Sur la page d'accueil :

- sélectionner un élément HTML ;
- modifier son contenu avec JavaScript ;
- afficher un message personnalisé.

### Exemple

```text
Bienvenue sur OutsideEat
```

ou

```text
Bienvenue sur jeBouquine
```

ou

```text
Bienvenue sur MonPetitKiosque
```

## Concepts travaillés

```javascript
querySelector()
textContent
```

## Critères de réussite

- Sélection correcte de l'élément dans le DOM
- Modification visible du contenu
- Code lisible et commenté

---

# Exercice 2 – Valider le formulaire d'inscription

## Objectif pédagogique

Contrôler les données utilisateur.

## Consignes

Vérifier :

### Nom

- obligatoire

### Prénom

- obligatoire

### Email

- obligatoire
- format valide

### Mot de passe

- minimum 8 caractères

### Confirmation

- identique au mot de passe

## Messages attendus

```text
Adresse email invalide.
```

```text
Les mots de passe sont différents.
```

## Concepts travaillés

```javascript
addEventListener()
preventDefault()
```

## Critères de réussite

- Validation fonctionnelle
- Messages d'erreur explicites
- Aucun rechargement inutile

---

# Exercice 3 – Afficher les erreurs directement sous les champs

## Objectif pédagogique

Améliorer l'expérience utilisateur.

## Consignes

En cas d'erreur :

- afficher le message sous le champ concerné ;
- supprimer le message lorsque la donnée est corrigée.

## Concepts travaillés

```javascript
createElement()
append()
remove()
```

## Critères de réussite

- Messages contextualisés
- Interface claire
- Gestion propre des erreurs

---

# Exercice 4 – Afficher la force du mot de passe

## Objectif pédagogique

Manipuler les chaînes de caractères.

## Consignes

Créer un indicateur :

```text
Faible
```

```text
Moyen
```

```text
Fort
```

Le niveau dépend :

- de la longueur ;
- des chiffres ;
- des caractères spéciaux ;
- des majuscules.

## Critères de réussite

- Mise à jour en temps réel
- Règles cohérentes
- Retour utilisateur immédiat

---

# Exercice 5 – Simuler la création d'un compte

## Objectif pédagogique

Manipuler des objets JavaScript.

## Consignes

Construire un objet utilisateur :

```javascript
{
    nom: "",
    prenom: "",
    email: ""
}
```

Afficher son contenu dans la console.

## Bonus

Afficher les informations dans une carte HTML.

## Critères de réussite

- Objet correctement créé
- Récupération des données du formulaire
- Affichage conforme

---

# Exercice 6 – Simuler une authentification

## Objectif pédagogique

Gérer un scénario de connexion.

## Consignes

Créer un utilisateur fictif :

```javascript
const utilisateur = {
    email: "admin@test.fr",
    password: "Password123"
};
```

Autoriser la connexion uniquement si :

- email correct ;
- mot de passe correct.

## Affichages attendus

```text
Connexion réussie.
```

ou

```text
Identifiants incorrects.
```

## Critères de réussite

- Comparaison correcte
- Gestion des erreurs
- Messages adaptés

---

# Exercice 7 – Sauvegarder l'utilisateur connecté

## Objectif pédagogique

Découvrir le stockage local.

## Consignes

Après connexion :

enregistrer dans :

```javascript
localStorage
```

les informations suivantes :

- nom ;
- prénom ;
- email.

## Concepts travaillés

```javascript
localStorage.setItem()
JSON.stringify()
```

## Critères de réussite

- Données enregistrées
- Persistance après rechargement
- Vérification possible via les outils développeur

---

# Exercice 8 – Afficher les informations du profil

## Objectif pédagogique

Lire des données enregistrées.

## Consignes

Sur la page Profil :

- récupérer les données du localStorage ;
- afficher les informations de l'utilisateur.

## Concepts travaillés

```javascript
localStorage.getItem()
JSON.parse()
```

## Critères de réussite

- Données correctement lues
- Affichage dynamique
- Aucun contenu codé en dur

---

# Exercice 9 – Modifier son profil

## Objectif pédagogique

Mettre à jour des données utilisateur.

## Consignes

Au chargement :

- préremplir le formulaire.

À la validation :

- mettre à jour les informations enregistrées.

## Critères de réussite

- Préremplissage automatique
- Sauvegarde fonctionnelle
- Confirmation utilisateur

---

# Exercice 10 – Changer son mot de passe

## Objectif pédagogique

Manipuler plusieurs validations.

## Consignes

Vérifier :

- ancien mot de passe ;
- nouveau mot de passe ;
- confirmation.

Refuser la modification lorsque :

- l'ancien mot de passe est incorrect ;
- la confirmation ne correspond pas.

## Critères de réussite

- Contrôles cohérents
- Messages explicites
- Logique métier respectée

---

# Exercice 11 – Gérer plusieurs adresses

## Objectif pédagogique

Manipuler des tableaux d'objets.

## Consignes

Créer un tableau :

```javascript
const adresses = [];
```

Ajouter une adresse via un formulaire.

Afficher automatiquement la liste.

## Structure proposée

```javascript
{
    libelle: "",
    rue: "",
    codePostal: "",
    ville: ""
}
```

## Critères de réussite

- Ajout fonctionnel
- Liste mise à jour automatiquement
- Affichage propre

---

# Exercice 12 – Supprimer une adresse

## Objectif pédagogique

Manipuler les tableaux.

## Consignes

Ajouter un bouton :

```text
Supprimer
```

pour chaque adresse.

Supprimer l'adresse sélectionnée.

## Concepts travaillés

```javascript
filter()
splice()
```

## Critères de réussite

- Suppression immédiate
- Interface mise à jour
- Données cohérentes

---

# Exercice 13 – Générer dynamiquement le tableau de bord

## Objectif pédagogique

Créer des composants avec JavaScript.

## Consignes

Afficher automatiquement :

- nom utilisateur ;
- email ;
- nombre d'adresses ;
- date de dernière connexion.

Les données doivent être générées dynamiquement.

## Critères de réussite

- DOM généré par JavaScript
- Données dynamiques
- Organisation claire

---

# Exercice 14 – Déconnexion utilisateur

## Objectif pédagogique

Gérer une session utilisateur.

## Consignes

Créer un bouton :

```text
Déconnexion
```

Au clic :

- supprimer les données enregistrées ;
- rediriger vers la page d'accueil.

## Concepts travaillés

```javascript
removeItem()
clear()
location.href
```

## Critères de réussite

- Données supprimées
- Redirection fonctionnelle
- Session fermée

---

# Exercice 15 – Simulation d'appel API

## Objectif pédagogique

Préparer la communication avec un back-end.

## Consignes

Effectuer un appel vers :

```javascript
https://jsonplaceholder.typicode.com/users
```

Afficher :

- nom ;
- email ;
- téléphone.

## Concepts travaillés

```javascript
fetch()
async/await
try/catch
```

## Critères de réussite

- Appel réussi
- Données affichées
- Gestion des erreurs

---

# TP de Synthèse

## TP 3 – Développer le module utilisateur complet

### Contexte

Vous devez rendre entièrement fonctionnel le module utilisateur développé lors des deux séries précédentes.

### Fonctionnalités attendues

✅ Inscription

✅ Connexion

✅ Validation des formulaires

✅ Gestion du profil

✅ Gestion des adresses

✅ Stockage local

✅ Déconnexion

✅ Tableau de bord dynamique

---

## Livrables attendus

```text
/
│
├── css/
│   └── style.css
│
├── js/
│   ├── app.js
│   ├── auth.js
│   ├── profil.js
│   ├── adresses.js
│   └── dashboard.js
│
├── index.html
├── inscription.html
├── connexion.html
├── mot-de-passe-oublie.html
├── dashboard.html
├── profil.html
├── profil-edition.html
├── mot-de-passe.html
└── adresses.html
```

---

## Critères d'évaluation

| Critère | Points |
|----------|---------:|
| Manipulation du DOM | 20 |
| Gestion des événements | 20 |
| Validation des formulaires | 20 |
| Gestion du stockage local | 20 |
| Qualité du code JavaScript | 20 |

**Total : 100 points**

---

## Durée estimée

**15 à 20 heures**

---

## Résultat attendu

À l'issue des trois séries, l'apprenant dispose d'un module utilisateur complet :

```text
HTML
↓
CSS
↓
JavaScript
```

Ce module pourra ensuite être connecté à une API Symfony/Laravel/Node.js dans les futures séquences consacrées :

- à l'authentification JWT ;
- à la consommation d'API REST ;
- au développement des fonctionnalités métier propres à :
  - jeBouquine ;
  - MonPetitKiosque ;
  - OutsideEat.