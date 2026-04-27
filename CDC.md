# Cahier des charges
# TamScore 

## 1-	Présentation du projet  
### 1-1-	Contexte 
Projet personnel réalisé dans le cadre d'une alternance en Data Analysis, visant à monter en compétence sur la modélisation et la manipulation de bases de données relationnelles complexes, à travers la conception d'un projet full-stack complet, from scratch.
### 1-2-	Présentation de la marque
TamScore est un site web de statistiques dédiée au football africain, couvrant les équipes nationales, la CAN et les compétitions CAF. Le site centralise et visualise les données de matchs (résultats, en direct, programme), les statistiques de joueurs et d'équipes, ainsi que les données par saison. Son nom est composé de deux termes : "Tam" issu de la langue Mə̀dʉ̂mbὰ (Medumba) de l'Ouest Cameroun, qui provient de “Tamkù” = “Football” et de “Score” en anglais. De manière globale, le site devra proposée du contenu telque l'on peut retrouver sur les sites classiques telsque SofaScore et BeSoccer.  
### 1-3-	Objectifs du projet
- Concevoir et modéliser une base de données relationnelle complexe sous PostgreSQL
- Développer un site web full-stack connecté à cette base de données
- Intégrer un module de reporting via Power BI Desktop

## 2. Périmètre fonctionnel
### 2.1 Fonctionnalités principales (modules du site)
TamScore s'articule autour de 7 modules fonctionnels : 
#### Module 1 - MATCHS
Affichage des matchs en temps réel, des résultats passés et du programme à venir, pour l'ensemble des compétitions couvertes. Ce module constitue le coeur du site
- Scores en direct (live)
- Résultats des matchs passés
- Programme des matchs à venir
- Détail d'un match (compositions, évènements, stats du match)
#### Module 2 - COMPETITIONS
Couverture des compétitions africaines officielles suivantes, constituant le périmètre de la version 1 du projet :
|Compétition|Type|Organisateur|
|---|---|---|
|CAN|Equipes nationales|CAF|
|Ligue des Champions CAF|Clubs|CAF|
|Coupe de la Confédération CAF(CCAF)|Clubs|CAF|
|MTN Elite One|Clubs(Cameroun)|FECAFOOT|

Chaque compétition dispose d'une page dédiée avec classements, résultats par journée/phase, classement des meilleurs joueurs par catégorie de stats (meilleurs buteurs, passeurs, etc...) et historique par édition.
#### Module 3 - EQUIPES NATIONALES
Suivi des sélections africaines engagées dans les compétitions couvertes.
- Fiche équipe nationale (confédération, classement FIFA, palmarès)
- Effectifs et joueurs convoqués
- Statistiques de l'équipe par compétition et par saison
- Historique des performances
#### Module 4 - CLUBS
Suivi des clubs engagés dans les compétitions couvertes (Ligue des Champions CAF, CCAF, Elite One).
- Fiche club (pays, stade, palmarès)
- Effectif
- Statistiques du club par compétition et par saison
#### Module 5 - Joueurs
Suivi des joueurs africains et des joueurs binationaux sélectionnables par une équipe nationale africaine.
- Profil joeur (nationalité, poste, pied fort, date de naissance, club actuel)
- Statistiques personnelles (buts, passes, cartons, temps de jeu, etc...)
- Historique de carrière
- Classement des meilleurs joueurs, selon divers catégories de stats (meilleur buteur, passeurs, etc...)
- Ballon d'or africain (classement et historique)
#### Module 6 - Reporting Power BI
Intégration de tableaux de bord analytiques produits via Power BI Desktop, connectés à la BDD PostgreDQL. (à voir...)
- Visualisations avancées (tendances, comparatifs, performances historiques)
- Rapports par compétition, équipe ou joueur
- Destiné à une lecture analytique approfondie, en complément des pages statistiques du site
- ... (à voir)
#### Module 7 - Administration 
Interface d'administration sécurisée permettant la gestion des données du site sans intervention directe en base.
- Gestion des compétitions, éditions et phases
- Gestion des équipes (nationales et clubs)
- Gestion des joueurs et de leurs affiliations
- Saisie et correction des matchs et résultats
- Gestion des utilisateurs admin

### 2.2 Fonctionnalités hors périmètre (ce que le projet ne couvre pas)
Les éléments suivants sont explicitement exclus du périmètre de la version 1 de TamScore. Ils pourront faire l'objet d'évolutions ultérieures.

**Compétitions et championnats**
Les championnats nationaux africains autres que la MTN Elite One camerounaise (championnat égyptien, marocain, sud-africain, etc.)
Les compétitions de jeunes (CAN U20, U17)
Les compétitions féminines (CAN Féminine, Ligue des Champions CAF Féminine)
Les compétitions de beach soccer et futsal
Les compétitions confederales hors CAF (UEFA, CONMEBOL, etc.)

**Joueurs & stats**
Les statistiques contextuelles des joueurs africains évoluant à l'étranger (classements, résultats de leurs clubs étrangers, données de leurs championnats)
Les agents, contrats et données financières des joueurs (valeur marchande, salaires)
Les statistiques physiques avancées (distance parcourue, sprints, données GPS)

**Fonctionnalités utilisateur**
La création de comptes utilisateurs publics (pas d'espace membre, ni favoris, ni alertes)
Les commentaires, forums ou fonctionnalités communautaires
Les pronostics et paris sportifs
Les notifications push ou alertes par email

**Contenu éditorial**
Les articles, actualités ou contenus rédactionnels
Les transferts et mercato
Les conférences de presse et déclarations

**Technique**
Une application mobile native (iOS / Android)
Un système de cache distribué ou infrastructure cloud avancée
Une API publique exposée à des tiers

## 3. Utilisateurs cibles & cas d'usage

### 3.1 Profils utilisateurs
### 3.2 Parcours utilisateurs principaux

## 4. Spécifications fonctionnelles

### 4.1 Module Matchs (résultats, live, programme)
### 4.2 Module Équipes nationales
### 4.3 Module Joueurs & statistiques
### 4.4 Module Compétitions (CAN, CAF)
### 4.5 Module Saisons
### 4.6 Module Reporting (Power BI)

## 5. Spécifications techniques

### 5.1 Architecture globale (stack technique)
### 5.2 Base de données (PostgreSQL)
### 5.3 Backend
### 5.4 Frontend
### 5.5 Intégration Power BI
### 5.6 Alimentation des données (source, ingestion)

## 6. Modélisation de la base de données

### 6.1 Entités principales
### 6.2 MCD / MLD
### 6.3 Règles de gestion

## 7. Contraintes & exigences non fonctionnelles

### 7.1 Performance
### 7.2 Sécurité
### 7.3 Scalabilité
### 7.4 Maintenabilité

## 8. Livrables attendus
## 9. Planning prévisionnel
## 10. Glossaire



