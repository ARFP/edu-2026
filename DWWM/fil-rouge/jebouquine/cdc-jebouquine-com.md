# Cahier des Charges Fonctionnel
## Projet Fil Rouge — Site e-commerce de vente de livres « jeBouquine »

**Version : 1.1**
**Date : 2026**
**Type de projet : Application web e-commerce**
**Méthodologie : Agile / Scrum**
**Public cible : Formation DWWM / CDA**

---

# 1. Présentation du projet

## 1.1 Contexte

La société fictive **jeBouquine** souhaite développer une plateforme de vente en ligne spécialisée dans les ouvrages francophones et anglophones.

Le site doit permettre aux internautes de :

- Rechercher des livres.
- Consulter des fiches détaillées.
- Ajouter des livres à un panier.
- Commander en ligne.
- Suivre leurs commandes.
- Gérer leur compte client.

L'objectif est de proposer une expérience utilisateur simple, fluide et sécurisée.

---

## 1.2 Parties prenantes

| Partie prenante | Rôle |
|----------------|-------|
| Direction jeBouquine | Commanditaire |
| Clients | Utilisateurs finaux |
| Administrateurs | Gestion du catalogue |
| Service logistique | Préparation des commandes |
| Équipe de développement | Réalisation du projet |

---

# 2. Objectifs métier

## 2.1 Objectifs fonctionnels

Le système doit permettre :

- La consultation du catalogue.
- La recherche avancée d'ouvrages.
- La gestion d'un panier.
- La création de compte client.
- La passation de commandes.
- Le paiement sécurisé.
- Le suivi des commandes.

## 2.2 Objectifs stratégiques

- Développer la présence numérique de l'entreprise.
- Augmenter les ventes de livres.
- Fidéliser la clientèle.
- Permettre l'ajout futur de nouvelles fonctionnalités.

---

# 3. Périmètre du projet

## Inclus

- ✅ Catalogue de livres
- ✅ Recherche avancée
- ✅ Gestion des comptes clients
- ✅ Gestion des commandes
- ✅ Paiement en ligne
- ✅ Espace client
- ✅ Administration du catalogue

---

## Hors périmètre (Version 1)

- ❌ Application mobile native
- ❌ Programme de fidélité
- ❌ Vente de livres numériques
- ❌ Marketplace vendeurs tiers
- ❌ Gestion des retours automatisée

---

# 4. Personas

## Persona 1 : Sophie Martin

- **Âge :** 37 ans
- **Profession :** Enseignante

### Besoins

- Trouver rapidement un livre.
- Pouvoir comparer plusieurs ouvrages.
- Commander facilement.

### Frustrations

- Recherche inefficace.
- Processus de commande complexe.

---

## Persona 2 : Thomas Weber

- **Âge :** 24 ans
- **Profession :** Étudiant

### Besoins

- Consulter les avis.
- Sauvegarder une sélection.
- Commander depuis un smartphone.

---

# 5. User Stories

## Gestion du catalogue

### US-001

- **En tant que** visiteur
- **Je souhaite** rechercher un livre
- **Afin de** trouver rapidement un ouvrage.

### Critères d'acceptation

- Recherche par titre.
- Recherche par auteur.
- Recherche par ISBN.
- Recherche par mot-clé.

---

### US-002

- **En tant que** visiteur
- **Je souhaite** filtrer les résultats
- **Afin de** faciliter ma recherche.

### Critères d'acceptation

- Filtre par catégorie.
- Filtre par prix.
- Filtre par disponibilité.

---

## Gestion du panier

### US-003

- **En tant que** client
- **Je souhaite** ajouter un ouvrage au panier
- **Afin de** préparer ma commande.

### Critères d'acceptation

- Ajout depuis la fiche produit.
- Mise à jour du nombre d'articles.
- Calcul automatique du total.

---

### US-004

- **En tant que** client
- **Je souhaite** modifier les quantités
- **Afin de** corriger mon panier.

---

## Gestion des comptes

### US-005

- **En tant que** visiteur
- **Je souhaite** créer un compte
- **Afin de** passer commande.

---

### US-006

