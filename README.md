Projet : Molécules et organismes
  
1. Introduction
Hier tu as vu comment faire un kit UI à partir de rien. Tu as réussi à définir un charte graphique, et c'est un bon début pour des sites pas trop moches. Aujourd'hui, nous allons te donner un kit déjà préfait, puis tu vas devoir construire des molécules et organismes à partir de ce kit. L'objectif est de te faire coder les quelques molécules qui vont prendre 80% de ton site, et comme ceci tu auras juste à les insérer pour un front qui déchire.

2. Le projet
Pour ce projet, nous allons te demander de partir sur un kit UI préfait. Ceci a deux avantages :

Déjà, tous les atomes sont désignés. Les tables, les forms, les alertes et bien d'autres. Pas d'oubli et tu seras prêt à faire des molécules et organismes au top
Ensuite, avec un kit UI déjà préfait, la mise en page sera beaucoup plus simple grâce au système de mise en page de Bootstrap
Ensuite, tu auras à réaliser les molécules et organismes suivants :

Une navbar
Un footer
L'organisme "formulaire d'authentification"
La bannière
Plusieurs formats de cartes de présentation
Puis les organismes qui représentent la listes de ces cartes
La molécule commentaire
L'organisme "section commentaires"
Une section "présentation ressource" qui sera grossomodo la section qui présente le show de n'importe quelle ressource
Une section qui présente un élément (à gauche du texte, à droite une image)
Un organisme de ton choix
Pour l'organisation ce sera simple, tu feras un fichier index.html qui va afficher plein de liens pour des pages contenant les molécules et organismes concernés. Ainsi, tu auras des fichiers navbar.html, footer.html, authentification_form.html, banner.html, etc. Le code CSS sera dans un fichier unique style.css, appelé par toutes tes pages.

Enfin, pour ce projet, nous allons te demander de l'imaginer pour ton projet Eventbrite. En effet, demain tu insèreras toutes les molécules dans ton application lorsque nous te montrerons la force de l'atomic design conjugué à Rails.

2.1. Choix d'un kit UI
Pour commencer, nous allons te demander de choisir un kit UI qui va bien. Va sur Bootswatch, puis choisis le thème qui t'inspire le plus pour Eventbrite.

🚀 ALERTE BONNE ASTUCE
Hier, tu as vu comment choisir des couleurs de BG et polices qui vont bien. Les thèmes Bootswatch ne sont au final qu'un fichier CSS que tu as à appeler dans ton application, et tu peux le modifier à ta guise. Par exemple faire un find and replace sur les codes couleur te permettra de changer aisément les couleurs de ton application.

2.2. Conception des molécules et organismes
Le gros de la journée, tu vas concevoir les molécules et organismes demandés. Pour ceci, tu vas devoir les imaginer pour la partie utilisateurs de l'application Eventbrite (ne prends pas en compte la partie Admin).

On ne recommandera jamais assez, mais la partie examples du site de Bootstrap contient un joli nombre de molécules exemples, avec une structure type d'une page html. Enfin, ce n'est jamais simple de devoir concevoir des molécules à partir de son imagination. Ainsi, pour chaque élément demandé, n'hésite pas à aller voir des exemples : les exemples de Bootstrap, ou alors les exemples des thèmes officiels de Bootstrap. À partir de ces exemples, tu prendras ton préféré, puis tu le dessineras sur un bout de papier, avant de concevoir le CSS de la molécule ou organisme.

L'exercice te demandera principalement de :

Essayer d'imaginer un design de molécule à partir de composants : jouer avec les briques des legos
Jouer avec du CSS et les classes Bootstrap pour faire de la mise en page
2.2.1. La navbar
Toute application qui se respecte se doit d'avoir une navbar qui permet de naviguer facilement dans les pages. Cet organisme sera assez simple à réaliser : tu n'as qu'à prendre un des exemples de Bootstrap et l'adapter à l'application Eventbrite !

2.2.2. Un footer
Pour cet exemple, tu devras faire un peu de CSS. Réfléchis bien à ce que tu veux mettre dans le footer, prends des exemples, puis designe-le.

