Voici une liste des commandes courantes en Pyramid avec leurs explications :

1. **`pcreate -s starter <project_name>`** : Crée un nouveau projet Pyramid en utilisant un modèle de projet standard.

2. **`pserve development.ini`** : Lance le serveur de développement pour l'application Pyramid en utilisant le fichier de configuration `development.ini`.

3. **`initialize_<project_name>_db development.ini`** : Initialise la base de données pour l'application en fonction des modèles définis.

4. **`pdistreport`** : Affiche un rapport de distribution des paquets installés dans l'environnement Python.

5. **`pviews <package_name>`** : Liste toutes les vues définies dans un package Pyramid.

6. **`pshell development.ini`** : Ouvre un shell Python interactif avec le contexte de l'application Pyramid, permettant d'interagir avec les modèles et la base de données.

7. **`proutes <package_name>`** : Affiche toutes les routes définies dans le package spécifié.

8. **`prequest <url>`** : Effectue une requête HTTP sur l'URL spécifiée en utilisant le contexte de l'application Pyramid.

9. **`ptweens <package_name>`** : Affiche la chaîne de tweens configurée dans l'application Pyramid (middlewares internes).

10. **`pserve --reload development.ini`** : Lance le serveur de développement avec rechargement automatique du code lors des modifications.

11. **`proutes --glob`** : Affiche les routes en utilisant des correspondances glob pour filtrer les routes affichées.

12. **`pscripts`** : Liste tous les scripts d'administration Pyramid disponibles dans l'environnement actuel.

13. **`pcelery --ini development.ini`** : Démarre le processus Celery pour la gestion des tâches asynchrones en utilisant Pyramid.

14. **`pviews --global`** : Affiche toutes les vues globalement accessibles dans l'application Pyramid.

15. **`ptweens --global`** : Affiche les tweens (middlewares) globaux configurés dans l'application.

Ces commandes permettent de créer, gérer et déployer efficacement des applications Pyramid tout en offrant des outils pour le développement et le débogage.