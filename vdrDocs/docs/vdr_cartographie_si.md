# vdr_cartographie_si

## Cahier des charges : Analyse du besoin

La cartographie du système d'information permet de visualiser et comprendre l'ensemble des composants et des interconnexions du système d'information de la Mairie de Val-de-Reuil. Voici les étapes à suivre pour réaliser cette cartographie :

1. **Collecte des informations** :

   - Réunir les documents existants sur l'infrastructure IT actuelle.
   - Rencontrer les différents responsables de services pour obtenir des informations supplémentaires.
2. **Identification des composants du SI** :

   - Réseaux (LAN, WAN, VLAN).
   - Serveurs (physiques, virtuels).
   - Applications métiers (AxelNet, MobiliEcole).
   - Bases de données (MySQL, PostgreSQL).
   - Postes de travail (PC, tablettes).
3. **Représentation graphique** :

   - Utiliser un outil de mind mapping pour créer une représentation visuelle du SI.
     * Nœuds principaux : Réseaux LAN, WAN, VLAN, Serveurs (physiques, virtuels), Applications métiers (AxelNet, MobiliEcole), Bases de données (MySQL, PostgreSQL), Postes de travail (PC, tablettes).
     * Sous-nœuds : détailler chaque composant en incluant des informations telles que les adresses IP, les versions logicielles, les interconnexions, etc.
4. **Relations et interconnexions** :

   - Identifier et représenter les liens entre les différents composants du SI.
   - Utiliser des flèches pour indiquer les flux d'informations ou de données entre les composants.
5. **Documentation complémentaire** :

   - Ajouter des notes ou des commentaires pour fournir des explications supplémentaires sur certains éléments du SI.
   - Inclure des informations sur la sécurité, la disponibilité et la performance de chaque composant.
6. **Mise à jour régulière** :

   - Planifier des sessions de mise à jour régulières pour maintenir la cartographie du SI à jour avec les évolutions et les changements.
7. **Partage et collaboration** :

   - Utiliser un outil collaboratif pour permettre aux différentes parties prenantes d'accéder à la cartographie du SI et de contribuer aux mises à jour.
8. **Utilisation de la cartographie du SI** :

   - Aider à la prise de décision en identifiant les points faibles et les opportunités d'amélioration du SI.
   - Faciliter la communication et la compréhension entre les différents acteurs du SI.
   - Servir de référence lors de l'élaboration de nouvelles stratégies ou de nouveaux projets.

## Cartographie du système d'information : Piste de réflexion

- [ ] A Faire

1. Liste des corps métiers :
2. Le Découpage Réseau

   - Le Réseau
   - Le Sous-Réseau
3. L'inventaire du parc informatique

   - Les Ordinateurs Portables
   - Les Ordinateurs Fixes
   - Les Tablettes
   - Les Téléphones Portables
   - Les Téléphones Fixes
   - Les Imprimantes
   - Les Caméras connectées
   - Les Serveurs
   - Les Switchs
   - Les licences (MsOffice_365)
4. Départements ou Services Municipaux
5. Outils, Logiciels utilisés
6. Internes
7. Externes
8. Criticité (élevée, moyen, faible, non défini)
9. Urgent
10. Important
11. Tableau visuels
12. Nomenclatures
13. Projets en cours
14. Les Acteurs
15. Observations
16. Liste de potentiel logiciel de cartographie
17. Rôle Délégué à la protection des données (DPO)
18. Règlement Général sur la Protection des Données (RGPD)

## Benchmark des communes ayant fait une cartographie de leur système d'information

#### Benchmark : Logiciels libres Architecture d'entreprise (AE)

