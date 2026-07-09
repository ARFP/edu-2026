# Cahier des Charges Fonctionnel
# MonPetitKiosque

**Version : 1.1**

**Type de projet :** Application web e-commerce hospitalière

**Méthodologie recommandée :** Agile / Scrum

**Public visé :**
- Patients
- Visiteurs
- Personnel hospitalier

---

# 1. Présentation du projet

## Contexte

MonPetitKiosque est une plateforme web permettant aux patients, visiteurs et personnels hospitaliers d’acheter des articles non périssables disponibles dans le kiosque de l’établissement.

Les produits peuvent être retirés :

- directement au kiosque pendant les horaires d’ouverture ;
- dans des casiers automatiques accessibles 24h/24 et 7j/7.

L'objectif est d'améliorer l'autonomie des utilisateurs tout en réduisant la charge opérationnelle du personnel. 【1-d48146】

---

# 2. Objectifs métier

## Objectifs fonctionnels

L'application doit permettre :

- la consultation d'un catalogue de produits ;
- l'achat en ligne sécurisé ;
- la gestion du retrait via casiers ;
- la gestion des stocks ;
- la gestion administrative des produits et commandes ;
- le suivi des retraits.

## Objectifs stratégiques

- Moderniser les services du kiosque hospitalier.
- Augmenter l'accessibilité aux produits.
- Réduire les files d'attente.
- Offrir un service disponible hors horaires d'ouverture.
- Préparer l'ouverture vers d'autres services hospitaliers.

---

# 3. Périmètre fonctionnel

## Produits proposés

### Presse

- Magazines
- Journaux

### Culture

- Livres
- Revues

### Loisirs

- Sudoku
- Mots croisés

### Hygiène

- Savons
- Mouchoirs
- Gel hydroalcoolique

### Accessoires

- Chargeurs
- Écouteurs
- Stylos
- Carnets

### Alimentaire longue conservation

- Snacks emballés
- Boissons longue conservation

## Hors périmètre

- Produits frais
- Produits réfrigérés
- Médicaments
- Produits nécessitant une chaîne du froid

---

# 4. Personas

## Persona 1 : Patient hospitalisé

### Profil

- Âge : 68 ans
- Mobilité réduite

### Besoins

- Commander facilement.
- Pouvoir retirer une commande à tout moment.
- Interface accessible.

---

## Persona 2 : Visiteur

### Profil

- Visite ponctuelle.

### Besoins

- Acheter rapidement un article.
- Trouver facilement un produit.

---

## Persona 3 : Gestionnaire du kiosque

### Profil

- Personnel administratif.

### Besoins

- Gérer les stocks.
- Préparer les commandes.
- Superviser les casiers.

---

# 5. User Stories

## EPIC 1 – Consultation du catalogue

### US-001

**En tant que** visiteur

**Je souhaite** consulter le catalogue

**Afin de** découvrir les produits disponibles.

### US-002

**En tant que** utilisateur

**Je souhaite** rechercher un produit

**Afin de** le retrouver rapidement.

---

## EPIC 2 – Gestion du panier

### US-003

**En tant que** utilisateur

**Je souhaite** ajouter un produit au panier

**Afin de** préparer ma commande.

### US-004

**En tant que** utilisateur

**Je souhaite** modifier mon panier

**Afin de** ajuster ma commande.

---

## EPIC 3 – Gestion des commandes

### US-005

**En tant que** utilisateur

**Je souhaite** payer ma commande

**Afin de** finaliser mon achat.

### US-006

**En tant que** utilisateur

**Je souhaite** choisir un mode de retrait

**Afin de** récupérer ma commande.

### US-007

**En tant que** utilisateur

**Je souhaite** suivre ma commande

**Afin de** connaître son statut.

---

## EPIC 4 – Gestion des casiers

### US-008

**En tant que** client

**Je souhaite** recevoir un code de retrait

**Afin d'ouvrir mon casier.

### US-009

**En tant que** système

**Je souhaite** attribuer automatiquement un casier libre

**Afin de** stocker la commande.

---

## EPIC 5 – Administration

### US-010

**En tant que** administrateur

**Je souhaite** gérer les produits

**Afin de** maintenir le catalogue.

### US-011

**En tant que** administrateur

**Je souhaite** gérer les commandes

**Afin de** superviser les ventes.

### US-012

**En tant que** administrateur

**Je souhaite** consulter les statistiques

**Afin de** piloter l'activité.

---

# 6. Critères d'acceptation Gherkin

