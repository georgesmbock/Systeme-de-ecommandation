# Projet Personnel: Système de Recommandation avec Word2Vec

## Description
Ce projet implémente un système de recommandation basé sur Word2Vec. Il suggère des articles similaires en fonction d’un article donné, en utilisant des représentations vectorielles des mots.

## Fonctionnalités
- Génération de recommandations basées sur la sémantique.
- Utilisation de Word2Vec pour capturer les relations entre les mots.
- Score de similarité basé sur la similarité cosinus.
- Facilement adaptable à différents types de documents (articles, avis, descriptions de produits…).

## Technologies utilisées
Python 3.x

Gensim (Word2Vec)

Scikit-learn
 - Installation et exécution

## Installer les dépendances
`pip install gensim scikit-learn`

## Définir le corpus d’articles
variable articles 
`
articles = [
    ["machine", "learning", "intelligence", "artificielle"],
    ["réseaux", "neurones", "deep", "learning"],
    ["traitement", "langage", "naturel", "NLP"],
    ["voitures", "autonomes", "apprentissage", "automatique"]
]
`

## Choisir un article pour lequel générer des recommandations
Par exemple, pour recommander des articles similaires à "NLP" :
`recommend(2)`

## Lancer le script
`python recommendation_system.py`

## Exemple de sortie
Articles similaires à : traitement langage naturel NLP
- machine learning intelligence artificielle (Score : 0.82)
- réseaux neurones deep learning (Score : 0.78)
(Les articles suggérés sont pertinents grâce à Word2Vec ! )

## Améliorations possibles
- Vaste ensemble de données
- Remplacer Word2Vec par FastText pour mieux gérer les mots rares.
- Intégrer un modèle BERT pour une meilleure compréhension du contexte.
- Ajouter une interface Web avec Flask ou Streamlit.

