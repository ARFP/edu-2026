# Cahier des Charges Fonctionnel
# OutsideEat

## Plateforme de commande et de livraison de repas pour le CRM

**Version : 1.1**

**Type de projet :** Application web de restauration et livraison

**Méthodologie recommandée :** Agile / Scrum

**Public visé :**
- Étudiants
- Résidents
- Personnel du CRM
- Restaurateurs partenaires
- Livreurs

---

# 1. Présentation du projet

## Contexte

Le CRM souhaite mettre à disposition une plateforme unique permettant aux étudiants, résidents et personnels de commander des repas auprès :

- de la cafétéria interne ;
- de restaurants partenaires.

Les commandes peuvent être :

- livrées en chambre ;
- livrées en salle de cours ;
- récupérées en click & collect.

L'objectif est d'améliorer l'expérience utilisateur tout en simplifiant la gestion des commandes et des livraisons. 【1-bdeb22】

---

# 2. Objectifs métier

## Objectifs fonctionnels

Le système doit permettre :

- la consultation des menus ;
- la personnalisation des plats ;
- la commande en ligne ;
- le paiement sécurisé ;
- le suivi des livraisons ;
- la gestion des menus et des stocks ;
- l'administration globale de la plateforme.

## Objectifs stratégiques

- Réduire les files d'attente.
- Améliorer le confort des résidents.
- Centraliser les offres de restauration.
- Faciliter la gestion des commandes.
- Développer les partenariats avec des restaurateurs locaux.

---

# 3. Périmètre fonctionnel

## Inclus

✅ Catalogue de menus

✅ Gestion des comptes utilisateurs

✅ Paiement en ligne

✅ Suivi des commandes

✅ Gestion des livraisons

✅ Gestion des menus

✅ Gestion des stocks

✅ Tableau de bord administrateur

✅ Gestion des promotions

---

## Hors périmètre (Version 1)

❌ Livraison hors CRM

❌ Programme de fidélité

❌ Application mobile native

❌ Marketplace ouverte

❌ Livraison par prestataires externes

---

# 4. Personas

## Persona 1 : Étudiant résident

### Profil

- 20 ans
- Logé au CRM

### Besoins

- Commander rapidement.
- Être livré en chambre.
- Payer facilement avec son téléphone.

### Frustrations

- Temps d'attente.
- Multiplication des points de commande.

---

## Persona 2 : Personnel administratif

### Profil

- Travaille toute la journée sur le campus.

### Besoins

- Réserver son repas à l'avance.
- Choisir un créneau précis.

---

## Persona 3 : Restaurateur partenaire

### Profil

- Commerce local partenaire du CRM.

### Besoins

- Gérer ses menus.
- Consulter les commandes.
- Suivre ses ventes.

---

## Persona 4 : Livreur

### Profil

- Personnel de livraison.

### Besoins

- Voir les commandes à livrer.
- Optimiser ses déplacements.
- Confirmer les livraisons.

---

# 5. User Stories

## EPIC 1 – Gestion des comptes

### US-001

**En tant qu'utilisateur**

Je souhaite créer un compte

Afin de pouvoir passer commande.

### US-002

**En tant qu'utilisateur**

Je souhaite me connecter

Afin d'accéder à mon espace personnel.

---

## EPIC 2 – Consultation des menus

### US-003

**En tant qu'utilisateur**

Je souhaite consulter les menus

Afin de choisir mes repas.

### US-004

**En tant qu'utilisateur**

Je souhaite rechercher ou filtrer des plats

Afin de trouver rapidement ce qui m'intéresse.

---

## EPIC 3 – Commande

### US-005

**En tant qu'utilisateur**

Je souhaite personnaliser un plat

Afin de l'adapter à mes préférences ou allergies.

### US-006

**En tant qu'utilisateur**

Je souhaite ajouter des plats à mon panier

Afin de préparer ma commande.

### US-007

**En tant qu'utilisateur**

Je souhaite payer ma commande

Afin de confirmer mon achat.

---

## EPIC 4 – Livraison

### US-008

**En tant qu'utilisateur**

Je souhaite choisir un mode de livraison

Afin de recevoir mon repas où je le souhaite.

### US-009

**En tant qu'utilisateur**

Je souhaite suivre ma commande

Afin de connaître son avancement.

### US-010

**En tant que livreur**

Je souhaite visualiser les commandes à livrer

Afin d'effectuer les livraisons.

### US-011

**En tant que livreur**

Je souhaite confirmer une livraison

Afin de clôturer la commande.

---

## EPIC 5 – Gestion restaurant

### US-012

**En tant que restaurateur**

Je souhaite gérer mes menus

Afin de maintenir mon offre à jour.

### US-013

**En tant que restaurateur**

Je souhaite gérer mes stocks

Afin d'éviter les ruptures.

### US-014

**En tant que restaurateur**

Je souhaite créer des promotions

Afin d'augmenter mes ventes.

---

## EPIC 6 – Administration CRM

### US-015

**En tant qu'administrateur**

Je souhaite gérer les utilisateurs

Afin de sécuriser la plateforme.

### US-016

**En tant qu'administrateur**

Je souhaite gérer les zones de livraison

Afin d'adapter le service aux contraintes du CRM.

### US-017

**En tant qu'administrateur**

Je souhaite consulter un tableau de bord global

Afin de piloter l'activité.

---

# 6. Critères d'acceptation Gherkin

## US-001 – Création de compte

```gherkin
Feature: Création de compte

Scenario: Inscription valide
    Given je suis sur la page d'inscription
    When je renseigne les informations obligatoires
    And je valide le formulaire
    Then mon compte est créé
```

---

## US-003 – Consultation des menus

