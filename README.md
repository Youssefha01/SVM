# SVM
# Projet : Analyse de la santé cardiaque

## Description du projet

Ce projet vise à analyser des données sur la santé cardiaque en utilisant un jeu de données contenant des informations sur les patients, telles que leur âge, sexe, taille, poids, pression artérielle, cholestérol, glucose, habitudes de tabagisme, et le temps d'exercice. L'objectif principal est de construire un modèle de classification pour prédire la probabilité d'une crise cardiaque chez les individus en utilisant des techniques d'apprentissage automatique, notamment les Support Vector Machines (SVM).

## Détails du jeu de données

Le fichier `Heart_health.csv` contient les colonnes suivantes :

- **ID** : Identifiant unique du patient
- **Name** : Nom du patient
- **Age** : Âge du patient (en années)
- **Gender** : Genre du patient (0 pour féminin, 1 pour masculin)
- **Height(cm)** : Taille du patient (en centimètres)
- **Weight(kg)** : Poids du patient (en kilogrammes)
- **Blood Pressure(mmHg)** : Pression artérielle du patient (systolique/diastolique)
- **Cholesterol(mg/dL)** : Niveau de cholestérol (en mg/dL)
- **Glucose(mg/dL)** : Niveau de glucose (en mg/dL)
- **Smoker** : Indique si le patient fume (0 pour non, 1 pour oui)
- **Exercise(hours/week)** : Nombre d'heures d'exercice par semaine
- **Heart Attack** : Indique si le patient a eu une crise cardiaque (0 pour non, 1 pour oui)

## Étapes de l'analyse

1. **Chargement des bibliothèques** : Utilisation de bibliothèques comme `numpy`, `pandas`, `matplotlib`, et `seaborn` pour l'analyse des données.
2. **Chargement et inspection des données** :
   ```python
   import numpy as np
   import pandas as pd
   import matplotlib.pyplot as plt
   import seaborn as sns

   df = pd.read_csv('Heart_health.csv')
   data = df.copy()
   data.head()
