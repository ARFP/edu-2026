# Série 2 – Mettre en forme le « Compte Utilisateur » avec CSS

## REAC DWWM 2023 – CP3

### Compétences

> Développer des interfaces utilisateur.

### Objectifs de la série

Cette deuxième série est consacrée à la mise en forme des pages HTML réalisées lors de la série précédente.

Vous allez :

- Créer un système de design
- Appliquer une charte graphique cohérente 
- Utiliser les sélecteurs CSS 
- Mettre en page les contenus 
- Créer des interfaces responsives 
- Améliorer l'expérience utilisateur

### Prérequis

- Vous avez terminé la [série précédente](./exos-01-01-utilisateurs-html)
- Toutes les pages HTML sont valides W3C et fonctionnelles
- Navigation déjà en place

### Contraintes

- HTML existant réutilisé
- CSS externe uniquement
- Aucun framework CSS
- Aucun JavaScript
- Responsive obligatoire
- Respect de l'accessibilité

---

# Exercice 1 – Créer la feuille de style principale

## Objectif pédagogique

Mettre en place l'organisation des styles du projet.

## Consignes

A la racine du projet, créer un dossier `css`.

Dans ce dossier `css`, créer un fichier `style.css`

Votre arborescence devrait être : 

```text
/
│
├── index.html (Accueil)
├── profil.html
├── [...]
├── css/
├────── style.css 
```

Lier ce fichier à toutes les pages du projet.

Ajouter :

- Réinitialisation légère des marges ;
- Police globale ;
- Couleurs principales ;
- Styles des titres ;
- Styles des liens.

## Critères de réussite

- Un seul fichier CSS partagé
- Style appliqué sur toutes les pages
- Cohérence visuelle

---

# Exercice 2 – Construire la charte graphique

## Objectif pédagogique

Définir une identité visuelle commune.

## Consignes

A la racine du projet, créer une page `ui-design.html` contenant :

### Couleur principale

Utilisée pour :

- boutons
- liens importants
- éléments interactifs

### Couleur secondaire

Utilisée pour :

- arrière-plans
- encadrés
- éléments décoratifs

### Couleur d'accentuation

Utilisée pour :

- notifications
- messages importants

### Typographie

Définir :

- police des titres ;
- police du contenu ;
- tailles principales.

## Critères de réussite

- Cohérence graphique
- Lisibilité
- Contrastes suffisants

---

# Exercice 3 – Mettre en forme la page d'accueil

## Objectif pédagogique

Créer une landing page simple.

## Consignes

Mettre en forme :

### Header

- logo à gauche ;
- navigation à droite.

### Zone principale

- titre mis en valeur ;
- texte aéré ;
- bouton principal visible.

### Footer

- séparé du contenu principal.

## Critères de réussite

- Mise en page claire
- Bonne hiérarchie visuelle
- Lecture confortable

---

# Exercice 4 – Styliser les formulaires

## Objectif pédagogique

Créer des formulaires professionnels.

## Consignes

Appliquer un style sur :

- labels ;
- champs de saisie ;
- boutons ;
- groupes de champs.

Ajouter :

- espaces cohérents ;
- bordures harmonieuses ;
- états visuels au survol.

## Critères de réussite

- Formulaire lisible
- Alignement cohérent
- Interface professionnelle

---

# Exercice 5 – Styliser la page d'inscription

## Objectif pédagogique

Créer une page agréable à utiliser.

## Consignes

Mettre en forme :

- formulaire centré ;
- largeur contrôlée ;
- titre visible ;
- bouton d'inscription mis en avant.

## Critères de réussite

- Page équilibrée
- Bonne utilisation des espaces
- Responsive

---

# Exercice 6 – Styliser la page de connexion

## Objectif pédagogique

Créer une interface claire et rassurante.

## Consignes

Mettre en évidence :

- le formulaire ;
- le bouton de connexion ;
- les liens secondaires.

Ajouter un effet visuel léger :

- ombre ;
- bordure ;
- encadré.

## Critères de réussite

- Connexion identifiable immédiatement
- Bonne lisibilité
- Interface moderne

