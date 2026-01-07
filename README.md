# JumeauRobotQuadripede
Ce projet s’inscrit dans un travail de groupe visant à concevoir et à générer des trajectoires pour un robot quadrupède. Mon rôle consistait à concevoir les trajectoires que le robot devait réaliser, ainsi qu’à les exporter dans un format exploitable par la personne responsable de l’implémentation du code embarqué sur le robot.

Cela m’a conduit à réaliser un jumeau numérique cinématique d’un robot quadrupède afin de concevoir ses trajectoires et de les optimiser à l’aide d’un algorithme génétique.

#### Aucune bibliothèque dédiée à la robotique n’a été utilisée.
### Objectifs :
- Réaliser un jumeau numérique cinématique du robot capable de générer des trajectoires quelconques
- Être capable d’évaluer les trajectoires
- Optimiser une trajectoire (via un algorithme génétique)
- Exporter une trajectoire sous deux formats :

1er format : une liste dont les colonnes sont
| x | y | z | BP |
où x, y et z représentent les positions du i-ème point de passage, et BP est un booléen indiquant si le point est en contact avec le sol.

2e format : une liste dont les colonnes sont
| t | q₁ | q₂ | q₃ | … | q₁₂ |
où q₁, …, q₁₂ correspondent aux angles des moteurs à l’instant t.

### Résultats

![til](./Resultat/traj.gif)
<legend>Simulation du robot suivant une trajectoire optimisée (itérations : 300)</legend>

![alt text](https://github.com/KLB-F/ProjetRobotique/blob/ffc319b9bc4cacaf6672e6c26e9feeabc2315b62/Resultats/%20EvolutionVitesseIteration.png)
<legend>Evolution de la vitesse moyenne du robot calculé issuent des 5 meilleurs trajectoirs à la i-ème itérations</legend>

#### En condition réel

Rotation de 360° : 3.5 s; 0° d'erreur
Sprint 3m : 25s; 10 cm d'erreur
