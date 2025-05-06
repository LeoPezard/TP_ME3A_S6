---
papersize: a4
lang: fr 
secnumdepth: 3
---


# Introduction

Ce TP vise à étudier les phénomènes acoustiques à travers des expériences concrètes de mesure, d’analyse et de modélisation du son, en lien avec les notions physiques et numériques abordées en cours.

## Contexte et Objectif

L'acoustique joue un rôle essentiel dans de nombreux domaines, notamment l’ingénierie du son, l’architecture, les télécommunications et le traitement du signal.  
Dans ce contexte, ce TP a pour objectif :

- De comprendre les bases de la propagation des ondes sonores dans différents milieux,
- De mesurer et analyser des signaux acoustiques à l’aide de capteurs et d’outils numériques,
- De modéliser des phénomènes comme la réverbération, les interférences ou l’effet Doppler,
- De mettre en œuvre un protocole expérimental pour valider des hypothèses acoustiques.

## Notions Clefs

- **Onde sonore** : vibration mécanique se propageant dans un milieu (air, solide, liquide) sous forme de variation de pression.
- **Fréquence** : nombre d’oscillations d’une onde par seconde, mesurée en hertz (Hz), perçue comme la hauteur d’un son.
- **Spectre** : représentation fréquentielle d’un signal, utilisée pour analyser les composantes harmoniques d’un son.
- **Réverbération** : persistance d’un son dans un espace fermé due aux réflexions successives sur les parois.
- **Effet Doppler** : variation apparente de la fréquence d’une onde sonore perçue par un observateur en mouvement relatif par rapport à la source.

## Dispositif Expérimental

Le dispositif expérimental mis en place pour ce TP d'acoustique comprend les éléments suivants :

- **Source sonore** : un haut-parleur émettant des signaux sinusoïdaux ou complexes à différentes fréquences.
- **Capteurs** : microphones calibrés permettant de capter les ondes sonores avec précision.
- **Carte d’acquisition** : interface permettant de numériser les signaux analogiques enregistrés par les microphones.
- **Logiciel d’analyse** : utilisé pour visualiser les formes d’ondes, effectuer des transformées de Fourier, et extraire des caractéristiques comme la fréquence fondamentale ou les harmoniques.
- **Environnement contrôlé** : expérience réalisée dans une enceinte réduisant les interférences extérieures.

L’ensemble du montage permet de générer, capter, et analyser les ondes sonores afin d’en étudier les propriétés physiques et spectrales.



# Expériences

## Mesure de la vitesse du son dans l'air

Le montage réalisé est composé d'un générateur 40kHz, d'un émetteur et récepteur (transducteurs ultrasonores) et enfin d'un oscilloscope pour visualiser les signaux d'émission et de réception. 

L'oscilloscope est réglé ........ pour distinguer correctement les deux signaux. 

Ainsi on peut observer l'évolution du signal d'émission en fonction de la distance d : TODO : Commmenter

TODO : Faire un graphe de delta t en fonction de d et/ou un tableau des valeurs (Mettre le premier curseur au moment où la pulsation est émise et mettre le deuxième lorsqu'elle est reçue)

On observe une (courbe affine???), le coefficent directeur de cette droite permet de calculer la vitesse expérimentale du son dans l'air. TODO : Calcul
On note ici que la température de la pièce est de .... °C

On sait que la vitesse du son dans l'air pour une température de 20°C est de 340 m/s.

Erreur relative : TODO : Calcul
Cette erreur peut provenir de la température de la pièce qui n'est pas forcément à 20°C mais également de l'interprétation graphique de delta t en fonction de la distance.

### Echantillon intercalé entre l'émetteur et le récepteur



## Niveaux acoustiques, atténuation, traitement du signal


# Conclusion

