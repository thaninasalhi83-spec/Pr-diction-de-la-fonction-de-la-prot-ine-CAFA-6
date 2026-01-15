# Prédiction de la fonction de la protéine CAFA-6
Ce projet vise à prédire la fonction des protéines à partir de leurs séquences d’acides aminés en utilisant des techniques d’apprentissage automatique.  L’objectif est de développer un modèle capable de déterminer automatiquement le rôle biologique des protéines.Le jeu de données contient des séquences de protéines basées sur l’ontologie génétique.
## Données

- Séquences de protéines fournies au format FASTA  
- Utilisation uniquement de l’aspect fonction moléculaire  
- Conservation des 100 termes GO les plus fréquents 

## Prétraitement

- Lecture et nettoyage des séquences  
- Suppression des caractères non valides  
- Conservation des 20 acides aminés standards  
- Suppression des protéines sans séquence valide  
- Filtrage des annotations GO  
## Caractéristiques utilisées

Pour chaque protéine :
- Fréquence des 20 acides aminés  
- Longueur de la séquence  

Cela donne 21 caractéristiques par protéine.

## Modèles utilisés

Deux modèles ont été testés :
- Régression logistique  
- Forêt aléatoire  

## Évaluation

Les modèles sont évalués avec :
- F1 micro  
- F1 macro  
- Précision micro  
- Rappel micro  


## Visualisation des résultats

- Projection 2D des protéines avec l’ACP  
- Matrice de confusion pour un terme GO  
- Courbe ROC pour la régression logistique  
- Graphique de comparaison des modèles 