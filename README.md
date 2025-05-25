# CarrefourDATA
Projet de veille Fusion Acquisition pour CARREFOUR


# CAS D'usage

Ce script Python permet de **vérifier automatiquement** si une marque appartient toujours à une holding donnée, en utilisant PERPLEXITY et des critères professionnels de veille stratégique.

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

Le fichier source doit s’appeler `Group_7_holdings.xlsx` et contenir une feuille `Sheet1` avec les colonnes suivantes :

| Main Holding Name | Brand Name |
|-------------------|------------|
|                   |            |
|                   |            |

Le script ajoutera les colonnes suivantes :

- `Statut` : Oui / Non / Erreur
- `Score` : niveau de certitude (sur 100)
- `Date de vérification`
- `NEW Holding` : nom du nouveau propriétaire si différent (si score > 85)

Fichier généré
CarrefourVC_YYYY-MM-DD_HH-MM.xlsx

