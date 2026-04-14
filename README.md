# ml_project

Pipeline de traduction automatique français → anglais avec évaluation de la qualité des traductions.

## Description

Ce projet met en place un pipeline complet de traduction automatique basé sur le modèle HuggingFace Helsinki-NLP/opus-mt-fr-en. Il évalue la qualité des traductions produites à l'aide des métriques BLEU et chrF.

## Structure du projet

- src/loaders/ : Chargement des données (CSV, JSON)
- src/processors/ : Nettoyage et prétraitement
- src/translators/ : Traduction via HuggingFace
- src/evaluators/ : Calcul des métriques BLEU et chrF
- src/orchestrator/ : Coordination du pipeline complet
- data/ : Fichiers d'entrée
- output/ : Résultats produits
- tests/ : Tests unitaires pytest

## Installation

python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt

## Utilisation

cd src
python orchestrator/orchestrator.py

## Tests

pytest

## Formatage

black .

## Auteur

YanisTounsi

## Version Python

Compatible avec Python 3.10+