---
marp: true
theme: default
paginate: true
backgroundColor: #F3F0DF
header: 'Titre Pro DWWM - CP1 : Installer son Environnement'
footer: 'Module 1 - Configuration Technique'
style: |
  section {
    font-family: 'Open Sans', sans-serif;
    color: #334155;
  }
  h1, h2 {
    color: #005088;
  }
  .blue-section {
    background-color: #005088;
    color: #F3F0DF;
  }
  .blue-section h2 {
    color: #11CAA0;
  }
  blockquote {
    background: #fff;
    border-left: 10px solid #11CAA0;
    font-style: italic;
  }
  code {
    background: #e2e8f0;
    color: #ef4444;
  }
  .step-box {
    border: 2px solid #005088;
    border-radius: 8px;
    padding: 10px;
    margin: 5px;
    display: inline-block;
    width: 20%;
    text-align: center;
    background: #fff;
  }

---

# Installer son Environnement

## Maîtriser les outils fondamentaux du développeur

**Objectif :** Configurer un espace de travail sécurisé, robuste et conforme aux exigences du Titre Professionnel DWWM.

---

# Étape 1 : Les Fondations

## Pourquoi la configuration est la clé du succès technique ?

---

# Les 4 Piliers de l'Environnement

| Outil | Rôle Principal | 
| ----- | ----- | 
| **IDE (VS Code)** | Écriture, organisation et formatage du code. | 
| **Git** | Gestion des versions et collaboration d'équipe. | 
| **Docker** | Isolation des services (BDD, Serveurs) via conteneurs. | 
| **Qualité & Sécurité** | Audits, Linters et protocoles de transfert sécurisés. | 

---

# Chronologie d'Installation

La mise en place suit un ordre logique strict pour éviter les erreurs de dépendances :

1. **Système (OS)** : Installation de WSL2 (Windows) ou préparation du terminal.
2. **Core Tools** : Installation de VS Code et de Git.
3. **Virtualisation** : Installation de Docker Desktop.
4. **Vérification** : Test des commandes et configuration des clés SSH.
5. **Finalisation** : Votre environnement est "Prêt à Coder".

---

# L'Impact d'un Bon Setup

### Critères de Performance (REAC) :

* **100% Conformité :** Votre environnement doit simuler la production.
* **Isolation :** Pas de pollution entre les projets (un projet A ne doit pas casser un projet B).
* **Sécurité :** Utilisation systématique de clés SSH pour les accès serveurs.

> "Un environnement mal configuré est la première source de bugs en production."

---

# Maîtriser le Versionnage Git

Git permet de suivre l'évolution de votre code comme une "machine à remonter le temps" :

* **Le Commit** : Une photo de votre code à un instant T.
* **La Branche** : Un espace de travail parallèle (ex: `develop` pour les tests, `main` pour le stable).
* **Le Merge** : La fusion du travail validé vers le projet principal.

*Workflow type :*
`Modif locale` ➡️ `git add` ➡️ `git commit` ➡️ `git push` (envoi au serveur)

---

# L'Approche par Conteneurs (Docker)

Au lieu d'installer les outils directement sur votre machine, on utilise des **Conteneurs** :

* **Isolation :** Chaque projet possède sa propre version de PHP ou Node.
* **Reproductibilité :** Le projet fonctionne à l'identique chez tous vos collègues.
* **Sécurité :** Les services (Base de données) sont enfermés dans des boîtes étanches.

**Le flux Docker :**
`Votre PC` ➡️ `Lien Volume` ➡️ `Conteneur Docker` ➡️ `Serveur Web / BDD`

---

# Configuration de VS Code

### Extensions Vitales
* **Prettier** : Formatage automatique.
* **ESLint** : Détection d'erreurs en direct.
* **GitLens** : Historique visuel des modifications.

### Accessibilité (TSA/ADHD)
* **Thèmes High Contrast** : Pour une meilleure lisibilité.
* **Indentation Rainbow** : Pour voir la structure des blocs d'un coup d'œil.
* **Mode Zen** : Pour masquer les menus inutiles et rester concentré.

---

# Checklist de Validation

Utilisez ces commandes pour vérifier que tout est prêt :

| Élément | Commande à taper | Résultat attendu | 
| ----- | ----- | ----- | 
| **WSL/Linux** | `whoami` | Votre nom d'utilisateur | 
| **Git** | `git --version` | Version 2.x ou supérieure | 
| **Docker** | `docker ps` | Un tableau (même vide) | 
| **SSH** | `ls -l ~/.ssh` | Fichiers `id_rsa` listés | 

---

# Sécurité et Qualité du Code

* **Gestion des Secrets :** Utilisation de fichiers `.env` (à ne jamais envoyer sur Git).
* **Transferts Sécurisés :** Publication via **SSH/SFTP** uniquement.
* **Accessibilité :** Intégration d'outils d'audit (Lighthouse) dès le début du projet.
* **Veille Technologique :** S'abonner aux alertes de sécurité pour vos outils.

---

# Documentation & Veille

## Communiquer et Apprendre

Documenter son environnement est une compétence transversale **MAJEURE** du titre professionnel.

1. **README** : Guide d'installation et d'utilisation du projet.
2. **Anglais B1** : Savoir lire et comprendre la doc technique.
3. **Veille quotidienne** : 
    - S'informer des évolutions technologiques.
    - S'informer des évolutions en matière de sécurité


---
# Documentation & README

Le fichier `README.md` est le document le plus important de votre projet :

1. **Pré-requis** : Ce qu'il faut installer et exécuter le projet.
2. **Lancement** : Comment exécuter le projet.
3. **Scripts utiles** :  pour l'équipe de développement.

> "**Si ce n'est pas documenté, cela n'existe pas.**"

---

# Prêt à Coder ?

## Des questions sur la configuration ?