- **En tant que** client
- **Je souhaite** modifier mes coordonnées
- **Afin de** maintenir mes informations à jour.

---

## Gestion des commandes

### US-007

- **En tant que** client
- **Je souhaite** valider une commande
- **Afin d'acheter mes livres.**

---

### US-008

- **En tant que** client
- **Je souhaite** suivre ma commande
- **Afin de connaître son état d'avancement.**

---

# 6. Exigences fonctionnelles

| ID | Exigence | Priorité |
|----|-----------|----------|
| REQ-F-001 | Recherche simple | Haute |
| REQ-F-002 | Recherche multicritère | Haute |
| REQ-F-003 | Consultation catalogue | Haute |
| REQ-F-004 | Gestion panier | Haute |
| REQ-F-005 | Création compte | Haute |
| REQ-F-006 | Authentification | Haute |
| REQ-F-007 | Paiement sécurisé | Critique |
| REQ-F-008 | Historique commandes | Moyenne |
| REQ-F-009 | Gestion adresses | Moyenne |
| REQ-F-010 | Administration catalogue | Haute |

---

# 7. Exigences non fonctionnelles

## Performance

| ID | Exigence |
|----|-----------|
| NFR-001 | Temps de réponse inférieur à 2 secondes |
| NFR-002 | 1000 connexions simultanées |
| NFR-003 | Catalogue supérieur à 1 million d'ouvrages |

---

## Sécurité

| ID | Exigence |
|----|-----------|
| NFR-004 | Chiffrement HTTPS |
| NFR-005 | Protection RGPD |
| NFR-006 | Hachage des mots de passe |
| NFR-007 | Gestion des rôles |

---

## Accessibilité

| ID | Exigence |
|----|-----------|
| NFR-008 | Respect WCAG 2.1 niveau AA |
| NFR-009 | Navigation clavier |
| NFR-010 | Contrastes conformes |

---

# 8. Modèle de données (conceptuel)

## Entités principales

### Livre

- id
- isbn
- titre
- résumé
- prix
- stock
- image
- datePublication

### Auteur

- id
- nom
- prénom

### Catégorie

- id
- libellé

### Utilisateur

- id
- nom
- prénom
- email
- motDePasse

### Adresse

- id
- rue
- codePostal
- ville
- pays

### Commande

- id
- dateCommande
- montantTotal
- statut

### LigneCommande

- quantité
- prixUnitaire

---

# 9. Backlog produit initial

| Priorité | Fonctionnalité |
|-----------|---------------|
| P1 | Authentification |
| P1 | Catalogue |
| P1 | Recherche |
| P1 | Fiche produit |
| P1 | Panier |
| P1 | Commande |
| P1 | Paiement |
| P2 | Historique commandes |
| P2 | Gestion adresses |
| P2 | Commentaires |
| P3 | Recommandations |

---

# 10. Matrice de traçabilité

| Exigence | User Story | Cas d'utilisation |
|-----------|-------------|-------------------|
| REQ-F-001 | US-001 | Rechercher un livre |
| REQ-F-002 | US-002 | Filtrer les résultats |
| REQ-F-004 | US-003 | Gérer le panier |
| REQ-F-005 | US-005 | Créer un compte |
| REQ-F-007 | US-007 | Valider une commande |
| REQ-F-008 | US-008 | Consulter ses commandes |

---

# 11. Critères de réussite

Le projet sera considéré comme réussi si :

- Toutes les exigences critiques sont implémentées.
- Les tests fonctionnels sont validés.
- Le temps de réponse respecte les objectifs.
- Le paiement est sécurisé.
- Les données personnelles sont protégées.
- Le site est responsive.
- Le parcours d'achat est réalisable sans assistance.

---

# 12. Livrables attendus

## Analyse

- Cahier des charges
- User Stories
- Diagrammes UML
- MCD / MLD

## Développement

- Dépôt Git
- Documentation technique
- Documentation utilisateur

## Livraison

- Application déployée
- Base de données
- Guide d'installation

---

# 13. Évolutions futures

- Système de notation avancé
- Programme fidélité
- Recommandation basée sur l'IA
- Vente de livres numériques
- Application mobile
- Système de wishlist