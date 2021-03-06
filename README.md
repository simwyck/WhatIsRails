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

---

## <a name="statdyn"></a>La différence entre un site statique et un site dynamique

* Site statique = On distribue un même contenu à tous les utilisateurs.
* Site dynamique = Le contenu est personnalisé en fonction de l'utilisateur, du contexte... La plupart du temps, les données de contenu proviendront de la [BDD](#bdd).

## <a name="mvc"></a>Le MVC

* Modèle - Vue - Contrôleur. En anglais : Model - View - Controller.
* Cas d'utilisation : L'utilisateur demande une page d'article. Le contrôleur vérifie avec le modèle si l'article existe en BDD. Si oui, le contrôleur demande à la vue la page à afficher pour cet article. Sinon, le contrôleur demande à la vue la page de message d'erreur à afficher. La page d'article ou celle d'erreur est renvoyée à l'utilisateur.

![Image Modèle - Vue - Contrôleur](https://upload.wikimedia.org/wikipedia/commons/6/63/ModeleMVC.png "Modèle - Vue - Contrôleur")

Une vidéo vaut mieux que de longs discours :

[![Architecture MVC (Modèle - Vue - Contrôleur)](https://img.youtube.com/vi/PuBjF8CRWWE/0.jpg)](https://www.youtube.com/watch?v=PuBjF8CRWWE)

(Source de l'image : Wikipedia)

Je vous conseille également la lecture de l'[article Wikipedia](https://fr.wikipedia.org/wiki/Mod%C3%A8le-vue-contr%C3%B4leur), en français.

## <a name="routes"></a>Les routes

Dans un projet Rails, on trouvera le fichier *routes.rb* dans le répertoire *config*.

Le rôle de ce fichier est de définir les différents chemins pour l'application web Rails, c'est-à-dire là où doit pointer chaque URL.

## <a name="bdd"></a>Les Bases de Données

* Ou BDD en abrégé, ou encore DB (anglais pour database).
* C'est une sorte de tableur Excel géant.
* Fichier ou ensemble de fichiers où l'on stocke des informations/données pour y accéder plus facilement et rapidement
* Le principe est d'avoir des clés/identifiants pour identifier le contenu et le lier à d'autres contenus de la BDD.

Comme je le disais, schématiquement une BDD se présente comme un tableau :

**Clé** | **Valeur** | **Type**
--- | --- | ---
123456 | "Comme elle belle ma valeur" | String

Ceci est bien sûr une vision simplifiée mais ça vous donne l'idée :)

Encore une vidéo explicative :

[![Comprendre les bases de données](https://img.youtube.com/vi/tmMmEYknwek/0.jpg)](https://www.youtube.com/watch?v=tmMmEYknwek)

## <a name="getpost"></a>GET / POST

* GET = On demande de recevoir une info au serveur. Le GET se retrouvera directement comme argument dans l'URL.
* POST = On envoie une info au serveur pour qu'il l'enregistre. Le POST sera défini dans le body de la page HTML.

Vidéo qui reprend les différences fondamentales entre GET et POST :

[![Differences Between Get and Post](https://img.youtube.com/vi/UObINRj2EGY/0.jpg)](https://www.youtube.com/watch?v=UObINRj2EGY)

(Vidéo en anglais avec sous-titres)

## <a name="migr"></a>Le concept de migration

Tout simplement, la migration intervient lorsqu'on modifie la structure de la BDD.

Pour se faire, la commande utilisée dans Rails sera *db:migrate*. Auparavant, vous aurez modifié le fichier *schema.rb* dans le répertoire *db* et bien sûr sauvegardé ces modifications.

Pour en savoir plus (et parce que vous aimez les vidéos), je vous conseille de visionner l'excellent tutoriel de notre ami de Graphikart :

[![Apprendre Ruby on Rails : Les Migrations](https://img.youtube.com/vi/LBtCqTeJvfg/0.jpg)](https://www.youtube.com/watch?v=LBtCqTeJvfg)

## <a name="models"></a>Les relations entre les models des BDD

[Wikipedia][1] définit le modèle relationnel comme *"une manière de modéliser les relations existantes entre plusieurs informations, et de les ordonner entre elles. Cette modélisation qui repose sur des principes mathématiques mis en avant par E.F. Codd est souvent retranscrite physiquement (« implémentée ») dans une base de données."*

Pour une bonne introduction aux bases de données relationnelles, nous vous conseillons la vidéo suivante de l'EPFL :

[![Modèle relationnel des bases de données](https://img.youtube.com/vi/4etRfqKF1XE/0.jpg)](https://www.youtube.com/watch?v=4etRfqKF1XE)

## <a name="crud"></a>Les fonctions du CRUD

* Create = Créer un élément
* Read = Lire/Afficher un élément
* Update = Mettre à jour un élément
* Destroy = Supprimer un élément

**Graphikart** détaille le fonctionnement de CRUD dans [une vidéo](https://www.grafikart.fr/formations/ruby-on-rails/crud).

---

Powered by Simwyck / Slack & GiHub: @simwyck

[1]: https://fr.wikipedia.org/wiki/Mod%C3%A8le_relationnel