## US-003 - Ajouter un produit au panier

```gherkin
Feature: Gestion du panier

Scenario: Ajout d'un article
    Given je consulte une fiche produit
    When je clique sur "Ajouter au panier"
    Then le produit apparaît dans mon panier
    And le total est recalculé
```

## US-005 - Paiement

```gherkin
Feature: Validation de commande

Scenario: Paiement accepté
    Given mon panier contient des produits
    And je suis sur la page de paiement
    When le paiement est accepté
    Then une commande est créée
    And un numéro de commande est généré
```

## US-006 - Choisir un retrait en casier

```gherkin
Feature: Choix du mode de retrait

Scenario: Retrait en casier
    Given des casiers sont disponibles
    When je sélectionne "Casier automatique"
    Then un casier libre est attribué
```

## US-008 - Réception du code de retrait

```gherkin
Feature: Retrait de commande

Scenario: Génération du code
    Given une commande est préparée
    When elle est placée dans un casier
    Then un QR Code est généré
    And le client reçoit une notification
```

## US-009 - Attribution automatique du casier

```gherkin
Feature: Gestion des casiers

Scenario: Attribution automatique
    Given plusieurs casiers sont disponibles
    When une commande est validée
    Then le système sélectionne un casier libre
    And son statut devient "Occupé"
```

---

# 7. Exigences fonctionnelles

| ID | Exigence | Priorité |
|------|------|------|
| REQ-F-001 | Consultation du catalogue | Haute |
| REQ-F-002 | Recherche produit | Haute |
| REQ-F-003 | Gestion panier | Haute |
| REQ-F-004 | Paiement en ligne | Critique |
| REQ-F-005 | Gestion commande | Haute |
| REQ-F-006 | Attribution casier | Critique |
| REQ-F-007 | Génération QR Code | Haute |
| REQ-F-008 | Suivi commande | Moyenne |
| REQ-F-009 | Gestion stock | Haute |
| REQ-F-010 | Administration catalogue | Haute |

---

# 8. Exigences non fonctionnelles

## Performance

| ID | Exigence |
|------|------|
| NFR-001 | Temps de réponse inférieur à 2 secondes |
| NFR-002 | Disponibilité 24/7 |
| NFR-003 | Architecture évolutive |

## Sécurité

| ID | Exigence |
|------|------|
| NFR-004 | HTTPS obligatoire |
| NFR-005 | Conformité RGPD |
| NFR-006 | Conformité PCI-DSS |
| NFR-007 | Journalisation des actions |

## Accessibilité

| ID | Exigence |
|------|------|
| NFR-008 | WCAG 2.1 AA |
| NFR-009 | Navigation clavier |
| NFR-010 | Contrastes conformes |

---

# 9. Modèle de données conceptuel

## Produit

- id
- nom
- description
- prix
- stock
- image

## Utilisateur

- id
- nom
- prénom
- email
- motDePasse

## Commande

- id
- dateCommande
- statut
- montant

## LigneCommande

- quantité
- prixUnitaire

## Casier

- id
- numéro
- état
- codeRetrait

## Paiement

- id
- montant
- datePaiement
- statut

---

# 10. Backlog Produit Initial

## Priorité P1

- Catalogue
- Recherche
- Panier
- Paiement
- Gestion commandes
- Gestion casiers

## Priorité P2

- Historique commandes
- Statistiques
- Gestion utilisateurs

## Priorité P3

- Notifications
- Chatbot
- Fidélité

---

# 11. Livrables attendus

## Analyse

- Cahier des charges
- User Stories
- Diagrammes UML
- MCD / MLD

## Développement

- Front-office
- Back-office
- API casiers

## Documentation

- Documentation technique
- Documentation utilisateur

## Qualité

- Tests unitaires
- Tests fonctionnels
- Tests sécurité

## Déploiement

- Mise en production
- Formation des utilisateurs

---

# 12. Planning prévisionnel

| Phase | Durée |
|---------|---------|
| Analyse | 2 à 4 semaines |
| Développement | 6 à 10 semaines |
| Intégration API casiers | 2 à 4 semaines |
| Tests | 2 semaines |
| Déploiement | 1 semaine |

**Durée totale estimée : 12 à 20 semaines**

---

# 13. Évolutions futures

- Application mobile
- Programme fidélité
- Notifications push
- Livraison en chambre
- Intégration badge personnel
- Extension à d'autres services hospitaliers
- Réservation de produits à l'avance
- Système de recommandations