---

# Exercice 7 – Mettre en forme la page Profil

## Objectif pédagogique

Valoriser les informations utilisateur.

## Consignes

Présenter les informations sous forme :

- de cartes ;
- ou de sections distinctes.

Mettre en évidence :

- identité ;
- coordonnées ;
- informations spécifiques au projet.

## Critères de réussite

- Lecture facile
- Organisation claire
- Mise en valeur des données

---

# Exercice 8 – Mettre en forme la gestion des adresses

## Objectif pédagogique

Créer une liste structurée.

## Consignes

Chaque adresse doit apparaître dans un bloc visuel.

Ajouter :

- marges ;
- bordures ;
- séparation visuelle.

Mettre en évidence les boutons :

- Modifier ;
- Supprimer.

## Critères de réussite

- Liste facile à parcourir
- Actions visibles
- Mise en forme homogène

---

# Exercice 9 – Construire le tableau de bord

## Objectif pédagogique

Créer une interface de type dashboard.

## Consignes

Créer une mise en page avec :

### Navigation

- colonne latérale ;
- menu vertical.

### Zone principale

- message de bienvenue ;
- blocs d'informations ;
- résumé du compte.

Utiliser :

```css
flex
```

ou

```css
grid
```

## Critères de réussite

- Dashboard moderne
- Navigation visible
- Mise en page structurée

---

# Exercice 10 – Rendre toutes les pages responsives

## Objectif pédagogique

Adapter l'interface aux différentes tailles d'écran.

## Consignes

Ajouter des media queries.

Tester :

- smartphone ;
- tablette ;
- ordinateur.

Adapter :

- navigation ;
- formulaires ;
- tableaux ;
- cartes.

## Critères de réussite

- Aucune barre de défilement horizontale
- Lecture confortable
- Interface exploitable sur mobile

---

# Exercice 11 – Uniformiser les composants

## Objectif pédagogique

Créer une bibliothèque graphique cohérente.

## Consignes

Vérifier que :

### Tous les boutons

- utilisent le même style ;

### Tous les formulaires

- ont la même apparence ;

### Toutes les cartes

- respectent les mêmes règles ;

### Tous les titres

- suivent la même hiérarchie visuelle.

## Critères de réussite

- Cohérence graphique
- Réutilisabilité
- Respect de la charte

---

# Exercice 12 – Audit UX et accessibilité

## Objectif pédagogique

Améliorer l'expérience utilisateur.

## Consignes

Contrôler :

- contraste des couleurs ;
- taille des textes ;
- taille des zones cliquables ;
- visibilité du focus clavier ;
- cohérence de navigation.

## Critères de réussite

- Utilisation confortable
- Accessibilité améliorée
- Respect des bonnes pratiques

---

# TP de Synthèse

## TP 2 – Réaliser l'habillage graphique complet du module « Compte Utilisateur »

### Contexte

Vous disposez désormais de toutes les pages HTML du module compte utilisateur.

Votre mission consiste à transformer ces pages brutes en une interface professionnelle respectant une identité graphique cohérente.

### Travail demandé

Mettre en forme :

```text
Accueil
Inscription
Connexion
Mot de passe oublié
Tableau de bord
Profil
Modification du profil
Changement du mot de passe
Gestion des adresses
```

### Contraintes techniques

- CSS externe uniquement
- Responsive obligatoire
- Aucun framework CSS
- Aucun JavaScript

### Livrables attendus

```text
/
│
├── css/
│   └── style.css
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

### Critères d'évaluation

| Critère | Points |
|----------|---------:|
| Charte graphique | 20 |
| Mise en page | 20 |
| Responsive | 20 |
| Accessibilité | 20 |
| Cohérence visuelle | 20 |

**Total : 100 points**

## Durée estimée

**12 à 15 heures**

## Résultat attendu

À la fin de cette série, les apprenants disposent :

- d'un module compte utilisateur complet ;
- d'une interface responsive ;
- d'une charte graphique cohérente ;
- d'une base prête à recevoir les comportements JavaScript de la Série 3.