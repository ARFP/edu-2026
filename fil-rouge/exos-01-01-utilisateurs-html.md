# Développer les UI « Compte Utilisateur »

## Compétences

Développer des interfaces utilisateur.


### Objectifs
- Produire des pages HTML sémantiques 
- Respecter les bonnes pratiques d'accessibilité 
- Structurer correctement les formulaires 
- Préparer les futures intégrations CSS et JavaScript

### Contraintes
- ✅ HTML5 uniquement
- ✅ Respect des balises sémantiques
- ✅ Respect de l'accessibilité
- ✅ Navigation fonctionnelle entre les pages
- ❌ Aucun CSS
- ❌ Aucun JavaScript

---

## Synthèse

Votre équipe doit développer la partie HTML du module **compte utilisateur** de l'un des projets suivants :

- [jeBouquine](./jebouquine/)
- [MonPetitKiosque](./monpetitkiosque/)
- [OutsideEat](./outside-eat/)

> [!WARNING]
> Aucun style CSS ni comportement JavaScript ne doit être implémenté.

### Travail demandé

Créer les pages suivantes :

```text
/
│
├── index.html (Accueil)
├── profil.html
├── inscription.html
├── connexion.html
├── mot-de-passe-oublie.html
├── mot-de-passe.html
├── profil-edition.html
├── adresses.html
├── adresses-edition.html
├── dashboard.html
```

### Livrables attendus

- 📂 Arborescence complète du projet
- 📄 Pages HTML valides
- 🔗 Navigation fonctionnelle

### Critères d'évaluation

| Critère | Points |
|----------|---------:|
| Structure HTML5 | 20 |
| Sémantique | 20 |
| Formulaires | 20 |
| Accessibilité | 20 |
| Navigation | 20 |

**Total : 100 points**

---

## Exercice 1 – Créer la page d'accueil

### Objectifs

- Découvrir les balises de structure HTML5
- Implémenter la structure d'un site web

### Contexte

Un visiteur découvre le service pour la première fois

### Consignes

Créer une page contenant :

#### En-tête