```gherkin
Feature: Consultation des menus

Scenario: Affichage des menus
    Given des menus sont disponibles
    When j'accède à la page catalogue
    Then la liste des menus est affichée
```

---

## US-005 – Personnalisation d'un plat

```gherkin
Feature: Personnalisation des plats

Scenario: Ajout d'un supplément
    Given je consulte une fiche plat
    When je sélectionne un supplément
    Then le prix est recalculé
```

---

## US-006 – Ajout au panier

```gherkin
Feature: Gestion du panier

Scenario: Ajouter un plat
    Given je consulte un plat
    When je clique sur "Ajouter au panier"
    Then le plat apparaît dans le panier
```

---

## US-007 – Paiement

```gherkin
Feature: Paiement

Scenario: Paiement accepté
    Given mon panier contient des articles
    When le paiement est validé
    Then une commande est créée
    And son statut devient "Payée"
```

---

## US-008 – Choix du mode de livraison

```gherkin
Feature: Livraison

Scenario: Livraison en chambre
    Given je valide ma commande
    When je choisis "Livraison en chambre"
    Then l'adresse de livraison correspond à ma chambre
```

---

## US-009 – Suivi de commande

```gherkin
Feature: Suivi de commande

Scenario: Consultation du statut
    Given une commande existe
    When je consulte son détail
    Then son statut est affiché
```

---

## US-011 – Confirmation de livraison

```gherkin
Feature: Livraison

Scenario: Livraison terminée
    Given une commande est en cours de livraison
    When le livreur valide la remise
    Then le statut devient "Livrée"
```

---

## US-012 – Gestion des menus

```gherkin
Feature: Administration des menus

Scenario: Ajout d'un menu
    Given je suis restaurateur
    When je crée un nouveau menu
    Then celui-ci apparaît dans le catalogue
```

---

# 7. Exigences fonctionnelles

| ID | Exigence | Priorité |
|------|------|------|
| REQ-F-001 | Création de compte | Haute |
| REQ-F-002 | Authentification | Haute |
| REQ-F-003 | Consultation des menus | Haute |
| REQ-F-004 | Personnalisation des plats | Haute |
| REQ-F-005 | Gestion panier | Haute |
| REQ-F-006 | Paiement en ligne | Critique |
| REQ-F-007 | Gestion des livraisons | Critique |
| REQ-F-008 | Suivi de commande | Haute |
| REQ-F-009 | Gestion des menus | Haute |
| REQ-F-010 | Gestion des stocks | Haute |
| REQ-F-011 | Gestion des promotions | Moyenne |
| REQ-F-012 | Tableau de bord CRM | Moyenne |

---

# 8. Exigences non fonctionnelles

## Performance

| ID | Exigence |
|------|------|
| NFR-001 | Temps de réponse inférieur à 2 secondes |
| NFR-002 | Disponibilité minimale de 99 % |
| NFR-003 | Application responsive |

## Sécurité

| ID | Exigence |
|------|------|
| NFR-004 | HTTPS obligatoire |
| NFR-005 | Conformité RGPD |
| NFR-006 | Chiffrement des données sensibles |
| NFR-007 | Gestion des rôles et permissions |

## Accessibilité

| ID | Exigence |
|------|------|
| NFR-008 | Accessibilité WCAG 2.1 AA |
| NFR-009 | Compatibilité mobile |
| NFR-010 | Navigation intuitive |

---

# 9. Modèle de données conceptuel

## Utilisateur

- id
- nom
- prénom
- email
- motDePasse
- rôle

## Restaurant

- id
- nom
- description

## Plat

- id
- nom
- description
- prix
- stock

## Commande

- id
- dateCommande
- statut
- montant

## LigneCommande

- quantité
- prixUnitaire

## Livraison

- id
- typeLivraison
- adresse
- statut

## Paiement

- id
- montant
- datePaiement
- statut

## Promotion

- id
- nom
- réduction
- dateDébut
- dateFin

---

# 10. Backlog Produit Initial

## Priorité P1

- Authentification
- Catalogue des menus
- Panier
- Paiement
- Livraison
- Suivi de commande

## Priorité P2

- Gestion des stocks
- Gestion des promotions
- Notifications

## Priorité P3

- Statistiques avancées
- Programme fidélité
- Wallet CRM avancé

---

# 11. Matrice de traçabilité

| Exigence | User Story |
|-----------|------------|
| REQ-F-001 | US-001 |
| REQ-F-002 | US-002 |
| REQ-F-003 | US-003 |
| REQ-F-005 | US-006 |
| REQ-F-006 | US-007 |
| REQ-F-007 | US-008 |
| REQ-F-008 | US-009 |
| REQ-F-009 | US-012 |

---

# 12. Livrables attendus

## Analyse

- Cahier des charges
- User Stories
- Diagrammes UML
- MCD / MLD

## Développement

- Front-office utilisateur
- Portail restaurateur
- Espace livreur
- Tableau de bord CRM
- API REST

## Documentation

- Documentation technique
- Documentation utilisateur

## Qualité

- Tests unitaires
- Tests fonctionnels
- Tests d'intégration

## Livraison

- Application déployée
- Base de données
- Documentation d'exploitation

---

# 13. Planning prévisionnel

| Phase | Durée |
|---------|---------|
| Analyse & conception | 3 semaines |
| Développement | 6 à 10 semaines |
| Tests & corrections | 2 à 3 semaines |
| Déploiement | 1 semaine |
| Formation | 1 semaine |

---

# 14. Évolutions futures

- Application mobile native
- Programme de fidélité
- Notifications Push
- Commandes récurrentes
- Livraison géolocalisée
- Intégration badges CRM
- Système de notation des restaurants
- Recommandations basées sur l'historique utilisateur