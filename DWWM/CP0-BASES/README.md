# Plan de Module : Les Fondations du Développeur Web

**Public cible :** Apprenants en reconversion professionnelle (Adapté aux profils TSA / TDAH)  
**Cadre réglementaire :** Titre Professionnel DWWM (Niveau 5) — Alignement REAC / RE

---

## Principes Directeurs d'Accessibilité
Pour maximiser la charge cognitive utile et minimiser la surcharge attentionnelle ou l'anxiété, ce module applique les règles suivantes :
* **Zéro ambiguïté :** Pas de métaphores, pas de consignes implicites. Chaque tâche commence par un verbe d'action univoque.
* **Prévisibilité structurelle :** Chaque sous-section utilise exactement la même structure visuelle : 
    - *Durée ➡️ Objectif ➡️ Livrable attendu ➡️ Liste d'actions séquentielles*.
* **Découpage atomique :** Les concepts complexes sont segmentés en micro-étapes indépendantes de maximum 15 à 20 minutes.

---

## Structuration Pédagogique selon la Taxonomie de Bloom

### 1. Mémoriser (Restituer des faits et concepts de base)
* **Objectif général :** Identifier les composants fondamentaux du Web et l'environnement d'un développeur sans manipulation technique majeure.

#### 📦 Sous-module 1.1 : L'Architecture Client-Serveur
* **Durée :** 1 heure
* **Objectif opérationnel :** Citer les 3 composants d'une architecture Web (Client, Serveur, Base de données) et décrire leur rôle unique.
* **Livrable attendu :** Un schéma relationnel textuel complété avec 100% d'exactitude.
* **Séquence d'actions pas-à-pas :**
    1.  Lire la fiche terminologique standardisée (définitions strictes de *Client*, *Serveur*, *Requête*, *Réponse*).
    2.  Regarder l'animation visuelle épurée (sans distraction sonore ni textuelle superflue) matérialisant le trajet d'une requête HTTP.
    3.  Remplir le texte à trous fourni pour fixer la terminologie exacte.
    4.  Associer, sous forme de carte à relier, chaque définition technique à son mot-clé.

#### 📦 Sous-module 1.2 : Le Vocabulaire du Développeur
* **Durée :** 1 heure
* **Objectif opérationnel :** Distinguer les rôles respectifs des langages HTML, CSS et JavaScript dans une page web.
* **Livrable attendu :** Un tableau comparatif trié sans erreur.
* **Séquence d'actions pas-à-pas :**
    1.  Ouvrir le document de référence présentant le triptyque du Web (HTML = Squelette, CSS = Habillage, JS = Comportement).
    2.  Classer 15 lignes de code d'exemple dans trois colonnes distinctes (HTML, CSS ou JS) en s'aidant des indices visuels (balises `<>`, accolades `{}`, fonctions `()`).

---

### 2. Comprendre (Expliquer des idées ou des concepts)
* **Objectif général :** Expliquer la logique sous-jacente des outils de développement et des protocoles sans écrire de code fonctionnel complexe.

#### 📦 Sous-module 2.1 : Le Protocole HTTP et le cycle Requête-Réponse
* **Durée :** 1 heure 30 minutes
* **Objectif opérationnel :** Expliquer le mécanisme d'une requête HTTP en décrivant le rôle des codes de statut principaux (200, 404, 500).
* **Livrable attendu :** Une retranscription logique d'un scénario de navigation (Exemple : "L'utilisateur clique sur un lien brisé").
* **Séquence d'actions pas-à-pas :**
    1.  Analyser l'arborescence visuelle des codes de statut HTTP (Familles 2xx, 4xx, 5xx) classés par codes couleur (Vert = Succès, Orange = Erreur Client, Rouge = Erreur Serveur).
    2.  Sélectionner le code de statut approprié pour 5 situations réelles décrites de manière factuelle.
    3.  Rédiger une phrase explicative simple pour chaque situation en suivant le modèle strict : *"Le serveur renvoie le code X parce que [cause concrète]"*.

#### 📦 Sous-module 2.2 : Le Rôle du Versionnage (Git)
* **Durée :** 1 heure 30 minutes
* **Objectif opérationnel :** Expliquer l'utilité d'un système de contrôle de version et la chronologie des trois états Git (Working Directory, Staging Area, Local Repository).
* **Livrable attendu :** Une frise chronologique légendée par l'apprenant.
* **Séquence d'actions pas-à-pas :**
    1.  Suivre la démonstration pas-à-pas du formateur conceptualisant Git comme un appareil photo (Modifications ➡️ Choix des éléments à photographier ➡️ Prise de vue finale).
    2.  Placer les commandes `git add` et `git commit` sur un axe linéaire fléché représentant la progression d'un fichier.
    3.  Formuler par écrit la différence entre un fichier "suivi" (tracked) et "non suivi" (untracked).

---

### 3. Appliquer (Utiliser des informations dans des situations concrètes)
* **Objectif général :** Exécuter des procédures techniques standardisées et installer son environnement de travail sans déviation algorithmique.

#### 📦 Sous-module 3.1 : Initialisation de l'Environnement Local (WSL & Git)
* **Durée :** 3 heures
* **Objectif opérationnel :** Configurer un dépôt Git local et exécuter les commandes de base pour sauvegarder un fichier.
* **Livrable attendu :** Un dépôt Git initialisé contenant un fichier d'historique validé.
* **Séquence d'actions pas-à-pas :**
    1.  Ouvrir le terminal Linux (WSL / Debian).
    2.  Saisir la commande `git init` dans le dossier spécifié.
    3.  Créer un fichier texte nommé `index.html` à l'aide de la commande `touch index.html`.
    4.  Saisir la commande `git status` et identifier visuellement la couleur rouge indiquant le fichier non suivi.
    5.  Exécuter `git add index.html`, puis vérifier le passage au vert avec `git status`.
    6.  Exécuter la commande de validation finale : `git commit -m "Initialisation du projet"`.

