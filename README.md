# Pour utiliser le projet

```
// cloner le repo
git clone git@github.com:O-clock-Lara/projet-02-barbiche-skin-front.git

// passer sur la branche dev
git checkout dev

// mettre à jour la version de node.js si jamais on travaille sur la VM O'clock
sudo npm install -g n
sudo n lts

// récupérer les dépendances
yarn 

// lancer le serveur front
yarn start

// lancer le serveur back (dans le repo du back)
php -S 0.0.0.0:8000 -t public

// pour choisir les endpoints API (prod ou localhost),
// aller dans le dossier middlewares et le fichier sourceAPI.js
// commenter la ligne de source que l'on ne veut pas utiliser 
// décommenter la ligne de source que l'on veut utiliser

// si jamais le login ne fonctionne pas (erreur 500), il faut aller dans le repo back, 
// supprimer les fichiers public.pem private.pem dans le dossier config\jwt 
// regénérer ces clefs en tapant
php bin/console lexik:jwt:generate-keypair

```
