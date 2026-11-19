# social-event-sentiment-platform

Plateforme d'analyse des sentiments et de détection de tendances sur les réseaux sociaux pour les événements sportifs de football.

## Présentation

Ce projet vise à concevoir et développer une plateforme de **Social Listening** spécialisée dans les événements de football.

Elle collecte, traite et analyse automatiquement les commentaires et publications des réseaux sociaux afin d'extraire les opinions du public, d'identifier les sujets les plus engagés et de détecter les moments marquants des conversations.

Les commentaires proviennent de multiples langues et écritures : **arabe, Darija marocaine, Arabizi, français, anglais et commentaires mixtes**.

## Objectifs

- Collecter les données depuis des sources sociales autorisées.
- Préparer et annoter des datasets multilingues.
- Nettoyer et normaliser le texte (gestion des emojis, Arabizi, dialectes).
- Construire et évaluer des modèles de classification des sentiments (3 classes : positif, négatif, neutre).
- Extraire les mots-clés et les sujets les plus fréquents.
- Détecter les pics d'activité conversationnelle et les corréler aux événements du match.
- Visualiser les résultats dans un dashboard interactif.

## Architecture du projet

```
src/social_sentiment/
  ingestion/       # Collecte et stockage des données
  preprocessing/   # Nettoyage et normalisation du texte
  nlp/             # Modèles NLP : sentiment, mots-clés, détection de langue
  evaluation/      # Évaluation des modèles et rapports
  streaming/       # Lecture des flux de données
  alerts/          # Détection de pics et notifications

data/
  raw/         # Données brutes collectées
  interim/     # Données intermédiaires (nettoyées)
  processed/   # Données prêtes pour l'entraînement

docs/          # Documentation du projet
frontend/      # Interface web et dashboard
scripts/       # Scripts utilitaires
notebooks/     # Analyses exploratoires et prototypes
reports/       # Rapports d'évaluation et résultats
```

## Installation

```bash
python -m venv .venv
.venv/Scripts/activate
pip install -r requirements.txt
```

## Modes de travail

- **Squelette du projet** : cette version contient la structure de base et les points d'entrée.
- **Étape suivante** : implémentation progressive des modules (ingestion, preprocessing, nlp, evaluation, streaming, alerts).
- **Dashboard** : interface web interactive construite avec les résultats du pipeline.

## Contenu de ce dépôt

- `README.md` : ce document.
- `docs/CDC_v0.1.md` : cahier des charges de base du projet.
- `requirements.txt` : dépendances Python.
- `.gitignore` : fichiers à ignorer (données brutes, fichiers de cache, variables d'environnement).
- `src/social_sentiment/` : code source Python du pipeline.
- `data/`, `reports/`, `notebooks/`, `scripts/`, `frontend/` : fichiers générés ou à créer.

## Licence

Projet académique (PFA) - À adapter selon les besoins de l'établissement.
