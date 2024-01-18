# Utilisez une image nginx légère comme base
FROM nginx:alpine

# Supprimez les fichiers par défaut de nginx
RUN rm -rf /usr/share/nginx/html/*

# Copiez le contenu de votre application front-end dans le répertoire par défaut de nginx
COPY . /usr/share/nginx/html

# Exposez le port 80 pour permettre l'accès à l'application
EXPOSE 80
