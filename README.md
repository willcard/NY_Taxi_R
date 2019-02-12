# New York Taxi R data visualisation

## Description du contexte

Dans le cadre de notre unité "R and Data Visualisation" nous devions, en utilisant le langage R, créer et générer des graphiques représentant les données et expliquant ces dernières.
Nous avons donc choisi d'utiliser les données kaggle suivante : https://www.kaggle.com/naveenkaveti/eda-10-points/data
Ce dataset regroupe les données recueillis sur les taxi new-yorkais lors de l'année 2016.

## Les données

Les données sont sour un format csv
Le fichier à une taille de 231,4 Mo
Vous pouvez télécharger les données à l'URL suivant : http://perso.esiee.fr/~coviller/NY_taxi.csv
Dans ce dataset, nous pouvons trouver différentes données intéressantes comme les lieux de départs et d'arrivées des courses de taxi, le moment de ces arrivées et départs, le nombre de passagers par taxi etc.
Pour plus de détail, nous vous invitons à aller sur la page kaggle qui explique de manière exhaustive le dataset (https://www.kaggle.com/naveenkaveti/eda-10-points/data)

## Installation des packages R

Ce projet nécessite l'installation de plusieurs packages R. Afin de s'assurer que le code puisse s'exéccuter, veuillez à bien exécuter la commande suivante :

# Chargement des packages nécessaires
list.of.packages <- c("ggplot2", "Rcpp","IRdisplay","dplyr","leaflet",
                      "leaflet.extras","gridExtra")
new.packages <- list.of.packages[!(list.of.packages %in% installed.packages()[,"Package"])]
if(length(new.packages)) install.packages(new.packages)

library(IRdisplay)
library(dplyr)
library(leaflet)
library(leaflet.extras)
library(ggplot2)
require(gridExtra)
