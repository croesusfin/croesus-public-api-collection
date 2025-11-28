# Croesus Public API Collection

Ce dépôt regroupe les collections d’APIs publiques Croesus, organisées pour faciliter le test, l’intégration et la documentation des différents services proposés par Croesus.

## Table des matières
- [Présentation](#présentation)
- [Structure du projet](#structure-du-projet)
- [Prérequis](#prérequis)
- [Installation](#installation)
- [Utilisation](#utilisation)
- [Organisation des environnements](#organisation-des-environnements)
- [Licence](#licence)

## Présentation
Ce projet propose des collections Bruno pour interagir avec les APIs publiques Croesus : Authentification, CRM, Gestion de portefeuille, etc. Il permet de tester les endpoints, gérer les environnements et documenter les flux d’authentification.

## Structure du projet
```
Croesus/
├── Auth/                # Authentification (First party, OAuth2 Third party)
├── Crm/                 # Gestion de la relation client (Accounts, Clients, Documents, etc.)
├── PFM/                 # Gestion de portefeuille (Positions, Transactions, Performances, etc.)
├── environments/        # Fichiers d’environnement
├── bruno.json           # Fichier de configuration Bruno
```
Chaque dossier contient des fichiers `.bru` pour les collections et les requêtes, ainsi que des fichiers `bruno.json` pour la configuration.

## Prérequis
- [Bruno](https://www.usebruno.com) (outil open-source pour tester les APIs REST)

## Installation
1. Installer Bruno :
   - [Télécharger Bruno](https://www.usebruno.com)
2. Cloner ce dépôt :
   ```powershell
   git clone https://github.com/votre-organisation/croesus-public-api-collection.git
   ```
3. Ouvrir le dossier dans Bruno.

## Authentification
- Utiliser la collection `Auth` pour obtenir des tokens d’accès
- Configurer les variables d’environnement nécéssaires (client_id, client_secret, etc.)
- Choisir le flux d’authentification approprié (First party (bearer token), OAuth2 Third party (openidconnect))
- Exécuter la requêtes pour obtenir la tokens

## Utilisation
- Sélectionner la collection souhaitée (Auth, Crm, PFM).
- Configurer l’environnement (token, variables, etc.).
- Exécuter les requêtes pour tester les endpoints.

## Organisation des environnements
Le dossier `environments/` contient des fichiers `.bru` pour différents environnements (ex : nonprod, production). Adaptez les variables selon vos besoins.

## Licence
Ce projet est sous licence propriétaire Croesus. Contactez l’éditeur pour toute utilisation commerciale ou redistribution.

# English Version

This repository gathers Croesus public API collections, organized to facilitate testing, integration, and documentation of the various services offered by Croesus.

## Table of Contents
- [Overview](#overview)
- [Project Structure](#project-structure)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Environment Organization](#environment-organization)
- [License](#license)

## Overview
This project provides Bruno collections to interact with Croesus public APIs: Authentication, CRM, Portfolio Management, etc. It allows you to test endpoints, manage environments, and document authentication flows.

## Project Structure
```
Croesus/
├── Auth/                # Authentication (First party, OAuth2 Third party)
├── Crm/                 # Customer Relationship Management (Accounts, Clients, Documents, etc.)
├── PFM/                 # Portfolio Management (Positions, Transactions, Performances, etc.)
├── environments/        # Environment files
├── bruno.json           # Bruno configuration file
```
Each folder contains `.bru` files for collections and requests, as well as `bruno.json` configuration files.

## Prerequisites
- [Bruno](https://www.usebruno.com) (open-source tool for testing REST APIs)

## Installation
1. Install Bruno:
   - [Download Bruno](https://www.usebruno.com)
2. Clone this repository:
   ```powershell
   git clone https://github.com/votre-organisation/croesus-public-api-collection.git
   ```
3. Open the folder in Bruno.

## Authentication
- Use the `Auth` collection to obtain access tokens
- Configure the required environment variables (client_id, client_secret, etc.)
- Choose the appropriate authentication flow (First party (bearer token), OAuth2 Third party (openidconnect))
- Run the requests to obtain tokens

## Usage
- Select the desired collection (Auth, Crm, PFM).
- Configure the environment (token, variables, etc.).
- Run requests to test the endpoints.

## Environment Organization
The `environments/` folder contains `.bru` files for different environments (e.g., nonprod, production). Adapt the variables as needed.

## License
This project is under Croesus proprietary license. Contact the publisher for any commercial use or redistribution.
