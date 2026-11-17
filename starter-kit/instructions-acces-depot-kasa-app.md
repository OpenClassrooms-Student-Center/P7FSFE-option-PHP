# Accès et préparation du dépôt kasa-app

## Dépôt de départ

L'option B utilise le dépôt [Starter-P7-option-PHP-dfs-Front-end-avanc-](https://github.com/OpenClassrooms-Student-Center/Starter-P7-option-PHP-dfs-Front-end-avanc-). Créez votre propre dépôt à partir de ce dépôt de départ et rendez le lien vers votre dépôt. Travaillez sur des branches dédiées et gardez un historique de modifications lisible.

## Application fournie

Le dépôt contient une interface React avec Vite (`frontend/`) et une API PHP avec Symfony (`backend/`). Elles communiquent par HTTP. L'API lit le jeu de démonstration dans `starter-kit/donnees-logements-utilisateurs-kasa.csv` via `DATA_FILE` ; aucune base de données ni initialisation Doctrine n'est nécessaire.

Le CSV fictif contient 10 comptes, 12 logements et 2 séjours. L'application propose la consultation des logements, la connexion, les séjours, l'administration, les coordonnées de conciergerie et l'aperçu HTML d'un avis. Vérifiez les routes et le comportement réellement présents dans le code.

## Installation et lancement

Suivez le [README du dépôt](../README.md) pour les versions requises, l'installation séparée de l'API et de l'interface, les fichiers d'environnement et les commandes de lancement. Les fichiers `.env.local` ne doivent pas être publiés. Toute variable préfixée `VITE_` est transmise au navigateur et ne doit contenir aucun secret. N'inscrivez aucun mot de passe dans les livrables.

## Périmètre du travail

Le code de départ sert d'état initial à auditer. Les protections sont volontairement insuffisantes : repérez notamment les mots de passe en clair, les accès aux données sans contrôle adapté et les entrées renvoyées dans l'aperçu d'avis. Les variables liées à JWT, bcrypt et OAuth mentionnées dans la configuration ne prouvent pas qu'une protection est implémentée. Ne présentez une protection comme active que si le code la met effectivement en œuvre.

Le dépôt de départ ne fournit pas les tests automatisés ni la pipeline demandés par la mission. Le travail consiste à auditer puis à sécuriser les flux existants, ajouter les tests et une pipeline, et documenter les interventions réelles. N'ajoutez pas de fonctionnalité métier non demandée. Utilisez uniquement les données fictives fournies pour vos démonstrations.

## Documents à remettre

La note de sécurisation, les tests, leurs rapports de couverture, la configuration de la pipeline et le journal de maintenance doivent correspondre au même dépôt. Utilisez les modèles adaptés à l'option B et vérifiez vos commandes depuis un clone propre en suivant le README.
