# Développer la structure HTML « Compte Utilisateur »

### Compétence visée

Développer des interfaces utilisateur.

> [!NOTE]
> Objectifs
> - Produire des pages HTML sémantiques 
> - Respecter les bonnes pratiques d'accessibilité 
> - Structurer correctement les formulaires 
> - Préparer les futures intégrations CSS et JavaScript


### Contraintes

- HTML5 uniquement
- Aucun CSS personnalisé
- Aucun JavaScript
- Respect des balises sémantiques
- Respect de l'accessibilité
- Navigation fonctionnelle entre les pages

---

# Synthèse

Votre équipe doit développer la partie HTML du module compte utilisateur de l'un des projets suivants :

- jeBouquine
- MonPetitKiosque
- OutsideEat

> [!warning]
>
> Aucun style CSS ni comportement JavaScript ne doit être implémenté.

## Travail demandé

Créer les pages suivantes :

```text
/
│
├── index.html (Accueil)
├── inscription.html
├── connexion.html
├── mot-de-passe-oublie.html
├── dashboard.html
├── profil.html
├── profil-edition.html
├── mot-de-passe.html
└── adresses.html
```

## Livrables attendus

- Arborescence complète du projet
- Pages HTML valides
- Navigation fonctionnelle
- Structure accessible

## Critères d'évaluation

| Critère | Points |
|----------|---------:|
| Structure HTML5 | 20 |
| Sémantique | 20 |
| Formulaires | 20 |
| Accessibilité | 20 |
| Navigation | 20 |

**Total : 100 points**

## Durée estimée

**12 à 15 heures**

---

# Exercice 1 – Créer la page d'accueil

## Objectif pédagogique

Découvrir les balises de structure HTML5.

## Contexte

Un visiteur découvre le service pour la première fois.

Le contenu doit pouvoir être adapté aux projets :

- [jeBouquine](./jebouquine/cdc-jebouquine.md)
- [MonPetitKiosque](./monpetitkiosque/cdc-monpetitkiosque.md)
- [OutsideEat](./outside-eat/cdc-outside-eat.md)

## Consignes

Créer une page contenant :

### En-tête

- Logo du projet
- Nom du projet
- Lien vers la connexion
- Lien vers l'inscription

### Zone principale

- Titre principal
- Texte de présentation
- Bouton ou lien « Créer un compte »

### Pied de page

- Mentions légales
- Contact

## Balises à utiliser

```html
<header>, <nav>, <main>, <section>, <footer>
```

## Critères de réussite

- Structure HTML valide
- Balises sémantiques utilisées
- Hiérarchie des titres cohérente

---

# 1 – Créer la page Profil utilisateur

**Objectif**
- Afficher des informations utilisateur.

**Consignes**

Créer une page contenant :

**Informations personnelles**
- Nom
- Prénom
- Email
- Téléphone

### Informations spécifiques au projet

#### jeBouquine

- Genre(s) littéraire préféré
- Auteur(s) favori

#### MonPetitKiosque

- N° Chambre
- Batiment (Grande Aile, Tour, RF1, RF2, RF3, HDC)

#### OutsideEat

- N° Chambre
- Batiment (Grande Aile, Tour, RF1, RF2, RF3, HDC)
- Préférences alimentaires

### Critères de réussite

- [ ] Informations regroupées par sections
- [ ] Structure claire
- [ ] Utilisation de titres adaptés

---

# Exercice 2 – Créer la page d'inscription

## Objectif pédagogique

Structurer un formulaire complet.

## Consignes

Créer un formulaire comprenant :

### Informations personnelles

- Nom
- Prénom

### Informations de connexion

- Adresse email
- Mot de passe
- Confirmation du mot de passe

### Validation

- Case à cocher d'acceptation des CGU
- Bouton d'inscription

## Balises attendues

```html
<form>
<fieldset>
<legend>
<label>
<input>
```

## Critères de réussite

- Tous les champs possèdent un label
- Les champs sont regroupés dans des fieldsets
- Le formulaire est accessible

---

# Exercice 3 – Créer la page de connexion

## Objectif pédagogique

Concevoir un formulaire d'authentification.

## Consignes

Créer une page contenant :

### Formulaire

- Adresse email
- Mot de passe

### Actions

- Bouton « Se connecter »
- Lien « Mot de passe oublié »
- Lien « Créer un compte »

## Critères de réussite

- Formulaire fonctionnel
- Navigation cohérente
- Structure accessible

---

# Exercice 4 – Créer la page « Mot de passe oublié »

## Objectif pédagogique

Créer une interface de récupération de compte.

## Consignes

Ajouter :

- Un titre explicite
- Un texte explicatif
- Un champ email
- Un bouton de validation

## Critères de réussite

- Structure claire
- Formulaire minimaliste
- Utilisation des balises adaptées

---



# Exercice 6 – Créer la page de modification du profil

## Objectif pédagogique

Concevoir une interface d'édition.

## Consignes

Créer un formulaire permettant de modifier :

- Nom
- Prénom
- Email
- Téléphone

Ajouter :

- Bouton Enregistrer
- Bouton Annuler

## Critères de réussite

- Structure cohérente
- Formulaire accessible
- Champs correctement identifiés

---

# Exercice 7 – Créer la page de changement de mot de passe

## Objectif pédagogique

Structurer un formulaire sécurisé.

## Consignes

Créer un formulaire contenant :

- Mot de passe actuel
- Nouveau mot de passe
- Confirmation du nouveau mot de passe

Ajouter :

- Bouton Modifier le mot de passe

## Critères de réussite

- Utilisation du type `password`
- Formulaire clair
- Accessibilité respectée

---

# Exercice 8 – Créer la page de gestion des adresses

## Objectif pédagogique

Structurer l'affichage d'une collection de données.

## Contexte

Un utilisateur peut enregistrer plusieurs adresses.

## Consignes

Afficher plusieurs adresses sous forme de liste.

Chaque adresse contient :

- Libellé
- Rue
- Code postal
- Ville

Ajouter :

- Bouton Modifier
- Bouton Supprimer
- Bouton Ajouter une adresse

## Balises recommandées

```html
<section>
<article>
<button>
```

## Critères de réussite

- Structure réutilisable
- Données clairement séparées
- Organisation logique

---

# Exercice 9 – Créer le tableau de bord utilisateur

## Objectif pédagogique

Assembler plusieurs composants HTML.

## Consignes

Créer une interface contenant :

### Zone de navigation

- Profil
- Adresses
- Commandes
- Déconnexion

### Contenu principal

- Message de bienvenue
- Résumé du compte
- Dernières activités

## Critères de réussite

- Organisation claire
- Navigation identifiable
- Structure sémantique correcte

---

# Exercice 10 – Relier l'ensemble des pages

## Objectif pédagogique

Construire une navigation complète.

## Consignes

Créer les liens entre les pages :

```text
Accueil
│
├── Inscription
├── Connexion
├── Mot de passe oublié
│
└── Tableau de bord
    ├── Profil
    ├── Modifier profil
    ├── Changer mot de passe
    └── Adresses
```

## Critères de réussite

- Tous les liens sont fonctionnels
- Navigation cohérente
- Arborescence claire

---


