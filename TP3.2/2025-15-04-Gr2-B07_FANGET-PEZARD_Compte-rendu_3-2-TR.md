---
title: Compte rendu de TP - Tour de refroidissement
author: Baptiste Fanget - Léo Pezard - Mécanique Energétique 3A
date: 15/04/2025
papersize: a4
lang: fr 
secnumdepth: 3
---

# Introduction

## Objectifs
Ce TP a pour objectif principal l’étude du fonctionnement d’une tour de refroidissement. Il s’agit de comprendre les phénomènes d’échange thermique et massique entre l’air et l’eau, et d’analyser l’influence de différents paramètres sur l’efficacité du refroidissement, comme le débit d’air, la charge thermique ou encore la vitesse d’écoulement.

## Contexte
Dans les installations industrielles, la gestion de la chaleur est un enjeu crucial. Les tours de refroidissement sont largement utilisées pour évacuer la chaleur excédentaire de manière économique et efficace. Ce TP s’inscrit dans ce cadre en proposant l’analyse d’un dispositif expérimental à échelle réduite, permettant de modéliser et de mieux comprendre le fonctionnement réel de ces systèmes.

## Notions clefs
- **Refroidissement par évaporation** : transfert de chaleur de l’eau vers l’air, par évaporation partielle de l’eau.
- **Bilans d’énergie et de masse** : permettent d’évaluer l’efficacité de la tour.
- **Air humide** : mélange air-vapeur dont les propriétés sont déterminées par la température sèche, la température de bulbe humide et l’humidité absolue.
- **Diagramme psychrométrique** : outil graphique essentiel pour caractériser les états thermodynamiques de l’air humide.

## Matériel utilisé

- **Banc expérimental de tour de refroidissement** miniature avec :
  - Un **circuit d’eau** : réservoir chauffant, pompe, garnissage, réservoir de récupération.
  - Un **circuit d’air** : ventilateur à débit réglable, dispositif de récupération de gouttelettes.
- **Instruments de mesure** :
  - Thermocouples (eau et air, en entrée et sortie)
  - Débitmètre pour l’eau
  - Manomètre à colonne d’eau (pour le débit d’air)
  - Résistance chauffante (pour simuler la charge thermique)
- **Outils d’analyse** :
  - Diagramme psychrométrique
  - Table de données expérimentales (en cas de mesures non fiables)


# Travail préliminaire

Avant de réaliser les manipulations expérimentales, un travail préliminaire a été effectué afin de mieux comprendre les propriétés de l’air humide, indispensable pour établir les bilans thermodynamiques de la tour de refroidissement.

## Propriétés de l’air humide

Les conditions atmosphériques de départ sont les suivantes :

- Pression atmosphérique : **1,013 bar** (soit 101300 Pa)
- Température sèche : **20°C**
- Température de bulbe humide : **14°C**
- Pression de vapeur saturante à 14°C : **1599 Pa** (issue des tables thermodynamiques)

À partir de ces données, plusieurs grandeurs caractéristiques ont été calculées :

**Pression partielle de vapeur d’eau (Pv)**

$P_v = P_{vs} - 6,666 \cdot 10^{-4} \cdot P_{atm} \cdot (\Theta - \Theta_h)$

Avec : 

- $P_v$ la pression partielle de l’eau dans l’air en mbar
- $P_{vs}$la pression de saturation de la vapeur d’eau à la température du bulbe humide $\Theta_h$ en mbar.
- $P_{atm}$ la pression totale de l’air (pression atmosphérique : 1013,25 mbar);
- $\Theta$ la température sèche de l’air en °C ;
- $\Theta_h$ la température du bulbe humide en °C.

Après calcul : $P_v = 1599 -6,666 \cdot 10^{-4} \cdot 101325 \cdot (20-14) \Rightarrow \boxed{P_v = 1193,84 \text{ Pa}}$


**Teneur en humidité (r)** calculée avec la relation $r= 0,622 \cdot \frac{P_v}{P_{atm}-P_v}$

On obtient donc $r = 7,418 \cdot 10^{-3} \text{kg}_{\text{vapeur}} \text{/} \text{kg}_{\text{air sec}}$


**Enthalpie spécifique de l’air humide (h)** 


Formule fournie dans le fascicule :  

$$h = \Theta + r \times (2490 + 1{,}96 \times \Theta)$$

Après calcul :  
$$h = 20 + 0{,}007418 \times (2490 + 1{,}96 \times 20)$$

On obtient :  
$$\boxed{h = 38{,}76 \ \text{kJ} / \text{kg}_{\text{air sec}}}$$


**Volume spécifique (v)** 

Formule du fascicule :  
$$v = 462 \times (0{,}622 + r) \times \frac{\Theta_K}{P_{\text{atmo}}}$$

Après calcul :  
$$v = 462 \times (0{,}622 + 0{,}007418) \times \frac{293{,}15}{101300}$$

On trouve ainsi :  
$$\boxed{v = 0{,}842 \ \text{m}^3 / \text{kg}_{\text{air sec}}}$$

Ces calculs permettent de mieux appréhender les échanges thermiques entre l’air et l’eau, notamment l’énergie transférée par évaporation.

## Utilisation du diagramme psychrométrique

En complément des calculs, le **diagramme psychrométrique** a été utilisé afin de vérifier la cohérence des résultats. Ce diagramme permet de :

- Repérer le point d’état de l’air à partir de la température sèche (20°C) et de la température de bulbe humide (14°C).
- Lire directement les valeurs d’enthalpie, d’humidité absolue et de volume spécifique.

Les valeurs obtenues par lecture graphique sont en très bon accord avec les calculs théoriques, avec un écart inférieur à **1%**, ce qui valide la méthode utilisée.

L’analyse de ces propriétés est essentielle pour le bon déroulement du TP, notamment lors de l’établissement des bilans d’énergie et de masse dans la suite de l’étude.



# Expériences


# Conclusion

