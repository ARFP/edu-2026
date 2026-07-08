# Cahier des charges – Site marchand `jeBouquine`

## 1. Présentation générale du projet

La société fictive **jeBouquine** souhaite développer un site web marchand destiné à la vente en ligne d’ouvrages francophones et anglophones.

Le site doit permettre aux internautes de rechercher, consulter, sélectionner et commander des livres de manière simple, rapide et sécurisée.

Le projet s’inscrit dans une démarche inspirée des pratiques du Processus Unifié (UP), notamment dans sa phase d’initialisation.

---

## 2. Objectifs du projet

### 2.1 Objectifs fonctionnels

Le site doit permettre à l’utilisateur de :

- Rechercher des ouvrages selon différents critères.
- Consulter des fiches détaillées pour chaque livre.
- Constituer un panier virtuel.
- Passer commande et régler en ligne.
- Gérer son compte client.
- Suivre l’état de ses commandes.

### 2.2 Objectifs stratégiques

- Se positionner sur le marché de la librairie en ligne face aux acteurs généralistes et spécialisés.
- Proposer des fonctionnalités évolutives permettant d’ajouter rapidement de nouveaux services.
- Devenir, à moyen terme, un acteur majeur de la vente de livres en ligne en France.

---

## 3. Exigences fonctionnelles

### 3.1 Recherche

Le site doit offrir plusieurs modes de recherche afin de permettre à l’internaute de trouver rapidement un ouvrage :

- Recherche par titre, auteur, ISBN ou mot-clé.
- Recherche multicritères.
- Accès direct à des catégories thématiques.
- Consultation des nouveautés, meilleures ventes ou sélections éditoriales.
- Résultats triables et facilement parcourables.

### 3.2 Découverte des ouvrages

Chaque livre doit disposer d’une page dédiée contenant :

- Une image de couverture (agrandissable).
- Le prix et la disponibilité.
- Des commentaires de lecteurs.
- La table des matières.
- D’éventuels extraits ou chapitres.

### 3.3 Sélection et panier

L’utilisateur doit pouvoir :

- Ajouter un ouvrage à un panier virtuel.
- Modifier les quantités.
- Supprimer des articles.
- Consulter le panier à tout moment.

Le panier n’est pas sauvegardé en base de données : il n’existe que le temps de la session.

### 3.4 Commande

Le site doit permettre :

- L’accès permanent au formulaire de commande.
- La saisie des coordonnées personnelles et de livraison.
- Le paiement sécurisé en ligne.
- L’impression d’un devis pour commande par courrier ou fax.
- Le suivi des commandes en cours.
- La modification d’une commande tant qu’elle n’est pas expédiée.

### 3.5 Gestion du compte client

Le client doit pouvoir :

- Modifier ses coordonnées.
- Gérer ses préférences.
- Ajouter plusieurs adresses.
- Consulter l’historique complet de ses commandes.

---

## 4. Exigences non fonctionnelles

### 4.1 Ergonomie

- Interface claire, intuitive et sobre.
- Navigation simple, sans surcharge visuelle.
- Processus d’achat fluide et rapide.

### 4.2 Formulaire de commande

- Présentation simplifiée.
- Saisie guidée pour éviter les erreurs.
- Limitation du nombre d’étapes.

### 4.3 Aide en ligne

- Aide contextuelle disponible à tout moment.
- Moteur de recherche interne dédié à l’aide.
- Visite guidée pour les nouveaux utilisateurs.

### 4.4 Performances

- Gestion de plus de **10 000 comptes clients**.
- Support de **1 000 connexions simultanées**.
- Catalogue pouvant dépasser **1 000 000 de titres**.
- Temps de réponse maximal pour une recherche : **2 secondes**.

---

## 5. Contraintes techniques

### 5.1 Mise à jour des données

Les données proviennent de deux sources externes :

- Une source pour l’ajout des nouveaux ouvrages.
- Une source pour la mise à jour des prix et des stocks.

Ces données doivent être intégrées automatiquement et régulièrement.

Une application intranet permettra d’enrichir manuellement les informations complémentaires.

### 5.2 Base de données

- Utilisation d’un SGBDR robuste, recommandé : **Oracle**.
- Capacité à gérer un volume important de transactions.
- Fiabilité et durabilité des données.

### 5.3 Données saisies par les utilisateurs

- Stockage des coordonnées clients.
- Conservation des informations nécessaires à la livraison.
- Protection et confidentialité des données personnelles.

### 5.4 Paiement sécurisé

- Utilisation du protocole **SSL** pour le chiffrement des échanges.
- Stockage temporaire du numéro de carte bancaire jusqu’à validation par la banque.
- Suppression automatique du numéro de carte après validation.

---

## 6. Gestion des exigences

Le projet doit intégrer un processus de gestion des exigences permettant :

- La cohérence entre besoins et livrables.
- L’analyse d’impact en cas de changement.
- La traçabilité entre exigences, cas d’utilisation et éléments du système.

Les outils possibles incluent :

- DOORS
- RequisitePro
- CaliberRM

Les exigences doivent être :

- Identifiées (ID unique).
- Décrites textuellement.
- Classées par priorité, stabilité, difficulté technique.
- Reliées aux cas d’utilisation et aux besoins des parties prenantes.

### Exemples d’exigences fonctionnelles

- **Recherche1** : l’internaute doit pouvoir trouver rapidement un ouvrage dans le catalogue.
- **Recherche2** : la recherche doit accepter un ou plusieurs critères.
- **Panier1** : l’utilisateur peut enregistrer un ouvrage dans un panier virtuel.
- **Commande1** : accès permanent au formulaire de commande.
- **Commande2** : les données doivent être transmises de manière cryptée.

### Exemples de demandes de parties prenantes

- Ergonomie sobre et efficace.
- Aide en ligne puissante.
- Transactions sécurisées.