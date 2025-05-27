# CarrefourDATA
Projet de veille Fusion Acquisition pour CARREFOUR


# CAS D'usage

Le projet a poiur objectif de d'actualiser le fichier. 
1. Actualisé l'appartenance ou non d'une marque à la holding ainsi qu'avoir la nouvelle holding si nécessaire
2. Connaître l'acquisition de nouvelle marques des holdings présentes dans le fichier 
---

## Objectif

- Vérifier l'appartenance actuelle d'une marque à une holding.
- S'appuyer sur des **sources fiables, récentes et multiples** (presse, bases d'entreprises, plateformes M&A).
- Générer un fichier Excel enrichi avec les résultats de l’analyse.

---

## Fonctionnalités

- Requête structurée via **Perplexity AI** avec exclusion de Wikipedia.
- Ajout automatique des colonnes : `Statut`, `Score`, `Date de vérification`, `NEW Holding`.
- Format de réponse contrôlé pour faciliter l’analyse automatique.
- Sauvegarde d’un fichier Excel de sortie daté.

---

Exemple de librairie 

pandas as pd
os
from dotenv import load_dotenv
from datetime import datetime
from openai import OpenAI
re
time
sys

---

## Fichier Excel attendu

2 fichiers sont attendus : 
Un fichier CarrefourVC_
Un fichier NewBrandsDetection_

Le script ajoutera les colonnes suivantes :


