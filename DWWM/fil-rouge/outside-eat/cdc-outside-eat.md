# Cahier des charges – Site marchand OutsideEat

## Plateforme de commande et de livraison de repas pour le CRM

---

# 1. Présentation générale du projet

## Contexte

Le CRM souhaite offrir aux étudiants, résidents et personnels une plateforme moderne permettant de commander des repas auprès :

- des restaurants partenaires ;
- de la cafétéria du CRM.

Les commandes doivent pouvoir être :

- livrées en chambre ;
- livrées en salle de cours ;
- récupérées en click & collect.

## Objectifs

Le projet **Outside Eat** vise à :

- Proposer un service de restauration flexible et accessible.
- Réduire les files d’attente à la cafétéria.
- Améliorer le confort des résidents.
- Centraliser toutes les offres de restauration dans une seule interface.
- Optimiser la gestion des commandes pour les restaurateurs et le CRM.

---

# 2. Périmètre fonctionnel

## Fonctionnalités pour les utilisateurs

- Création de compte et connexion (email, SSO CRM, numéro étudiant).
- Consultation des menus des restaurants et de la cafétéria.
- Personnalisation des plats (options, suppléments, allergies).
- Choix du mode de livraison :
  - chambre ;
  - salle de cours ;
  - retrait sur place.
- Paiement en ligne :
  - carte bancaire ;
  - portefeuille CRM ;
  - tickets restaurant (si intégration possible).
- Suivi de commande en temps réel.
- Historique des commandes.
- Notifications par email.
- Notifications SMS (optionnel).
- Notifications web.

## Fonctionnalités pour les restaurateurs et la cafétéria

- Interface de gestion des commandes en cours.
- Gestion des menus.
- Gestion des stocks.
- Gestion des disponibilités horaires.
- Création de promotions.
- Gestion des promotions.
- Accès à des statistiques :
  - ventes ;
  - plats populaires ;
  - heures de pointe.

## Fonctionnalités pour les livreurs

- Interface mobile simple permettant de consulter les commandes à livrer.
- Informations de livraison (chambre, salle de cours).
- Confirmation de livraison.

## Fonctionnalités pour l’administrateur CRM

- Gestion des utilisateurs.
- Gestion des restaurateurs.
- Gestion des livreurs.
- Paramétrage des horaires.
- Paramétrage des zones de livraison.
- Paramétrage des tarifs.
- Accès à un tableau de bord global.

---

# 3. Spécifications techniques

## Architecture

- Application web responsive (mobile-first).
- API REST pour la communication front/back.
- Base de données centralisée.

## Technologies recommandées

### Front-end

- React
- Vue.js
- Angular

### Back-end

- Node.js
- Django
- Laravel

### Base de données

- PostgreSQL
- MySQL

### Hébergement

- Azure
- AWS
- OVH

### Sécurité

- HTTPS
- Chiffrement des données sensibles
- Conformité RGPD

---

# 4. Contraintes et exigences

## Contraintes fonctionnelles

- Livraison limitée aux bâtiments autorisés du CRM.
- Gestion des créneaux horaires pour éviter les surcharges.
- Système de contrôle des stocks pour éviter les surcommandes.

## Contraintes techniques

- Temps de réponse inférieur à deux secondes.
- Disponibilité du service d’au moins 99 %.
- Compatibilité avec :
  - mobile ;
  - tablette ;
  - ordinateur.

## Contraintes légales

- Respect du RGPD.
- Conservation des données de transaction.
- Présence de CGU.
- Présence des mentions légales.

---

# 5. Design & UX

## Principes directeurs

- Interface simple, intuitive et accessible.
- Navigation fluide permettant de commander en quelques clics.
- Respect de la charte graphique du CRM et des restaurants partenaires.

## Éléments clés

- Page d’accueil mettant en avant les menus du jour.
- Fiches plats détaillées.
- Panier visible en permanence.
- Suivi de commande en temps réel.

---

# 6. Planning prévisionnel

Le projet se déroule en plusieurs phases :

| Phase | Durée estimée |
|---------|---------|
| Analyse & conception | 3 semaines |
| Développement | 6 à 10 semaines |
| Tests & corrections | 2 à 3 semaines |
| Déploiement | 1 semaine |
| Formation | 1 semaine |

---

# 7. Budget estimatif

| Poste | Estimation |
|---------|---------|
| Développement | 15 000 € à 40 000 € |
| Hébergement annuel | 500 € à 2 000 € |
| Maintenance annuelle | 10 % à 20 % du coût initial |

---

# 8. Livrables

- Maquettes UX/UI.
- Code source complet.
- Documentation technique.
- Documentation utilisateur.
- Tableau de bord administrateur.
- Version finale déployée et fonctionnelle.