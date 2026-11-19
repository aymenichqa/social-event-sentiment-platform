# Document de César Cour (CDC) - Version 0.1

Plafond du projet : **Conception et développement d'une plateforme intelligente d'analyse des sentiments et de détection des tendances sur les réseaux sociaux lors d'événements sportifs de football.**

---

## 1. Intitulé du projet

Conception et développement d'une plateforme intelligente d'analyse des sentiments et de détection des tendances sur les réseaux sociaux lors d'événements sportifs de football.

## 2. Contexte et problématique

Les événements sportifs, particulièrement les matchs de football, génèrent une quantité importante de commentaires et de réactions sur les plateformes sociales.

Ces interactions contiennent des informations intéressantes pour les community managers, les journalistes sportifs, les créateurs de contenu et les organisations sportives.

Cependant, l'exploitation manuelle de ces données est difficile, particulièrement en présence de plusieurs langues, de dialectes, d'expressions informelles, d'Arabizi et de commentaires multilingues.

Le projet consiste à développer une plateforme capable de collecter, traiter et analyser automatiquement ces données afin d'extraire les opinions du public et d'identifier les sujets qui génèrent le plus d'engagement.

## 3. Objectif général

Concevoir et développer une plateforme de Social Listening spécialisée dans les événements de football, intégrant des techniques de Machine Learning, Deep Learning et NLP pour analyser les sentiments, identifier les sujets populaires et détecter les moments marquants des conversations sociales.

## 4. Objectifs spécifiques

- Collecter les commentaires provenant de sources sociales autorisées.
- Constituer et préparer des datasets multilingues.
- Développer un pipeline de nettoyage et de normalisation textuelle.
- Construire et évaluer des modèles de classification des sentiments.
- Prendre en charge le Darija marocain, l'Arabizi, l'arabe, le français, l'anglais et les commentaires mixtes.
- Extraire les mots-clés, expressions et sujets les plus fréquents.
- Détecter automatiquement les pics d'activité conversationnelle.
- Analyser les réactions du public autour des événements du match.
- Développer un dashboard interactif pour visualiser les résultats.

## 5. Utilisateurs cibles

- Community managers sportifs.
- Créateurs de contenu spécialisés dans le football.
- Journalistes et médias sportifs.
- Organisateurs d'événements sportifs.
- Responsables marketing et communication sportive.

## 6. Fonctionnalités attendues

### F1 – Gestion des événements sportifs

- Créer un événement.
- Définir les équipes, les joueurs et les mots-clés associés.
- Configurer les sources de données.
- Définir la période d'analyse.

### F2 – Collecte des données

- Récupérer les publications et commentaires accessibles via les API autorisées.
- Stocker les dates et les informations nécessaires à l'analyse.
- Éviter les doublons.
- Gérer les erreurs et les limites des API.

### F3 – Prétraitement des données

- Nettoyage des commentaires.
- Normalisation du texte.
- Gestion des emojis et caractères spéciaux.
- Gestion des différentes formes d'écriture du Darija.
- Identification des langues et des scripts.

### F4 – Analyse des sentiments

- Classification positive, négative et neutre.
- Affichage de la confiance du modèle.
- Comparaison des réactions entre équipes et joueurs.

### F5 – Extraction des sujets et mots-clés

- Identification des termes les plus mentionnés.
- Extraction des expressions fréquentes.
- Regroupement des commentaires par thématique.
- Analyse des sujets liés à l'arbitrage, aux joueurs, aux buts et aux décisions du match.

### F6 – Détection des moments marquants

- Analyse du volume de commentaires dans le temps.
- Détection des augmentations inhabituelles.
- Identification des sujets associés aux pics.
- Corrélation avec les événements du match lorsque leur chronologie est disponible.

### F7 – Dashboard analytique

- Nombre total de mentions collectées.
- Répartition des sentiments.
- Évolution des sentiments dans le temps.
- Classement des mots-clés et des sujets.
- Classement des joueurs et équipes les plus mentionnés.
- Visualisation des moments marquants.
- Filtres par événement, période, source et langue.

## 7. Contraintes techniques

- Respect des politiques et conditions d'utilisation des API.
- Disponibilité et qualité des datasets.
- Capacité de traitement des commentaires.
- Gestion des différentes langues et écritures.
- Limitation des ressources matérielles.
- Protection des données personnelles.

## 8. Périmètre du MVP

La première version doit intégrer :

- Un seul événement sportif à la fois.
- Une source de données réelle.
- Un système de collecte et de stockage.
- Un modèle de sentiment à trois classes.
- Une analyse des mots-clés et des sujets.
- Une détection élémentaire des pics de conversation.
- Un dashboard interactif.

Les autres plateformes, les émotions avancées et les fonctionnalités complexes seront considérées comme des extensions.

## 9. Livrables attendus

- Étude bibliographique sur le NLP et la sentiment analysis.
- Rapport d'analyse des datasets.
- Dataset préparé et documentation de son annotation.
- Modèles de Machine Learning et Deep Learning.
- Rapport d'évaluation des performances.
- Pipeline de collecte et de traitement.
- Application web et dashboard.
- Documentation technique.
- Rapport final du PFA et démonstration fonctionnelle.

## 10. Critères de réussite

- Collecte fonctionnelle depuis au moins une source autorisée.
- Traitement correct des différentes formes de texte ciblées.
- Évaluation reproductible du modèle sur des données indépendantes.
- Visualisation cohérente des résultats.
- Détection de pics de conversation avec identification des sujets associés.
- Exécution de bout en bout sur un événement de football.