Ce projet constitue le **serveur backend** de notre application ionic du repository (https://github.com/MT98/thiop). Il contient la base de données **SQLite** permettant de stocker les données de l'application et l'ensemble des **webservices** permettant d'effectuer des requêtes Http à partir de notre application ionic cliente précitée. Ce serveur backend a été facilement créé grâce à la plateforme **strapi**.    
    
    
    
# Intégration du projet dans votre local
    
### 1. Installation
Il faut d'abord installer la structure d'un projet strapi de manière globale. C'est la manière la plus simple d'éviter les problémes de dépendances de bibliothéques à l'intégration du projet strapi aprés l'avoir téléchargé du dépôt github.    
Pour ce faire, placez-vous dans votre repertoire de base et **taper les commandes suivantes:**    

* ```npm -g uninstall strapi --save``` pour désinstaller l'installation existante de strapi afin d'installer une version alpha globale. 
* Consulter le dossier node_modules contenant les packages globales du gestionnaire de paquets (%AppData%\Roaming\npm pour windows) et supprimer le dossier strapi s'il est toujours là.    
* ```npm install strapi@alpha -g``` pour installer la version alpha strapi de manière globale.    
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
* ```cd thiopstrapi``` pour se placer dans le repertoire de base du dossier installé.
* ```strapi start``` pour le démarrer.    

Au cas où le serveur échoue dans le démarrage, supprimer le dossier .tmp et demmarer le server.

### 5. Configuration au navigateur
