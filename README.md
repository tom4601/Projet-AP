# Gestion du Parc Informatique MyGest

## 1) Présentation Générale
Ce projet est un script Bash qui permet de gérer l'inventaire d'un parc informatique à l'aide d'une base de données MySQL. L'application permet de consulter, ajouter, modifier et supprimer des équipements répertoriés dans la base de données MyGest.

L'objectif de ce projet est de proposer une interface simple en ligne de commande pour interagir avec la base de données et manipuler les informations du parc informatique.

## 2) Détails des Fonctionnalités

### Consultation des données
L'utilisateur peut consulter les informations stockées dans la base de données via un menu interactif. Il peut choisir d'afficher :
- Toutes les informations du parc,
- Uniquement les machines
- Uniquement les serveurs,
- Uniquement les switches

### Ajout de données
L'utilisateur peut ajouter un nouvel équipement en fournissant les informations suivantes :
- Nom de l'équipement,
- Adresse MAC,
- Adresse IP,
- Masque CIDR,
- Type d'équipement (Machine, Switch, Serveur).

Une requête SQL est ensuite exécutée pour insérer ces informations dans la base de données.

### Suppression de données
L'utilisateur peutsupprimer un équipement en fournissant son ID. Une requête SQL est alors exécutée pour supprimer l'enregistrement correspondant dans la base de données.

### Modification de données
L'utilisateur peut modifier les informations d'un équipement existant en indiquant son Id et les nouvelles valeurs pour :
- Nom,
- Adresse MAC,
- Adresse IP,
- Masque CIDR,
- Type d'équipement.

Une requête SQL est ensuite exécutée pour mettre à jour les informations de l'équipement dans la base de données.

## Installation et Exécution
### Prérequis
- Un serveur MySQL 
- Un utilisateur MySQL avec les droits nécessaires sur la base de données MyGest


### Installation
1. Clonez ce dépôt GitHub 

2. Importez la base de données 

3. Exécutez le script Bash 


## Demonstration video


## Sources
