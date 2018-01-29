# Rails pour les Nuls

## Table des Matières

1. [La différence entre un site statique et un site dynamique](#statdyn)
2. [Le MVC](#mvc)
3. [Les routes](#routes)
4. [Les Bases de Données](#bdd)
5. [GET / POST](#getpost)
6. [Le concept de migration](#migr)
7. [Les relations entre les models des BDD](#models)
8. [Les fonctions du CRUD](#crud)

## <a name="statdyn"></a>La différence entre un site statique et un site dynamique

* Site statique = On distribue un même contenu à tous les utilisateurs.
* Site dynamique = Le contenu est personnalisé en fonction de l'utilisateur, du contexte... La plupart du temps, les données de contenu proviendront de la [BDD](#bdd).

## <a name="mvc"></a>Le MVC

* Modèle - Vue - Contrôleur. En anglais : Model - View - Controller.
* Cas d'utilisation : L'utilisateur demande une page d'article. Le contrôleur vérifie avec le modèle si l'article existe en BDD. Si oui, le contrôleur demande à la vue la page à afficher pour cet article. Sinon, le contrôleur demande à la vue la page de message d'erreur à afficher. La page d'article ou celle d'erreur est renvoyée à l'utilisateur.

![Image Modèle - Vue - Contrôleur](https://upload.wikimedia.org/wikipedia/commons/6/63/ModeleMVC.png "Modèle - Vue - Contrôleur")

Une vidéo vaut mieux que de longs discours :

[![Architecture MVC (Modèle - Vue - Contrôleur)](https://img.youtube.com/vi/PuBjF8CRWWE/0.jpg)](https://www.youtube.com/watch?v=PuBjF8CRWWE)

Je vous conseille également la lecture de l'[article Wikipedia](https://fr.wikipedia.org/wiki/Mod%C3%A8le-vue-contr%C3%B4leur), en français.

## <a name="routes"></a>Les routes

Dans un projet Rails, on trouvera le fichier *routes.rb* dans le répertoire *config*.

Le rôle de ce fichier est de définir les différents chemins pour l'application web Rails, c'est-à-dire là où doit pointer chaque URL.

## <a name="bdd"></a>Les Bases de Données

* Ou BDD en abrégé, ou encore DB (anglais pour database).
* C'est une sorte de tableur Excel géant.
* Fichier ou ensemble de fichiers où l'on stocke des informations/données pour y accéder plus facilement et rapidement
* Le principe est d'avoir des clés/identifiants pour identifier le contenu et le lier à d'autres contenus de la BDD.

Encore une vidéo explicative :

[![Comprendre les bases de données](https://img.youtube.com/vi/tmMmEYknwek/0.jpg)](https://www.youtube.com/watch?v=tmMmEYknwek)

## <a name="getpost"></a>GET / POST

* GET = On demande de recevoir une info au serveur. dans url
* POST = On envoie une info au serveur pour qu'il l'enregistre. dans body

Vidéo qui reprend les différences fondamentales entre GET et POST :

[![Differences Between Get and Post](https://img.youtube.com/vi/UObINRj2EGY/0.jpg)](https://www.youtube.com/watch?v=UObINRj2EGY)

(Vidéo en anglais avec sous-titres)

## <a name="migr"></a>Le concept de migration

MAJ bdd ?

## <a name="models"></a>Les relations entre les models des BDD

???

## <a name="crud"></a>Les fonctions du CRUD

* Create = Créer un élément
* Read = Lire/Afficher un élément
* Update = Mettre à jour un élément
* Destroy = Supprimer un élément
