# Gestion du Parc Informatique MyGest

## Présentation Générale
Le projet vise à développer un programme pour simplifier la gestion des systèmes et réseaux pour les techniciens. Il est decompose en 3 parties:

Partie 1 - Gestion du parc : Cette section permet de gérer un inventaire du parc informatique à l'aide d'une base de données MyGest. Elle inclut des fonctionnalités telles que la consultation, l'ajout, la suppression et la modification des équipements du réseau.

Partie 2 - Outils réseau : Elle fournit plusieurs outils permettant de tester l’état du réseau. Par exemple, des outils pour tester la connectivité d'une adresse IP, vérifier l'ouverture d'un port TCP, ou encore générer un fichier .txt avec des informations extraites de la base de données.

Partie 3 - Installateur : Cette partie garantit la bonne installation et configuration du programme, en vérifiant les prérequis, comme les paquets nécessaires, et en différenciant entre une machine serveur et cliente. Un script d'installation initialise la configuration et crée la base de données.

## Détails des Fonctionnalités

Le script pour la Partie 1 permet de gérer efficacement l’inventaire du parc informatique à l’aide d’une base de données MyGest. Il propose plusieurs fonctionnalités essentielles :

Connexion à la base de données : Avant toute interaction, le script vérifie la connexion à la base MyGest avec l’utilisateur u1. Si la connexion échoue, un message d’erreur s’affiche et le programme s’arrête.

Menu principal interactif :

Consultation des équipements : Possibilité d'afficher tous les équipements ou de filtrer par type (machines, serveurs, switches).
Ajout d’un nouvel équipement : L’utilisateur entre les informations nécessaires (nom, adresse MAC, adresse IP, CIDR, type).
Suppression d’un équipement : Suppression d’un équipement en indiquant son ID.
Modification d’un équipement : Mise à jour des informations d’un équipement existant en saisissant son ID et les nouvelles valeurs.
Option de sortie pour quitter proprement le programme.
Chaque action repose sur des commandes SQL exécutées directement depuis le script. L’ensemble permet une gestion simple et rapide du parc informatique sans nécessiter une interface graphique.

Avec le script de la Partie 2 - Outils réseau, on peux également tester la connectivité des équipements, vérifier l’ouverture des ports et générer un fichier contenant toutes les IP enregistrées. Ces outils complètent la gestion du parc en ajoutant des fonctionnalités de diagnostic réseau.

La Partie 3 vise à automatiser la configuration et l'installation des éléments nécessaires au bon fonctionnement du programme. Elle inclut la vérification et l'installation des paquets requis, la création et la configuration de la base de données, ainsi que la génération du fichier config.sh. Elle distingue également si le programme est utilisé sur un serveur ou une machine cliente pour adapter les paramètres en conséquence.

## Mes réalisations

### Consultation des données
L'utilisateur peut consulter les informations stockées dans la base de données via un menu interactif. Il peut choisir d'afficher :
- Toutes les informations du parc,
- Uniquement les machines
- Uniquement les serveurs,
- Uniquement les switches

  
<img width="336" alt="Screenshot 2025-03-20 at 15 29 53" src="https://github.com/user-attachments/assets/21978ecb-80ca-43d4-96db-f53fda6e7069" />

  
<img width="339" alt="Screenshot 2025-03-20 at 15 30 02" src="https://github.com/user-attachments/assets/d46cb77a-8b7d-4e39-a122-ebd88bef84ee" />


### Ajout de données
L'utilisateur peut ajouter un nouvel équipement en fournissant les informations suivantes :
- Nom de l'équipement,
- Adresse MAC,
- Adresse IP,
- Masque CIDR,
- Type d'équipement (Machine, Switch, Serveur).

Une requête SQL est ensuite exécutée pour insérer ces informations dans la base de données.

<img width="284" alt="Screenshot 2025-03-20 at 15 30 45" src="https://github.com/user-attachments/assets/cd16ae5f-049f-4257-b687-5e8422311882" />


### Suppression de données
L'utilisateur peutsupprimer un équipement en fournissant son ID. Une requête SQL est alors exécutée pour supprimer l'enregistrement correspondant dans la base de données.

<img width="280" alt="Screenshot 2025-03-20 at 15 31 30" src="https://github.com/user-attachments/assets/8dea34bf-a62d-4d94-9dde-cc76726d804e" />


### Modification de données
L'utilisateur peut modifier les informations d'un équipement existant en indiquant son Id et les nouvelles valeurs pour :
- Nom,
- Adresse MAC,
- Adresse IP,
- Masque CIDR,
- Type d'équipement.

Une requête SQL est ensuite exécutée pour mettre à jour les informations de l'équipement dans la base de données.

<img width="291" alt="Screenshot 2025-03-20 at 15 31 12" src="https://github.com/user-attachments/assets/d5d02541-9ccf-4bd8-80df-dcc23ba77062" />


## Installation et Exécution
### Prérequis
- Un serveur MySQL 
- Un utilisateur MySQL avec les droits nécessaires sur la base de données MyGest


### Installation
1. Clonez ce dépôt GitHub 

2. Importez la base de données 

3. Exécutez le script Bash 


## Demonstration video

https://www.youtube.com/watch?v=UemAYIW3zXg


## Sources

-Documentation de pedagogeek.fr

-https://stackoverflow.com

-https://www.debian.org


