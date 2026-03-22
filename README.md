# Projet-IA
## Modélisation de la demande matériau liée à la demande en intelligence artificielle.

A l'heure où l'intelligence artificielle (IA) explose et devient la 4e grande révolution technologique, nous sommes constamment exposés au challenge énergétique qui en découle. Cependant, l'aspect matériel est quant à lui très peu souvent abordé. Cette étude a pour but de mettre le doigt sur les consommations en matériaux pour soutenir la demande de l'IA.



L'objectif est de modéliser la demande en matériaux nécessaires au bon fonctionnement de l'IA générative dans un futur proche. L'IA de référence est chatGPT 4 (autour de 17 500 milliards de paramètres). Il est important de noter que les résultats concernent uniquement les besoins matériaux pour le fonctionnement des unités GPU. Les composants d'infrastructure plus larges, tels que les réseaux, le stockage et les systèmes de refroidissement, ne sont pas pris en compte dans cette analyse.

La puce GPU étudiée est la NVIDIA A100, utilisé par OpenAI, Meta, Microsoft.
Le modèle ChatGPT 4 sera donc la référence dans les calculs, en faisant ensuite l'hypothèse que la consommation en matériaux des autres IA génératives est similaire.


Dans une première partie, nous verrons la modèlisation des besoins matériaux relatif à la demande en IA.
Dans une seconde partie, nous analyserons le résultat de l'analyse au vu des ressources actuelles en matériaux, tout en prenant en compte les facteurs géographiques, géopolitiques et commerciales.

Une grande partie des données de référence proviennent d'une source, qui est la suivante : [1] *From FLOPs to Footprints: The Resource Cost of Artificial Intelligence* ; Sophia Falk, Nicholas Kluge Correa, Sasha Luccioni, Lisa Biber-Freudenberger, and Aimee van Wynsberghe ; 3 Décembre 2025.

Nous avons fait le choix de commencer le modèle en partant des requêtes. Ces requêtes ne sont autres que des chaînes de caractères découpés en tokens. Ces tokens sont traités dans les data centers par des FLOPS (number of floating-point operations it can perform per second). Ainsi, il suffit de faire le lien entre requêtes et nombre de calculs associés (FLOPs) pour pouvoir remonter au nombre de GPUs nécessaires. Avec cette quantité, nous retrouvons la demande en matériaux associée.

