# Utilisez l'image Docker officielle de Nginx basée sur Alpine
FROM nginx:alpine

# Copiez le fichier index.sh dans le répertoire HTML de Nginx
COPY index.sh /usr/share/nginx/html/index.sh

# Exposez le port 80 pour accéder à Nginx depuis l'extérieur du conteneur
EXPOSE 80

# Commande pour démarrer Nginx en mode daemon
CMD ["nginx", "-g", "daemon off;"]
