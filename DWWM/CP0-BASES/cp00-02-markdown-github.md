# Syntaxe Markdown GitHub

## Qu'est-ce que Markdown ?

Markdown est un langage simple pour écrire des documents lisibles.

GitHub utilise Markdown pour :

- les README ;
- la documentation ;
- les issues ;
- les pull requests ;
- les discussions.


## 1. Les titres

Les titres structurent le document.

```markdown
# Titre niveau 1
## Titre niveau 2
### Titre niveau 3
#### Titre niveau 4
```
Résultat : 

# Titre niveau 1
## Titre niveau 2
### Titre niveau 3
#### Titre niveau 4

GitHub crée automatiquement un sommaire (table des matières) à partir des titres.

2. Mise en forme du texte

- Gras `**texte**`
    - Résultat : **texte**
- Italique `*texte*`
    - Résultat : *texte*
Italique
*texte*


Résultat : texte

Gras + italique
***texte***


Résultat : texte

Barré
~~texte~~


Résultat : texte

Souligné
<ins>texte</ins>


Résultat :

texte

Indice
<sub>texte</sub>


Exemple : H2O

Exposant
<sup>texte</sup>


Exemple : x2

3. Les citations

Pour citer un texte :

> Citation


Résultat :

Citation

Très utile pour afficher une remarque ou une référence.

4. Le code
Dans une phrase
`npm install`


Résultat :

npm install

Bloc de code
```javascript
console.log("Bonjour");
```


GitHub colore automatiquement le code selon le langage indiqué.

5. Les couleurs

GitHub reconnaît certains formats de couleur :

`#0969DA`

`rgb(9, 105, 218)`

`hsl(212,92%,45%)`


Une prévisualisation de la couleur apparaît dans les issues et discussions.

6. Les liens
Lien simple
https://github.com


Résultat :

https://github.com

7. Les liens vers une section

Vous pouvez créer un lien vers un titre du document.

# Installation

#installation


GitHub génère automatiquement les ancres.

8. Les liens relatifs

Pour relier des fichiers du même dépôt :

docs/guide.md


C'est la méthode recommandée dans un projet GitHub.

9. Les ancres personnalisées

Vous pouvez créer un point de navigation précis.

<a name="debut"></a>


Puis :

#debut


Pratique pour les longs documents.

10. Les retours à la ligne

Dans un fichier Markdown :

Ajouter :

deux espaces à la fin d'une ligne ;
ou \ ;
ou <br>.

Exemple :

Ligne 1  
Ligne 2

11. Les images
images/logo.png


Le texte entre crochets est le texte alternatif utilisé pour l'accessibilité.

GitHub recommande d'utiliser des chemins relatifs dans les projets.

12. Les listes
Liste à puces
- HTML
- CSS
- JavaScript


ou

* HTML
* CSS


ou

+ HTML
+ CSS

Liste numérotée
1. Analyse
2. Conception
3. Développement

13. Les listes imbriquées
1. Front-end
   - HTML
   - CSS
   - JavaScript


Permet de créer plusieurs niveaux d'information.

14. Les listes de tâches

Très utilisées en gestion de projet.

- [ ] Installer Node.js
- [x] Créer le dépôt Git


Résultat :

 Installer Node.js
 Créer le dépôt Git
15. Les mentions

Pour notifier une personne :

@nom_utilisateur


Pour notifier une équipe :

@organisation/equipe


GitHub envoie une notification.

16. Les issues et Pull Requests

Référence à une issue :

#123


GitHub crée automatiquement le lien correspondant.

17. Les ressources externes

GitHub peut aussi créer automatiquement des liens vers :

Jira ;
Zendesk ;
autres outils configurés dans l'entreprise.
18. Télécharger des fichiers

Dans :

les issues ;
les pull requests ;
les commentaires ;
les fichiers Markdown.

Vous pouvez :

glisser-déposer ;
coller ;
sélectionner un fichier.
19. Les emojis
:+1:
:rocket:
:tada:


Résultat :

👍 🚀 🎉

20. Les paragraphes

Laisser une ligne vide :

Paragraphe 1

Paragraphe 2

21. Les notes de bas de page
Voici une référence[^1].

[^1]: Explication.


La note apparaît en bas du document.

22. Les alertes GitHub

GitHub propose des blocs spéciaux.

NOTE
> [!NOTE]
> Information utile

TIP
> [!TIP]
> Astuce

IMPORTANT
> [!IMPORTANT]
> À connaître absolument

WARNING
> [!WARNING]
> Risque important

CAUTION
> [!CAUTION]
> Attention aux conséquences


Ces blocs attirent l'œil du lecteur.

23. Les commentaires cachés
<!-- commentaire -->


Le contenu n'apparaît pas dans le rendu final.

24. Échapper les caractères Markdown

Pour afficher un caractère Markdown sans appliquer sa mise en forme :

\*texte\*


Résultat :

*texte*

25. Afficher le Markdown brut

Sur GitHub, il est possible de désactiver le rendu Markdown pour voir le code source du fichier.

À retenir (version DWWM)

Pour un développeur web, les éléments indispensables sont :

✅ Titres (#)
 ✅ Paragraphes
 ✅ Gras et italique
 ✅ Listes
 ✅ Liens
 ✅ Images
 ✅ Blocs de code
 ✅ Checklists
 ✅ Alertes (NOTE, TIP, WARNING)
 ✅ Ancres de navigation
 ✅ Mentions (@)
 ✅ Références d'issues (#123)

Ces fonctionnalités couvrent environ 95 % des besoins d'un README professionnel ou d'une documentation technique GitHub.