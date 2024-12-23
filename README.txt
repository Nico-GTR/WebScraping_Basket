================================================================
Projet NBA - Scraping et Analyse des Données NBA
================================================================

Ce projet vise à scraper des données sur les équipes NBA et leurs joueurs depuis le site basketball-reference.com grâce à une API, 
puis à les stocker dans des fichiers CSV et les présenter via différentes pages web.

##########################
Arborescence des fichiers
##########################

Projet NBA
│
├── Dossier Équipes
│   ├── Script de scraping
│   └── Dossiers d'informations sur les équipes
│
├── Dossier Joueurs
│   ├── Script de scraping
│   └── Dossiers d'informations sur les joueurs
│
├── Fichiers template HTML
│
├── Script d'installation des modules
│
├── Scripts de génération des pages HTML
│
├── Dossier Pages Équipes
│   └── Pages HTML des équipes
│
├── Dossier Pages Joueurs
│   └── Pages HTML des joueurs
│
└── Dossier CSS
    └── Fichiers de styles CSS

##########################
Installation
##########################

Avant de commencer à utiliser le projet, vous devez installer les modules nécessaires en exécutant le script installation_modules.py. 
Ce script vérifie et installe automatiquement toutes les bibliothèques Python requises.

Important : Après l'exécution du script, relancez le kernel Python pour que les installations soient prises en compte.

##########################
Dossier Équipes
##########################

Le fichier equipes.py scrappe les données des équipes NBA. Il récupère des informations sur chaque équipe, ses joueurs, ses statistiques, etc, et les exporte en fichiers CSV.

- 5 sous-dossiers sont créés
- Chaque sous-dossier contient 30 fichiers (.csv ou .jpg)
- Chaque fichier correspond à une équipe de la NBA

##########################
Dossier Joueurs
##########################

Le fichier joueurs.py scrappe les données des joueurs NBA, collectant des informations telles que :
- Nom
- Équipe
- Statistiques individuelles

Les données sont exportées en fichiers CSV.

######################################
Dossier Pages Équipes et Pages Joueurs
######################################

Les scripts suivants génèrent les pages HTML :
- page-menu.py
- pages_equipes.py
- pages_joueurs.py

Utilisation de 3 templates :
- menu_template.html
- equipe_template.html
- joueur_template.html

Les fichiers HTML générés sont stockés dans les dossiers Pages_Equipes et Pages_Joueurs.

##########################
Dossier CSS
##########################

Contient 3 feuilles de style :
- styles_menu.css
- styles_equipe.css
- style_joueurs.css

Ces fichiers gèrent la mise en forme des pages HTML.

##########################
Utilisation
##########################

1. Installer les modules avec installation_modules.py

2. Scraper les données des équipes : exécuter equipes.py
|-----> Il y a un risque que le nombre de requête autorisées par le site sports-reference.com depuis une API soit limité. 
	Dans ce cas là, le scrapping des données sur les équipes va être interrompu.
	Il n'y a pas d'autres choix que de modifier le code et attendre un certain temps (non précisé par le site web) avant de relancer le scrapping.
	
3. Scraper les données des joueurs : exécuter joueurs.py

4. Générer les pages HTML : exécuter page-menu.py, pages_equipes.py, pages_joueurs.py

5. Ouvrir nba_equipe_joueurs.html pour naviguer entre les pages web

##########################
Contributeurs
##########################

- Manoubi Mahbouli
- Julien Pichon
- Nicolas Gautier