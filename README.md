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

* statique = mm contenu pr ts users
* dynamique = contenu personnalisé en fonction du user, contexte... données du contenu proviennent de bdd

## <a name="mvc"></a>Le MVC

* modele vue controleur
* user demande 1 page. controleur verifie avec modele si info existe en bdd. si oui demande à vue page à afficher pour cette info. sinon demande à vue message d'erreur à afficher. la page succès ou erreur et renvoyée au user.

[![Architecture MVC (Modèle - Vue - Contrôleur)](https://img.youtube.com/vi/PuBjF8CRWWE/0.jpg)](https://www.youtube.com/watch?v=PuBjF8CRWWE)

## <a name="routes"></a>Les routes

config/routes.rb = fichier qui définit différents chemins pour app web rails, cad où doit pointer chaque url

## <a name="bdd"></a>Les Bases de Données

* sorte de tableur excel géant
* fichier ou ensemble de fichiers ou on stocke des infos pour y accéder plus facilement et rapidement
* principe est d'avoir des clés/identifiants pour identifier le contenu et le lier à d'autre contenu de la bdd

[![Comprendre les bases de données](https://img.youtube.com/vi/tmMmEYknwek/0.jpg)](https://www.youtube.com/watch?v=tmMmEYknwek)

## <a name="getpost"></a>GET / POST

* get = on demande de recevoir une info au serveur. dans url
* post = on envoie une info au serveur pour qu'il l'enregistre. dans body

[![Differences Between Get and Post](https://img.youtube.com/vi/UObINRj2EGY/0.jpg)](https://www.youtube.com/watch?v=UObINRj2EGY)

(Vidéo en anglais avec sous-titres)

## <a name="migr"></a>Le concept de migration

MAJ bdd ?

## <a name="models"></a>Les relations entre les models des BDD

???

## <a name="crud"></a>Les fonctions du CRUD

* Create = créer élément
* Read = lire l'élément
* Update = mettre à jour l'élément
* Destroy = suprimer l'élément
