Ce projet constitue le **serveur backend** de notre application ionic du repository (https://github.com/MT98/thiop). Il contient la base de données **SQLite** permettant de stocker les données de l'application et l'ensemble des **webservices** permettant d'effectuer des requêtes Http à partir de notre application ionic cliente précitée. Ce serveur backend a été facilement créé grâce à la plateforme **strapi**.    
    
    
    
# Intégration du projet dans votre local
    
### 1. Installation
Il faut d'abord installer la structure d'un projet strapi de manière globale. C'est la manière la plus simple d'éviter les problémes de dépendances de bibliothéques à l'intégration du projet strapi aprés l'avoir téléchargé du dépôt github.    
Pour ce faire, placez-vous dans votre repertoire de base et **taper les commandes suivantes:**    

* ```npm -g uninstall strapi --save``` pour désinstaller l'installation existante de strapi afin d'installer une version alpha globale. 
* Consulter le dossier node_modules contenant les packages globales du gestionnaire de paquets (%AppData%\Roaming\npm pour windows) et supprimer le dossier strapi s'il est toujours là.    
* ```npm install strapi@alpha -g``` pour installer la version alpha strapi de manière globale. 
* ```npm install sqlite3 ```
* ```strapi new thiopstrapi --quickstart``` pour créer le nouveau projet strapi définissant notre serveur backend.
    
### 2. Téléchargement et décompression
Téléchargez le repository du README que vous lisez actuellement dans votre local. Puis décompressez-le.

### 3. Intégration    
Copiez le contenu du dossier api se trouvant dans la racine du dossier téléchargé.    
Puis collez-le à l'intérieur du dossier api se trouvant à la racine du dossier installé à l'étape 1.    
Ce qui vous permettra de disposer de l'ensemble des webservices et modèles créés dans ce repository directement dans votre nouveau projet.

### 4. Redemarrage du serveur strapi
Pour redemarrer le serveur du dossier installé à l'étape 1:
* Taper Ctrl-C en ligne de commande pour arrêter le serveur.  
* Assurer vous que le port 1337 n'est pas toujours occupé par un processus. 
* ```cd thiopstrapi``` pour se placer dans le repertoire de base du dossier installé.
* ```strapi start``` pour le démarrer.    

Au cas où le serveur échoue dans le démarrage, supprimer le dossier .tmp et démarrer le server.

Vous devriez avoir un résultat similaire:    
![Démarrage serveur réussie](https://drive.google.com/uc?id=10iMChxQ-cZaGgI9_k6m9Kbf7ePvEtK3V)    
    
### 5. Configuration au navigateur    
Utilisez votre navigateur et aller à l'adresse http://localhost:1337/admin afin de créer votre compte admin.
Aprés connexion, vous verrez les modèles déjà créés dans le menu. Comme suit:    
![Modèles pré-éxistants](https://drive.google.com/uc?id=12o4FWpqRxHbcvcGu0vtIYRL_DL9062QJ)
    
Maintenant dans le menu, aller dans Rôles et autorisations. Puis cliquer sur public dans la page affiché.    
Cocher "Tout cocher" pour chaque modèle. Puis sauvegarder la configuration.


### 6. Tester les webservices
Aller à l'adresse http://localhost:1337/Plats. Vous devriez obtenir un tableau vide comme suit:    
![Requêtes plats](https://drive.google.com/open?id=1r6VK5OKSxnzT4vhKdMV0IwQbWWebS6ej)    

Il va falloir maintenant remplir notre base de données. Et c'est là qu'entre en jeu notre application cliente développée avec ionic. Je vous invite donc à aller au repository https://github.com/MT98/thiop.


