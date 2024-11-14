# Description du Projet

Bienvenue à bord ! Notre entreprise traverse actuellement une période critique suite au départ de notre administrateur système. L'infrastructure qu'il a laissée est à la fois non sécurisée et partiellement défaillante, ce qui a paralysé de nombreux départements et services qui dépendent de notre plateforme web hébergée. Nous craignons également une cyberattaque imminente dans les semaines à venir.

Votre mission est de prendre en charge l'infrastructure et de la réparer le plus rapidement possible. L'application web doit être fonctionnelle dans les plus brefs délais, avec un système d'inventaire complet (et non seulement une gestion des utilisateurs).

## Contraintes

1. L'API ne doit pas être sur le même hôte que l'application web et ne doit pas être déplacée.
2. Tous les services doivent être conteneurisés et lancés avec l'utilisateur `service-web`.
3. Mettre en place un système de journalisation complet pour l'API et le tester de manière exhaustive.
4. Mettre en place un système d'intégration et de déploiement scripté en utilisant GitLab.
5. Utiliser un logiciel de gestion des artefacts lié au système d'intégration et de déploiement pour éviter la disponibilité directe du code source sur des hôtes peu fiables.

## Informations Disponibles

Le site web est hébergé sur quatre machines virtuelles, chacune contenant un service : la plateforme web, l'API, la base de données et la surveillance (gérée par Portainer). La configuration de l'automatisation est incomplète et aucun serveur GitLab n'est installé.

## Démarrage Rapide

### Frontend

**Sans Docker :**
1. Exécutez `yarn install` pour installer les dépendances.
2. Exécutez `yarn start` pour lancer l'application en local.
3. Exécutez `yarn run build` pour construire la version de production de l'application dans le dossier build.

**Avec Docker :**
1. Exécutez `docker-compose up --build -d; cd back && docker-compose up --build -d` pour lancer l'application sur localhost:8080.

### Backend

**Sans Docker :**
1. Exécutez `yarn install` pour installer les dépendances.
2. Exécutez `yarn start` pour lancer l'application sur le port 3000 en local.
3. Exécutez `yarn run build` pour construire la version de production de l'application dans le dossier build.

**Avec Docker :**
1. Exécutez `docker-compose up --build -d; cd back && docker-compose up --build -d` pour lancer l'application sur localhost:3000.

## Identifiants

Voici quelques identifiants qui pourraient être utiles :
- `test:test`
- `admin:admin`
- `john:fJrUkjsh_0~E1&`
- `john:john`
- `baba:express`
- `root:aSecurePasswordMustBeAtLeast128CharactersLongIncludingDifferentStuff`
- `root:doNotCommunicate`
- `no_rights:no_rights`
- `toto:toto`
- `titi:tata`
- `user:password`

## Sécurité et Déploiement

- Identifier et corriger les vulnérabilités sans mettre à jour la pile technique.
- Fournir des recommandations et des meilleures pratiques pour le renforcement des services.
- Préparer une démonstration de la plateforme web fonctionnelle connectée à une base de données pour la phase d'acceptation.

## Contact

Pour toute question, veuillez rester en contact avec Gina, votre responsable.