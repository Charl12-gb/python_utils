Voici une liste des commandes courantes en Pyramid avec leurs explications :

1. Crée un nouveau projet Pyramid en utilisant un modèle de projet standard.
```
pcreate -s starter <project_name>
```

2. Lance le serveur de développement pour l'application Pyramid en utilisant le fichier de configuration `development.ini`.
```
pserve development.ini
```

3. Initialise la base de données pour l'application en fonction des modèles définis.
```
initialize_<project_name>_db development.ini
```

4. Affiche un rapport de distribution des paquets installés dans l'environnement Python.
```
pdistreport
```

5. Liste toutes les vues définies dans un package Pyramid.
```
pviews <package_name>
```

6. Ouvre un shell Python interactif avec le contexte de l'application Pyramid, permettant d'interagir avec les modèles et la base de données.
```
pshell development.ini
```

7. Affiche toutes les routes définies dans le package spécifié.
```
proutes <package_name>
```

8. Effectue une requête HTTP sur l'URL spécifiée en utilisant le contexte de l'application Pyramid.
```
prequest <url>
```

9. Affiche la chaîne de tweens configurée dans l'application Pyramid (middlewares internes).
```
ptweens <package_name>
```

10. Lance le serveur de développement avec rechargement automatique du code lors des modifications.
```
pserve --reload development.ini
```

11. Affiche les routes en utilisant des correspondances glob pour filtrer les routes affichées.
```
proutes --glob
```

12. Liste tous les scripts d'administration Pyramid disponibles dans l'environnement actuel.
```
pscripts
```

13. Démarre le processus Celery pour la gestion des tâches asynchrones en utilisant Pyramid.
```
pcelery --ini development.ini
```

14. Affiche toutes les vues globalement accessibles dans l'application Pyramid.
```
pviews --global
```

15. Affiche les tweens (middlewares) globaux configurés dans l'application.
```
ptweens --global
```

Ces commandes permettent de créer, gérer et déployer efficacement des applications Pyramid tout en offrant des outils pour le développement et le débogage.