2.2.3. Formulaire d'authentification
Aller sur un site professionnel et tomber sur cela quand tu veux changer de mot de passe, cela ne fait pas très professionnel. L'avantage est que ce genre de formulaire se ressemble beaucoup : deux-trois champs de formulaire, une checkbox, des liens, un bouton, et hop ! Par exemple, voici deux pages différentes au design très similaire : page 1, et page 2.

Imagine un design type pour tous les formulaires d'authentification :

Inscription
Connexion
Rentrer son email pour mot de passe oublié
Changement de mot de passe
Fais un design générique qui sera adapté à tous les formulaires.

2.2.4. Une bannière
En général, tout site qui se respecte se doit d'avoir au moins deux types de bannière :

Une grosse bannière, que l'on retrouve sur la page d'accueil (exemple)
Elle contient une image, un énorme titre, un paragraphe, puis un call to action
Une bannière plus petite, que l'on retrouve sur d'autres pages (exemple)
Elle contient en général une image, puis le titre de la page où nous nous trouvons
Imagine un design pour les deux types de bannière, puis code-les.

2.2.5. Les cartes de présentation, molécules et organismes
Les cartes sont très importantes. Tu en auras besoin pour :

Afficher une liste de carte d'événements
Afficher la liste des cartes des participants à un événement (des cartes horizontales comme celles-ci)
Afficher une liste de cartes de villes
Les cartes dans l'atomic design sont un élément très important, et c'est bien d'avoir plein de genre de cartes. Heuresemment, Bootstrap sont sympas et ont prévu le coup.

2.2.5.1. Les molécules : cartes
Construis les trois types de carte pour ce qui a été dit plus haut.

2.2.5.2. Les organismes : listes de cartes
Maintenant imagine les organismes qui vont aller avec ces cartes. Nous allons avoir besoin de listes pour les afficher :

Une liste qui affiche plusieurs cartes d'événements (mets-en le nombre que tu veux dans une row), qui sera un des organismes principaux de ta page d'accueil
Une liste qui affiche plusieurs cartes horizontales d'utilisateurs, qui sera un élément important dans la page qui affiche les participants à un événement
2.2.6. Les commentaires : molécule et organisme
Imaginons que l'on veuille afficher les commentaires de ton application. Voici comment nous allons procéder :

Il va falloir créer une molécule de commentaire, avec prénom de l'auteur, photo, contenu, et heure de post du commentaire
Puis nous allons devoir ajouter un textarea, un bouton "commenter", quelques séparateurs, et nous avons un organisme "section de commentaires".
Construis la molécule de commentaire, puis constuis l'organisme de la section de commentaires

2.2.7. Présentation ressource
Quand tu arrives sur la page d'un événement ou d'un utilisateur, il faut que ce soit affiché joliment. Par exemple, pour le vrai site Eventbrite, la page qui affiche les événements est bien organisée :

Tout dans un container
Une molécule d'une image qui prend 8 colonnes, et une section d'informations importantes qui prend 4 colonnes
Une molécule avec des icones, puis un bouton
Une molécule de la description qui prend 8 colonnes et du reste des informations sur les 4 colonnes restantes
Enfin, quelques icones de réseaux sociaux
Si tu arrives à faire cet organisme, il te sera très aisé de le reproduire pour d'autres ressources et d'autres pages show. Designe un organisme passe-partout, puis construis la molécule à partir de cela.

2.2.8. Présentation d'un élément
Sur les pages d'accueil, il arrive de présenter des éléments en mode : une photo à droite / gauche, du texte à gauche / droite. Tu peux trouver des exemples ici. Designes et construis ces sections.

2.2.9. Un organisme de ton choix
Tu as construit plein d'organismes, nous allons te demander de constuire un dernier : celui de ton choix. Réfléchis à l'application Eventbrite, puis essaie de voir une fonctionnalité en front qu'il manquerait. Designe-la, et construis-la.

3. Rendu attendu
Nous attendons à ce que tu rendes un dossier contenant toutes les molécules et organismes demandés. Petit bonus si tu arrives à présenter tout cela proprement :

Une page qui présente tout ton kit UI avec seulement les atomes (la page Bootswatch)
Puis plusieurs pages qui affichent les différentes molécules et organismes que tu as codés