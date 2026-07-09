# Cahier des charges – Site marchand MonPetitKiosque

## 1. Présentation du projet

**MonPetitKiosque** est une application web destinée aux patients, visiteurs et personnels hospitaliers.

Elle permet d’acheter des **articles non périssables** du kiosque de l’hôpital et de les retirer soit :

- au kiosque pendant les heures d’ouverture ;
- dans des **casiers automatiques** accessibles 24/7.

L’objectif est d’améliorer l’accès aux produits, fluidifier le service et offrir une solution autonome en dehors des horaires du personnel.

---

## 2. Objectifs fonctionnels

- Proposer un catalogue digital d’articles non périssables.
- Permettre l’achat en ligne via un parcours simple et sécurisé.
- Offrir un retrait autonome via casiers automatiques.
- Gérer les stocks en temps réel (kiosque + casiers).
- Fournir un back-office complet pour le personnel.
- Assurer une expérience fluide et accessible pour tous les utilisateurs.

---

## 3. Périmètre des produits

L’application MonPetitKiosque propose uniquement des **articles non périssables**, tels que :

- magazines ;
- journaux ;
- livres ;
- mots croisés ;
- sudoku ;
- produits d’hygiène (savon, gel, mouchoirs…) ;
- accessoires (chargeurs, écouteurs, stylos, carnets…) ;
- snacks et boissons **emballés longue conservation** (optionnel selon politique interne).

Aucun produit frais, réfrigéré ou à date courte n’est proposé.

---

## 4. Fonctionnalités détaillées

### 4.1 Front-office (utilisateurs)

- Page d’accueil MonPetitKiosque.
- Catalogue avec catégories, filtres et recherche.
- Fiches produits (photo, description, prix, disponibilité).
- Panier et gestion des quantités.
- Paiement sécurisé (CB, Apple Pay, Google Pay).
- Choix du mode de retrait :
  - kiosque (si ouvert) ;
  - casier automatique.
- Sélection d’un casier libre.
- Confirmation de commande.
- Envoi automatique du **code de retrait** (QR code ou PIN).
- Suivi de commande.
- Espace personnel (historique, factures, données).

### 4.2 Back-office (administration)

- Gestion du catalogue (ajout, modification, suppression).
- Gestion des stocks (kiosque + casiers).
- Gestion des commandes et états.
- Gestion des casiers :
  - disponibilité ;
  - ouverture manuelle ;
  - signalement de panne.
- Statistiques :
  - ventes ;
  - produits les plus consultés ;
  - taux d’occupation des casiers.
- Gestion des utilisateurs internes (rôles, permissions).
- Paramétrages généraux (horaires, messages automatiques, TVA…).

### 4.3 Gestion des casiers automatiques

- Communication via API fournie par le fabricant.
- Attribution automatique d’un casier libre.
- Envoi du code de retrait au client.
- Détection de l’ouverture du casier.
- Mise à jour automatique de l’état du casier.
- Historique des ouvertures et incidents.

---

## 5. Contraintes techniques

### 5.1 Architecture

- Application web responsive (mobile-first).
- Framework recommandé : Symfony, Laravel, Node.js ou équivalent.
- Base de données SQL (MySQL, PostgreSQL).
- API REST pour communication casiers.
- Hébergement sécurisé (HTTPS).

### 5.2 Sécurité

- Conformité RGPD.
- Paiement sécurisé (norme PCI-DSS).
- Chiffrement des données sensibles.
- Gestion stricte des rôles et permissions.
- Journalisation des actions critiques.

---

## 6. Design & ergonomie

- Identité visuelle centrée sur **MonPetitKiosque**.
- Interface simple, rassurante et accessible.
- Respect des normes WCAG 2.1 AA.
- Couleurs douces adaptées à l’environnement hospitalier.
- Parcours utilisateur optimisé pour rapidité et clarté.

---

## 7. Contenus

- Textes descriptifs des produits.
- Photos HD.
- Mentions légales.
- Conditions Générales de Vente (CGV).
- Politique de confidentialité.
- FAQ.
- Support client (formulaire ou chatbot).

---

## 8. Livrables attendus

- Application MonPetitKiosque (front-office + back-office).
- API casiers.
- Documentation technique.
- Documentation utilisateur.
- Formation du personnel.
- Jeux de tests :
  - unitaires ;
  - fonctionnels ;
  - sécurité.
- Mise en production.

---

## 9. Planning prévisionnel

| Étape | Durée estimée |
|---------|---------|
| Analyse & conception | 2 à 4 semaines |
| Développement | 6 à 10 semaines |
| Intégration casiers | 2 à 4 semaines |
| Tests & validation | 2 semaines |
| Mise en ligne | 1 semaine |

**Durée totale estimée : 12 à 20 semaines**

---

## 10. Budget estimatif

Selon la complexité du projet, l’intégration des casiers et le niveau de personnalisation du design :

**Entre 12 000 € et 50 000 €**

---

## 11. Évolutions possibles

- Application mobile MonPetitKiosque.
- Programme de fidélité.
- Notifications push.
- Livraison en chambre.
- Intégration avec badges du personnel.
- Extension à d’autres services de l’hôpital.