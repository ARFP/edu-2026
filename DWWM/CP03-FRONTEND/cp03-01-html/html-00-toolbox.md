# La boîte à outils du Développeur Front-End

Avant d'écrire votre première ligne de code, vous devez préparer votre espace de travail. Un bon artisan travaille toujours avec les bons outils. En développement web, votre boîte à outils contient trois éléments essentiels.

> [!NOTE] 
>
> #### Objectifs pédagogiques
>
> - **Savoirs**
>   * **Identifier** les 3 piliers fondateurs du Web (URL, HTTP, HTML) et leur rôle respectif.
>   * **Différencier** le rôle du HTML (fond / structure) et du CSS (forme / design).
>   * **Distinguer** les caractéristiques du HTML et du XML.
>   * **Expliquer** le fonctionnement local d'un navigateur web.
> 
> - **Savoir-faire**
>   * **Configurer** un environnement de travail local propre.
>   * **Nommer** correctement les fichiers et dossiers selon les conventions professionnelles.
>   * **Utiliser** les fonctionnalités de base d'un IDE et l'inspecteur de code d'un navigateur.
>   * **Soumettre** un fichier HTML au validateur W3C pour auto-corriger ses erreurs de syntaxe.

---

> [!IMPORTANT]
>
> Avant de démarrer
> Il est recommandé d'avoir suivi la présentation sur la petite histoire du web et du HTML. 
> [Voir la présentation](./html-00-presentation.md)

<div style="page-break-after:always;"></div>

## 1. Le Navigateur Web (Votre Traducteur)

Une erreur fréquente au début est de penser qu'il faut obligatoirement "être sur Internet" ou payer un hébergeur pour créer un site web. *C'est faux*.

* Un navigateur (comme Google Chrome, Mozilla Firefox ou Brave) est simplement un **traducteur**. Le code HTML est un texte brut. Le navigateur lit ce texte et le traduit en images, en boutons et en paragraphes colorés à l'écran.
* Vous pouvez créer un fichier nommé `index.html` sur votre propre ordinateur et double-cliquer dessus. Votre navigateur va s'ouvrir et afficher votre page, **même si votre connexion internet est coupée**. On appelle cela *travailler "en local"*.

---

## 2. L'Environnement de Travail (Vos Outils de Production)

Pour coder de manière propre et rapide, vous allez utiliser deux outils au quotidien :

### L'Éditeur de Code (Exemple : VS Code)

C'est votre traitement de texte spécialisé pour le code. Contrairement à un bloc-notes classique, un éditeur comme *[Visual Studio Code](https://code.visualstudio.com/)* intègre des aides visuelles indispensables pour le confort mental :

* **La coloration syntaxique :** Les balises, les attributs et les textes s'affichent avec des couleurs différentes. Si vous oubliez de fermer une balise, la couleur change immédiatement. Cela permet de repérer une erreur en un coup d'œil.
* **L'auto-complétion :** L'éditeur devine ce que vous voulez écrire et ferme automatiquement les balises pour vous. Cela vous évite de faire des fautes de frappe.

#### Les extensions VsCode pour un développeur FrontEnd

* **[Prettier - Code Formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) :** L'outil indispensable pour la structure. Il reformate automatiquement le code (HTML, CSS, JS, JSON) à chaque sauvegarde. 
* **[Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) :** Permet de lancer un serveur local en un clic. Chaque modification enregistrée dans VS Code actualise instantanément le navigateur, offrant un retour visuel immédiat.
* **[Vue - Official](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (anciennement Volar) :** L'extension officielle pour le module VueJS. Elle apporte la coloration syntaxique et l'auto-complétion indispensables pour les fichiers `.vue` et la manipulation des composants.


### L'Inspecteur de Code (La touche F12)

C'est l'outil d'analyse intégré à votre navigateur. On l'appelle souvent "outils de développement" (*DevTools*).

* En appuyant sur la touche **F12** de votre clavier sur n'importe quel site web, vous ouvrez une fenêtre secrète.
* Cet outil fonctionne comme des **lunettes à rayons X** : il vous permet de voir le squelette HTML de n'importe quel site existant (Google, Wikipédia, ou votre propre travail) pour comprendre comment il est construit.

---

## 3. Le Validateur W3C (Votre Arbitre Neutre)

Le code informatique demande de la rigueur. Face à une page qui ne s'affiche pas comme vous le souhaitez, il est normal de ressentir de la frustration. Pour éviter de stresser, vous devez adopter un réflexe métier dès le premier jour : **utiliser le [Validateur W3C](https://validator.w3.org/)**.

* **Qu'est-ce que c'est ?** 
    * Le [W3C](https://www.w3.org/) est l'organisme international qui gère les règles du web. Ils mettent à disposition un outil en ligne gratuit. Vous lui donnez votre fichier `.html`, et la machine vérifie si vous avez respecté les règles.
* **Pourquoi l'utiliser ?** 
    * Au lieu de stresser et de vous demander *"Est-ce que mon code est bon ?"*, vous laissez le validateur juger de manière totalement neutre.
* **Le but du jeu** 
    * Corriger les lignes signalées par l'outil jusqu'à obtenir une validation complète. Transformer la correction du code en un jeu d'enfant consiste simplement à faire passer toutes les alertes au vert (🟢).
* **Adresse du validateur**
    * [https://validator.w3.org](https://validator.w3.org/)

<div style="page-break-after:always;"></div>

## 4. Les 3 Règles d'Or du rangement

Le code informatique déteste le désordre. Pour que votre traducteur (le navigateur) et vos outils s'y retrouvent, **vous devez respecter ces 3 règles strictes** dès aujourd'hui :


📁 **Un projet = Un dossier :** Ne laissez jamais traîner vos fichiers sur votre Bureau. Créez un dossier propre pour votre projet (ex: `projet-cv`). Tout ce qui concerne votre site (fichiers HTML, css, js, images) doit rester **à l'intérieur** de ce dossier.

> [!INFO] 
>
> Le reflexe du développeur pro :
> 
> 📁 **Un projet = Un dossier = Un dépôt GIT**


---

🛑 **Zéro majuscule, zéro espace :** Pour nommer vos fichiers et vos dossiers, utilisez uniquement des lettres minuscules, des chiffres et des *tirets du 6* (`-`).

| Nommage | ? |
| --- | --- |
| `MonDossier` | ❌ Mauvais |
| `mon-dossier` | ✅ Bon |
| `mondossier` | ✅ Bon |
|  |  |
| `ma page web.html` | ❌ Mauvais |
| `Ma-Page-Web.html` | ❌ Mauvais  |
| `ma-page-web.html` | ✅ Bon |

---

🏠 **Le fichier d'accueil s'appelle toujours `index.html` :** C'est une règle internationale. La page principale de votre site doit s'appeler exactement `index.html` (tout en minuscules). C'est ce nom précis que les serveurs et les navigateurs cherchent en premier pour afficher un site.

---
