Voici une liste des commandes courantes et des étapes associées à Flask, à partir de l'installation et de la configuration :

### **1. Installation et Configuration de Flask**

1. **`pip install Flask`** : Installe Flask via `pip`, le gestionnaire de paquets de Python.

2. **`export FLASK_APP=app.py`** *(Linux/macOS)* / **`set FLASK_APP=app.py`** *(Windows)* : Définit la variable d'environnement pour spécifier le fichier principal de l'application Flask.

3. **`export FLASK_ENV=development`** *(Linux/macOS)* / **`set FLASK_ENV=development`** *(Windows)* : Active le mode de développement avec rechargement automatique et affichage des erreurs détaillées.

### **2. Commandes de Base pour Développer et Gérer une Application Flask**

4. **`flask run`** : Lance le serveur de développement Flask, accessible par défaut à `http://127.0.0.1:5000`.

5. **`flask shell`** : Ouvre un shell interactif Python avec le contexte de l'application Flask chargé.

6. **`flask routes`** : Liste toutes les routes définies dans l'application Flask.

7. **`flask db init`** : Initialise le répertoire de migration de la base de données pour Flask-Migrate (extension pour la gestion des migrations).

8. **`flask db migrate -m "description"`** : Crée une nouvelle migration basée sur les changements apportés aux modèles de données.

9. **`flask db upgrade`** : Applique les migrations à la base de données pour synchroniser la structure avec les modèles.

10. **`flask db downgrade`** : Annule la dernière migration, revenant ainsi à l'état précédent de la base de données.

### **3. Création et Gestion d’Extensions Flask**

11. **`pip install Flask-SQLAlchemy`** : Installe l'extension Flask-SQLAlchemy pour l'intégration de SQLAlchemy dans Flask.

12. **`pip install Flask-Migrate`** : Installe Flask-Migrate pour la gestion des migrations de base de données.

13. **`pip install Flask-Login`** : Installe Flask-Login pour gérer l'authentification des utilisateurs dans Flask.

### **4. Commandes Utiles pour le Développement**

14. **`flask test`** : Commande personnalisée (nécessite implémentation) pour exécuter les tests unitaires de l'application.

15. **`flask run --host=0.0.0.0`** : Lance le serveur Flask pour être accessible depuis toutes les interfaces réseau, utile pour le développement sur un réseau local.

16. **`flask run --port=8000`** : Lance le serveur Flask sur un port différent (par exemple, 8000).

### **5. Commandes pour Déploiement**

17. **`pip install gunicorn`** : Installe Gunicorn, un serveur WSGI compatible avec Flask pour déployer l'application en production.

18. **`gunicorn -w 4 app:app`** : Lance l'application Flask avec Gunicorn en utilisant 4 workers pour traiter les requêtes.

### **6. Commandes pour le Débogage et l'Environnement**

19. **`export FLASK_DEBUG=1`** *(Linux/macOS)* / **`set FLASK_DEBUG=1`** *(Windows)* : Active le mode débogage pour Flask, utile pendant le développement pour un rechargement automatique et des messages d'erreur détaillés.

20. **`flask run --reload`** : Lance le serveur Flask avec le rechargement automatique du code source.

### **7. Gestion des Environnements Virtuels (Recommandé pour Flask)**

21. **`python -m venv venv`** : Crée un environnement virtuel nommé `venv`.

22. **`source venv/bin/activate`** *(Linux/macOS)* / **`venv\Scripts\activate`** *(Windows)* : Active l'environnement virtuel.

23. **`deactivate`** : Désactive l'environnement virtuel actif.

### **8. Installation des Dépendances**

24. **`pip freeze > requirements.txt`** : Génére un fichier `requirements.txt` listant toutes les dépendances du projet, utile pour déployer l'application sur un autre environnement.

25. **`pip install -r requirements.txt`** : Installe toutes les dépendances listées dans `requirements.txt`.