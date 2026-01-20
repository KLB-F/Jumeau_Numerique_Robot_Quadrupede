# Jumeau numérique cinématique d'un robot quadrupéde
Ce projet s’inscrit dans un travail de groupe visant à concevoir et commander un robot quadrupéde. Mon rôle consistait à concevoir les trajectoires que le robot devait réaliser, ainsi qu’à les exporter dans un format exploitable par la personne responsable de l’implémentation du code embarqué sur le robot.

Cela m’a conduit à réaliser un jumeau numérique cinématique d’un robot quadrupède afin de concevoir ses trajectoires et de les optimiser à l’aide d’un algorithme génétique.

#### Aucune bibliothèque dédiée à la robotique n’a été utilisée.
De plus, bien que le projet soit en groupe, le travail ici présent à été effectué seul.

#### Davantage de détails et de précision sont dans le [rapport](Rapport.pdf)

## Objectifs :
- Réaliser un jumeau numérique cinématique du robot capable de suivre des trajectoires quelconques
- Être capable d’évaluer les trajectoires selon leurs vitesse et stabilités
- Optimiser une trajectoire (via un algorithme génétique)
- Exporter une trajectoire sous deux formats .csv :
  - 1er format - Sauvegarde de la trajectoire pour réutilisation ultérieur par le programme
  - 2eme format - Exportation pour implémentation hardware

## Fonctionnalités principals :

Simulation de trajectoire :
- Simulation cinématique dans le domaine temporelle et spatiale
- Gestion de la synchronicité des pattes
- Possibilité d'enregistrer / de charger des trajectoires
- Exportation possible pour l'implémentation hardware
- Possibilité d'afficher la trajectoire par le biais d'un gif
- Grande variété de trajectoire crées possible

Evaluation et optimisation de trajectoire :
- Evaluation de la stabilité
- Evaluation de la vitesse
- Détection des trajectoire non valide
- Optimisation des trajectoire via algorithme génétique

## Utilisation

## Résultats :

Voici une présentation des résultats pour la trajectoire en rotation. On part d'abord d'une trajectoire initiale (Figure 1), avant d'appliqué l'algorithme d'optimisation de la trajectoire. L'on obtient alors une trajectoire optimisée (Figure 3) ainsi que l'évolution de la vitesse de roation en fonction des générations (Figure 2). Enfin, l'on peut maintenant exporter la trajectoire pour l'implémenter sur le robot et observé le résultat (Vidéo 1).

> Figure 1

![Figure_1](./Resultat/traj.gif)

> Figure 2

![Figure_2](./Resultat/_EvolutionVitesseIteration.png)

> Figure 3

## Limites : 



![Figure_3](./Resultat/traj_opti.gif)

> Video 1

[![Video_1](./Resultat/Preview_video.png)](./Resultat/video_rotation.mp4)
