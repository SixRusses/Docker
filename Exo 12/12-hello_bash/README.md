Nous avons un stagiaire qui a utilisé **`chatgtp`** pour créer le `Dockerfile`, mais malheureusement, cela ne fonctionne pas correctement et il est incapable de nous expliquer ce que le `Dockerfile` est censé faire. Voici donc ta mission : 

1. **Réviser le `Dockerfile`** : Assure-toi qu'il soit bien écrit et qu'il fonctionne comme prévu. Rectifie toute erreur que tu pourrais trouver. 

2. **Tester le déploiement** : Après avoir corrigé le `Dockerfile`, teste 

3. **Documenter le processus** : Rédige une explication claire de ce que chaque ligne du `Dockerfile` fait et comment cela contribue au fonctionnement global du projet.


## 📝 Rendu Attendu
un Dockerfile fonctionnel, accompagné d'un README. Ce README devra inclure une explication détaillée du projet. 



## EXPLICATION: 

1. FROM nginx:alpine : Cette ligne indique que nous utilisons l'image Docker officielle de Nginx basée sur Alpine Linux comme base pour notre image personnalisée.

2. COPY index.sh /usr/share/nginx/html/index.sh : Cette ligne copie le fichier index.sh dans le répertoire HTML par défaut de Nginx à l'intérieur du conteneur.


4. EXPOSE 80 : Cette ligne expose le port 80 du conteneur, sur lequel Nginx écoute les connexions HTTP.

5. CMD ["nginx", "-g", "daemon off;"] : Cette ligne spécifie la commande par défaut à exécuter lorsque le conteneur démarre. Ici, nous démarrons Nginx en mode daemon pour servir le contenu HTML.