1. Modelio

   - Installation : [lien vers le site](https://www.modelio.org/). L'outil est on premise, s'installe et se désinstalle facilement. Sous licence GNU-GPL, Modelio gère bien un référentiel d'objets d'entreprise. Il ne permet pas le partage entre plusieurs utilisateurs autorisés. On peut juste exporter le projet, le transmettre à un autre utilisateur qui pourra l'importer. Modelio propose des diagrammes de types Business Process Modeling (BPMN) et UML.
2. Visual Paradigm (online)

   - SaaS online uniquement, [consulter le site](https://www.visual-paradigm.com). L'outil offre plusieurs templates variés, au choix de l'utilisateur.
3. ADOIT
4. Archi (Arch imatetool)
5. GenMyModel
6. Draw.io
7. Mercator

### Métiers : Services de la Commune

!!! info "Ecosystème"
    Vue d'ensemble : Processus, technologies, données, personnes

    Vue métier du SI : Processus et information clés qui sont nécessaire pour que le SI remplisse sa fonction. "Valeurs Métiers"

#### Tableau des Métiers : Vue Métier

| Nom                                    | Description                 | Responsable                      | @mail                    | code |
| :------------------------------------- | :-------------------------- | :------------------------------- | :----------------------- | :--- |
| Finances                               | Administration et Finances  | Maria Guibert                    | mguibert@valdereuil.fr   | 1    |
| Ressources Humaines                    | Administration et Finance   | Elodie Barbey, Matthieu Chevanne | mchevanne@valdereuil.fr  | 1    |
| Centre Communal d'action social (CCAS) | Directions Opérationnelles | Sonia Rossignol                  | srossignol@valdereuil.fr | 1    |
| Enfance-Jeunesse-et-emploi             | CCAS                        | Agnès Dupain                    | adupain@valdereuil.fr    | 1    |

#### Tableau services : Vue Processus

!!! info "Vue Processus"
    Il me faudra décomposer la gestion de la paie :
    Besoins : Procéder utiliser pour effectuer la paie

| Services                        | Processus                                                                       | Logiciels |
| :------------------------------ | :------------------------------------------------------------------------------ | :-------- |
| Gestion des ressources humaines | -Paie -Carrière -Agents -Retraite -Congés                                     | x         |
| Enfance et Jeunesse             | Inscription -Revenus -Données sur la santé des enfants                        | x         |
| Tiers, Subvention Budget        | Données_Financières_et_Bancaires -Données_Personnelles -Données_Entreprises | x         |

#### Tableau : Vue Application

!!! info "Vue applicative"
    Décrire les composants du logiciels du SI , des services offerts, et les flux de données entre eux.
    La vue de l'administration : Nous allons répertorier les périmètres et les niveaux de privilèges : utilisateurs et admin

| Applications/Logiciels | Services A                          | Service B  | Données         |
| :--------------------- | :---------------------------------- | :--------- | :--------------- |
| Horoquartz -> 2        | Gestion des Ressources Humaines-> 3 | Finances 4 | <-temps/agents 1 |

#### Tableau : Vue Infrastructure

!!! info "Vue Infrastructure"
   La vue des Infra Logiques : Cloisonnement logique des réseaux, la définition des plages d'adresses IP, les VLAN, des fonctions de Filtrages
   La vue des Infra Physique : Description des équipements physique utilisés par le SI

| Services                               | Plage @IP | Nom ou code VLAN | Equipements          | Licences      |
| :------------------------------------- | :-------- | :--------------- | :------------------- | :------------ |
| Finances                               |           | 1                | PC, Mac, Workstation | O365          |
| Ressources Humaines                    |           | 1                | .........            | ...........   |
| Centre Communal d'action social (CCAS) |           | 1                | ...........          | ............. |
| Enfance-Jeunesse-Petite Enfance CCAS   |           | 1                | ............         | ............. |

## Mercator

Mercator est un outil open source permettant de mettre en place une cartographie du système d'information. Il respecte le guide mis en place par l'ANSSI et a été développé par Didier Barzin, RSSI.

### Prérequis

Avant de commencer, assurez-vous de disposer des éléments suivants :

- Un serveur de production avec les caractéristiques suivantes :
  - Système d'exploitation : Fedora Server 64 bits
  - RAM : 2 Go
  - Disque : 20 Go
  - VCPU : 2

## Installation

### Mise à jour du système

Avant d'installer Mercator, mettez à jour votre système en exécutant la commande suivante :

```bash
dnf update --refresh -y
```

### Installation des dépendances

Installez les dépendances nécessaires en exécutant les commandes suivantes :

```bash
dnf install php-zip php-curl php-mbstring php-dom php-ldap php-soap php-xdebug php-mysql php-gd libapache2-mod-php php-fpm php-mysqlnd
dnf install httpd
```

### Configuration d'Apache

Démarrez le service Apache et configurez-le pour qu'il démarre automatiquement au démarrage du système :

```bash
systemctl start httpd
systemctl enable httpd
```

### Installation de MariaDB

Installez MariaDB en exécutant la commande suivante :

```bash
dnf install mariadb-server
```

Démarrez le service MariaDB et configurez-le pour qu'il démarre automatiquement au démarrage du système :

```bash
systemctl start mariadb
systemctl enable mariadb
```

### Installation de Git et Composer

Installez Git et Composer en exécutant les commandes suivantes :

```bash
dnf install git composer
```

## Configuration de Mercator

Clonez le projet Mercator depuis GitHub en exécutant la commande suivante :

```bash
git clone https://www.github.com/dbarzin/mercator /var/www/mercator
```

Accédez au répertoire du projet Mercator :

```bash
cd /var/www/mercator/mercator
```

Mettez à jour les dépendances de Composer en exécutant la commande suivante :

```bash
composer update
```

Publiez tous les paquets depuis le gestionnaire des paquets de PHP en exécutant la commande suivante :

```bash
php artisan vendor:publish --all
```

## Configuration de la base de données

### Installation de MySQL

Installez MySQL en exécutant la commande suivante :

```bash
dnf install mysql-server
```

Démarrez le service MySQL et configurez-le pour qu'il démarre automatiquement au démarrage du système :

```bash
systemctl start mysqld
systemctl enable mysqld
```

### Création de la base de données

Connectez-vous à MySQL en tant qu'utilisateur root et créez une base de données pour Mercator :

```sql
mysql -u root -p

CREATE DATABASE mercator CHARACTER SET utf8 COLLATE utf8_general_ci;
CREATE USER 'vrd_user'@'localhost' IDENTIFIED BY 's3cr3t';
GRANT ALL PRIVILEGES ON mercator.* TO 'vrd_user'@'localhost';
FLUSH PRIVILEGES;
EXIT;
```

### Configuration de Mercator

Créez un fichier `.env` à la racine du projet Mercator en copiant le fichier `.env.example` :

```bash
cp .env.example .env
```

Modifiez le fichier `.env` pour y ajouter les informations de connexion à la base de données.

Exécutez les migrations pour créer les tables de la base de données :

```bash
php artisan migrate --seed
```

Générez une clé d'application en exécutant la commande suivante :

```bash
php artisan key:generate
```

Nettoyez le cache des configurations en exécutant la commande suivante :

```bash
php artisan config:clear
```

## Démarrage du serveur web

Démarrez le serveur web en exécutant la commande suivante :

```bash
php artisan serve -d
# Dans mon exemple en virtuelle pour accéder à l'hote depuis mon addresse il faut lancer la commande suivante 
php artisan server --host 10.110.12.158 --port 8000
```

Vous pouvez maintenant accéder à l'application Mercator depuis votre navigateur à l'adresse [http://localhost:8000](http://localhost:8000).

## Prise en main

Une fois connecté, vous pouvez commencer à remplir et administrer les données internes
