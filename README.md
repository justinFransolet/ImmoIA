# ImmoIA

## Utilité

Intelligence Artificielle conçue pour les agences immobilières travaillant à la fois avec des clients particuliers et professionnels. 
Afin d'optimiser leurs propositions de biens immobiliers et de réduire le nombre de visites nécessaires, y compris virtuelles, 
l'agence envisage de recourir à l'intelligence artificielle.

## Traitement des données

Dans cette boucle, nous allons préparer notre jeu de données pour l'analyse et l'apprentissage automatique. 
Nous suivrons le processus suivant :

1. ### Importation des librairies et configuration de l'environnement

    Tout d'abord, nous allons importer les bibliothèques nécessaires et configurer notre environnement 
    pour une meilleure lisibilité des données et des graphiques.

2. ### Chargement et exploration des données

   Nous commençons par extraire les fichiers d'une archive .tgz puis nous chargeons les données du fichier CSV. 
   Ensuite, nous explorons la structure du jeu de données pour obtenir un aperçu des colonnes, des types de données et des valeurs manquantes.

3. ### Compréhension des données

   Nous produirons un résumé du jeu de données pour comprendre la distribution des variables et identifier les valeurs manquantes. 
   Les méthodes _info()_ et _describe()_ de **pandas** sont utilisées pour fournir des résumés concis et des statistiques descriptives.

4. ### Gestion des valeurs manquantes

   Pour simplifier, nous remplissons les valeurs manquantes dans les colonnes numériques avec la valeur médiane de chaque colonne. 
   Pour les colonnes catégorielles, nous utilisons la valeur la plus fréquente (mode) pour l'imputation.

5. ### Visualisation des données

   Nous utilisons diverses visualisations pour analyser la distribution des données et les relations entre les variables.
   Cela inclut des histogrammes pour les caractéristiques numériques, des diagrammes en barres pour les caractéristiques catégorielles, 
   des cartes de chaleur pour les corrélations et des cartes géographiques pour la visualisation spatiale des prix des maisons.

   Cette préparation des données nous permet de transformer notre jeu de données brut en un format propre et 
   prêt pour les analyses ultérieures et les **modèles d'apprentissage automatique**.
   Les résultats semblent prometteurs, les points rouges semblent correspondre à des zones avec lesquelles l'immobilier est plus cher.
   On utilise l'algorithme de **K-means** qui donne de meilleurs résultats en préparant au mieux son jeu de données de manière 
   à exploiter le potentiel de l'ensemble des données fournies.
   Cet algorithme est capable de séparer les données de la base en _k_ parties distinctes sans aucun paramètres préalables !
   Uniquement par une analyse intelligente des données entre elles !