#### 📦 Sous-module 3.2 : Structure d'un Document HTML Propre
* **Durée :** 2 heures
* **Objectif opérationnel :** Écrire un document HTML5 valide respectant la sémantique de base et l'imbrication des balises.
* **Livrable attendu :** Un fichier `index.html` structurellement parfait, validé par le validateur W3C.
* **Séquence d'actions pas-à-pas :**
    1.  Recopier le squelette standard HTML5 fourni (Doctype, html, head, body).
    2.  Insérer de manière hiérarchique un titre principal `<h1>`, deux sous-titres `<h2>` et trois paragraphes `<p>`.
    3.  Vérifier l'alignement et l'indentation du code à l'aide de l'extension de formatage automatique de l'éditeur (raccourci clavier explicite fourni).
    4.  Soumettre le code au validateur en ligne pour obtenir la mention "Zero Errors".

---

### 4. Analyser (Décomposer les informations en parties pour en comprendre les liens)
* **Objectif général :** Inspecter une structure existante, identifier les anomalies logiques et décortiquer les flux d'exécution.

#### 📦 Sous-module 4.1 : Inspection du DOM et Débogage Visuel
* **Durée :** 2 heures 30 minutes
* **Objectif opérationnel :** Identifier les erreurs de balisage ou de liaison CSS dans une page cassée en utilisant les outils de développement du navigateur.
* **Livrable attendu :** Une liste écrite répertoriant les 3 anomalies structurelles d'une page témoin.
* **Séquence d'actions pas-à-pas :**
    1.  Ouvrir la page web d'exercice fournie volontairement dégradée.
    2.  Faire un clic droit ➡️ *Inspecter* pour ouvrir les DevTools.
    3.  Parcourir l'onglet *Elements* pour localiser une balise non fermée qui brise la mise en page.
    4.  Consulter l'onglet *Console* pour repérer une erreur 404 indiquant un mauvais chemin d'accès vers un fichier CSS.
    5.  Noter les corrections nécessaires sur la feuille de route sans modifier le code source dans un premier temps.

#### 📦 Sous-module 4.2 : Analyse d'un Algorithme Linéaire
* **Durée :** 2 heures
* **Objectif opérationnel :** Décomposer un script séquentiel simple (variables et conditions) pour déterminer la valeur finale d'une variable.
* **Livrable attendu :** Un tableau de suivi des variables complété étape par étape (Trace d'exécution).
* **Séquence d'actions pas-à-pas :**
    1.  Prendre connaissance d'un bloc de code de 10 lignes contenant des affectations de variables numériques.
    2.  Pour chaque ligne de code, reporter la valeur de chaque variable dans le tableau fourni.
    3.  Identifier la ligne exacte où une variable change d'état ou subit une modification inattendue.

---

### 5. Évaluer (Formuler des jugements fondés sur des critères et des normes)
* **Objectif général :** Mesurer la conformité d'une production par rapport à des standards professionnels (Normes W3C, bonnes pratiques, critères d'accessibilité RGAA).

#### 📦 Sous-module 5.1 : Revue de Conformité Standard (Qualité Web)
* **Durée :** 3 heures
* **Objectif opérationnel :** Juger de la qualité d'une page web d'un pair au regard des critères de sémantique et d'accessibilité de base (présence des attributs `alt` sur les images, hiérarchie des titres).
* **Livrable attendu :** Une grille d'évaluation binaire (Conforme / Non conforme) argumentée.
* **Séquence d'actions pas-à-pas :**
    1.  Ouvrir la grille d'évaluation fournie (contenant 10 critères explicites et mesurables).
    2.  Analyser le code source du projet d'un autre apprenant de manière anonyme.
    3.  Cocher "Oui" ou "Non" pour chaque critère de manière objective.
    4.  Pour chaque case "Non", indiquer la ligne de code concernée et la règle violée (Exemple : *"Ligne 12 : L'image n'a pas d'attribut alt"*).

---

### 6. Créer (Regrouper des éléments pour former un tout fonctionnel)
* **Objectif général :** Assembler l'ensemble des connaissances acquises pour réaliser une première intégration statique autonome et documentée.

#### 📦 Sous-module 6.1 : Le Mini-Projet "Ma Première Page Pro"
* **Durée :** 6 heures (Segmenté en sessions de 2 heures avec pauses obligatoires)
* **Objectif opérationnel :** Assembler une page de profil professionnel statique en HTML5, versionnée avec Git, intégrant une structure sémantique irréprochable.
* **Livrables attendus :** 1. Un fichier `index.html` complet et valide.
    2. Un dépôt Git local contenant un historique de commits clair (minimum 4 commits thématiques).
* **Séquence d'actions pas-à-pas :**
    1.  **Étape 1 (Structure) :** Écrire l'architecture HTML globale (En-tête `header`, zone de contenu `main`, pied de page `footer`).
    2.  **Étape 2 (Contenu sémantique) :** Intégrer une section de présentation avec un titre, un paragraphe textuel et une liste à puces énumérant des compétences techniques.
    3.  **Étape 3 (Mise en conformité) :** Inclure une image de profil avec son attribut `alt` descriptif obligatoire.
    4.  **Étape 4 (Versionnage) :** Effectuer un commit Git intermédiaire avec un message explicite : `"Feat: Ajout de la structure et du contenu de base"`.
    5.  **Étape 5 (Validation) :** Passer le code au validateur W3C et corriger les éventuelles alertes.
    6.  **Étape 6 (Livraison) :** Effectuer le commit de clôture : `"Docs: Finalisation et validation de la page"`.
