![npm](https://img.shields.io/npm/v/modelize-cli)
![npm bundle size](https://img.shields.io/bundlephobia/min/modelize)
# Modelize
Modelize est un script NodeJS ayant pour but de transformer un fichier .sql ou une connexion vers une base de donnée en plusieurs modèle (un par table) pour différents ORM

## Disponibilité
#### Fichier SQL
- Syntaxe PostgreSQL
#### Base de donnée
- PostgreSQL
- MariaDB / MySQL
#### ORM
- Sequelize
- Eloquent

## Configuration

#### Fichier .sql

Un fichier `data.sql` contenant le script de création de vos tables utilisant les syntaxes supportées (Voir catégorie "Disponibilité"). Ne pas oublier les `;` en fin de requête pour la bonne exécution du script

#### Connexion à une base de donnée

Créez un fichier .env à la racine du projet contenant les informations suivantes :

    DB_HOST=<your_host_address>
    DB_PORT=<port_of_the_database> //If empty, it will take the default port of your SGBDR
    DB_USER=<username>
    DB_PASS=<password>
    DB_NAME=<name_of_the_database>
    

## Utilisation
 
Commande pour installer le projet :
`npm install -g modelize-cli`

Ensuite il vous suffit de lancer la commande suivante depuis la racine de votre projet :
`modelize`
