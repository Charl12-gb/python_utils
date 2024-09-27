Voici une liste des commandes courantes et des étapes associées à Django, à partir de l'installation et de la configuration :

### **1. Installation et Configuration de Django**

1. Installe Django via `pip`, le gestionnaire de paquets de Python.
```
pip install django
```

2. Crée un nouveau projet Django avec le nom spécifié.
```
django-admin startproject <project_name>
```

3. Accède au répertoire du projet Django.
```
cd <project_name>
```

### **2. Commandes pour Gérer l'Application Django**

4. Crée une nouvelle application au sein du projet Django.
```
python manage.py startapp <app_name>
```

5. Lance le serveur de développement Django, accessible par défaut à `http://127.0.0.1:8000`.
```
python manage.py runserver
```

6. Lance le serveur de développement Django sur un port différent (par exemple, `http://127.0.0.1:8080`).
```
python manage.py runserver <port>
```

7. Crée des fichiers de migration basés sur les modifications apportées aux modèles de l'application.
```
python manage.py makemigrations
```

8. Applique les migrations à la base de données pour synchroniser la structure avec les modèles.
```
python manage.py migrate
```

9. Crée un utilisateur administrateur avec accès au panneau d'administration Django.
```
python manage.py createsuperuser
```

10. Ouvre un shell interactif Python avec le contexte du projet Django chargé.
```
python manage.py shell
```

11. Exécute les tests unitaires définis dans l'application Django.
```
python manage.py test
```

12. Collecte tous les fichiers statiques des applications pour les préparer au déploiement.
```
python manage.py collectstatic
```

13. Effectue une vérification du projet pour détecter des erreurs ou des problèmes courants.
```
python manage.py check
```

14. Ouvre une interface de ligne de commande pour interagir directement avec la base de données configurée.
```
python manage.py dbshell
```

15. Affiche une liste des migrations disponibles et leur état (appliqué ou non).
```
python manage.py showmigrations
```

16. Affiche les instructions SQL générées pour une migration spécifique.
```
python manage.py sqlmigrate <app_label> <migration_name>
```

### **3. Gestion des Migrations**

17. Crée des migrations spécifiques à une application donnée.
```
python manage.py makemigrations <app_name>
```

18. Applique les migrations d'une application spécifique.
```
python manage.py migrate <app_name>
```

19. Applique ou revient à une migration spécifique par son numéro ou son nom.
```
python manage.py migrate <app_name> <migration_number>
```

20. Combine plusieurs migrations en une seule pour optimiser le nombre de migrations.
```
python manage.py squashmigrations <app_name> <start_migration> <end_migration>
```

### **4. Commandes pour Débogage et Développement**

21. Lance le serveur de développement en utilisant un fichier de configuration spécifique.
```
python manage.py runserver --settings=<settings_module>
```

22. Affiche la différence entre les paramètres par défaut et ceux configurés pour le projet.
```
python manage.py diffsettings
```

23. Affiche les migrations avec un plan d'exécution.
```
python manage.py showmigrations --plan
```

24. Génère les commandes SQL nécessaires pour réinitialiser la base de données.
```
python manage.py sqlflush
```

25. Supprime toutes les données des tables de la base de données, mais conserve la structure.
```
python manage.py flush
```

26. Lance le serveur de développement avec des fonctionnalités supplémentaires pour le débogage.
- *(avec Django Extensions)*
```
python manage.py runserver_plus
```

### **5. Commandes pour le Déploiement**

27. Vérifie les configurations pour s'assurer qu'elles sont adaptées à un environnement de production.
```
python manage.py check --deploy
```

28. Collecte les fichiers statiques sans demander confirmation, utile pour l'automatisation du déploiement.
```
python manage.py collectstatic --noinput
```

29. Compresse et combine les fichiers CSS et JavaScript pour les optimiser en vue du déploiement.
- *(avec Django Compressor)*
```
python manage.py compress
```

### **6. Gestion des Environnements Virtuels (Recommandé pour Django)**

30. Crée un environnement virtuel nommé `venv`.
```
python -m venv venv
```

31. Active l'environnement virtuel.
- *(Linux/macOS)*
```
source venv/bin/activate
```

- *(Windows)*
```
venv\Scripts\activate
```

32. Désactive l'environnement virtuel actif.
```
deactivate
```

### **7. Installation des Dépendances**

33. Génère un fichier `requirements.txt` listant toutes les dépendances du projet, utile pour déployer l'application sur un autre environnement.
```
pip freeze > requirements.txt
```

34. Installe toutes les dépendances listées dans `requirements.txt`.
```
pip install -r requirements.txt
```

### **8. Commandes Utilitaires**

35. Exporte les données d'un modèle spécifique au format JSON.
```
python manage.py dumpdata <app_name>.<model_name>
```

36. Importe des données à partir d'un fichier JSON dans la base de données.
```
python manage.py loaddata <filename>
```

37. Ouvre une interface en ligne de commande pour interagir directement avec la base de données configurée.
```
python manage.py dbshell
```

38. Supprime les sessions expirées de la base de données.
```
python manage.py clearsessions
```

Ces commandes couvrent les principales actions nécessaires pour développer, tester, et déployer une application Django, en passant par la gestion de la base de données, l'administration des applications, et les pratiques recommandées pour le développement et le déploiement.