- Logo du projet (cliquer sur le logo redirige vers la page d'accueil)
- Nom du projet 
- Lien vers la connexion
- Lien vers l'inscription

#### Zone principale

- Titre principal
- Zone de présentation
- Bouton ou lien « Créer un compte »

#### Pied de page (liens)

- Mention "*© Copyright Nom de l'équipe*"
- Lien vers la page "*Mentions légales*"
- Lien vers la page "*Conditions générales de vente*"
- Lien vers la page "*RGPD*"
- Lien vers le formulaire de contact
- Lien vers "[https://crm68.fr](https://crm68.fr)"

**Pour vous aider**

- [Mentions sur votre site internet : les obligations à respecter](https://www.economie.gouv.fr/entreprises/developper-son-entreprise/innover-et-numeriser-son-entreprise/mentions-sur-votre-site-internet-les-obligations-respecter)
- [Quelles sont les mentions légales pour un site internet professionnel ?](https://www.francenum.gouv.fr/guides-et-conseils/developpement-commercial/site-web/quelles-sont-les-mentions-legales-pour-un-site)
- [Le règlement général sur la protection des données (RGPD), mode d’emploi](https://www.economie.gouv.fr/entreprises/gerer-son-entreprise-au-quotidien/assurer-sa-cybersecurite-et-la-protection-de-ses/le)
- [Conditions générales de vente : quelles mentions sont obligatoires ?](https://www.economie.gouv.fr/dgccrf/les-fiches-pratiques/conditions-generales-de-vente-quelles-mentions-sont-obligatoires)

### Critères de réussite

- [ ] Structure HTML valide
- [ ] Balises sémantiques utilisées
    - `<header>, <nav>, <main>, <section>, <article>, <footer>`
- [ ] Hiérarchie des titres cohérente
    - ❌ `<h1> <h3> <h2> <h4>`
    - ✅ `<h1> <h2> <h3> <h4>`

---

## 1 – Créer la page Profil utilisateur

**Objectif**
- Afficher des informations utilisateur

**Consignes**

Créer une page contenant :

**Informations personnelles**

- Nom
- Prénom
- Email
- Téléphone

### Informations spécifiques au projet (à compléter si besoin)

#### jeBouquine

- Genre littéraire préféré
- Auteur favori

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

## Exercice 2 – Créer la page d'inscription

### Objectif pédagogique

Structurer un formulaire complet.

### Consignes

Créer un formulaire comprenant :

#### Informations personnelles

- Nom
- Prénom

#### Informations de connexion

- Adresse email
- Mot de passe
- Confirmation du mot de passe 

#### Champs supplémentaires 

- A compléter selon votre projet

#### Validation

- Case à cocher d'acceptation des CGV (avec un lien vers les CGV)
- Case à cocher d'acceptation des règles de confidentialité (avec un lien vers la page RGPD)
- Bouton d'inscription

### Balises attendues

```html
<form>
<fieldset>
<legend>
<label>
<input>
```

### Critères de réussite

- [ ] Tous les champs possèdent un label
- [ ] Les champs sont regroupés dans des fieldsets
- [ ] Le formulaire est accessible

---

## Exercice 3 – Créer la page de connexion

### Objectif pédagogique

Concevoir un formulaire d'authentification.

### Consignes

Créer une page contenant :

#### Formulaire

- Adresse email
- Mot de passe

#### Actions

- Bouton « Se connecter »
- Lien « Mot de passe oublié »
- Lien « Créer un compte »

### Critères de réussite

- Formulaire fonctionnel
- Navigation cohérente
- Structure accessible

---

## Exercice 4 – Créer la page « Mot de passe oublié »

### Objectif pédagogique

Créer une interface de récupération de compte.

### Consignes

Ajouter :

- Un titre explicite
- Un texte explicatif
- Un champ email
- Un bouton de validation

### Critères de réussite

- Structure claire
- Formulaire minimaliste
- Utilisation des balises adaptées

---



## Exercice 6 – Créer la page de modification du profil

### Objectif pédagogique

Concevoir une interface d'édition.

### Consignes

Créer un formulaire permettant de modifier :

- Nom
- Prénom
- Email
- Téléphone

Ajouter :

- Bouton Enregistrer
- Bouton Annuler

### Critères de réussite

- Structure cohérente
- Formulaire accessible
- Champs correctement identifiés

---

## Exercice 7 – Créer la page de changement de mot de passe

### Objectif pédagogique

Structurer un formulaire sécurisé.

### Consignes

Créer un formulaire contenant :

- Mot de passe actuel
- Nouveau mot de passe
- Confirmation du nouveau mot de passe

Ajouter :

- Bouton Modifier le mot de passe

### Critères de réussite

- Utilisation du type `password`
- Formulaire clair
- Accessibilité respectée

---

## Exercice 8 – Créer la page de gestion des adresses

### Objectif pédagogique

Structurer l'affichage d'une collection de données.

### Contexte

Un utilisateur peut enregistrer plusieurs adresses.

### Consignes

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

### Balises recommandées

```html
<section>
<article>
<button>
```

### Critères de réussite

- Structure réutilisable
- Données clairement séparées
- Organisation logique

---

## Exercice 9 – Créer le tableau de bord utilisateur

### Objectif pédagogique

Assembler plusieurs composants HTML.

### Consignes

Créer une interface contenant :

#### Zone de navigation

- Profil
- Adresses
- Commandes
- Déconnexion

#### Contenu principal

- Message de bienvenue
- Résumé du compte
- Dernières activités

### Critères de réussite

- Organisation claire
- Navigation identifiable
- Structure sémantique correcte

---

## Exercice 10 – Relier l'ensemble des pages

### Objectif pédagogique

Construire une navigation complète.

### Consignes

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

### Critères de réussite

- Tous les liens sont fonctionnels
- Navigation cohérente
- Arborescence claire

---


