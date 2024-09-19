# TP2 Symfony - CodeXpress

Ce projet est une mise à jour du projet CodeXpress, réalisé dans le cadre du TP2 Symfony du 19/09/2024.

## Objectifs du TP

1. Mettre à jour les templates Twig à partir du dépôt [codexpress-sf](https://github.com/Jensone/codexpress-sf).
2. Faire évoluer les entités selon le nouveau schéma fourni.
3. Mettre à jour la base de données avec une nouvelle migration.
4. Mettre à jour les fixtures et remplir la base de données.
5. Coder de nouveaux templates Twig : `/note/new.html.twig` et `/profile/edit.html.twig`.

## Installation du projet

1. Clonez ce dépôt :
git clone https://github.com/Matheo93/TP2symfonyMB.git
Copy
2. Installez les dépendances :
composer install
Copy
3. Configurez votre base de données dans le fichier `.env`.

4. Créez la base de données :
php bin/console doctrine:database:create
Copy
5. Exécutez les migrations :
php bin/console doctrine:migrations:migrate
Copy
6. Chargez les fixtures :
php bin/console doctrine:fixtures:load
Copy
7. Lancez le serveur Symfony :
symfony server:start
php -S localhost:8000 -t public
Copy
## Fonctionnalités principales

- Création de notes publiques ou privées par les utilisateurs.
- Édition du profil utilisateur.
- Attribution automatique de l'utilisateur actuel lors de la création d'une note.

## Technologies utilisées

- Symfony 7.1
- Twig
- Doctrine ORM
- Tailwind CSS

## Auteur

Matheo93
