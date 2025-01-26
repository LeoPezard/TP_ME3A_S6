---
title : Compte rendu TP Mécanique Energétique - Rayonnement Thermique
author : Baptiste Fanget - Pezard Léo - ME3A
papersize: a4
lang: fr 
toc: true # table of contents
lof: true # list of figures
lot: true # list of tables
---

# Préambule

## Introduction

L'objectif de cette séance de travaux pratiques est d’explorer les mécanismes de
transfert thermique par rayonnement et d’étudier les paramètres influençant le
flux radiatif émis par une surface. Les variations du flux seront examinées en
fonction de la nature du matériau, de son état de surface, de sa température,
ainsi que de l'effet d’un écran en verre.

## Notions clés

Tout corps à une température $T>0K$ émet un rayonnement thermique, dû à la
conversion de son énergie interne en énergie électromagnétique. Ce rayonnement,
caractérisé par des longueurs d'onde de 1 à 100 ${\mu m}$ inclut les domaines
ultraviolet, visible et infrarouge. Contrairement à la conduction et à la
convection, le transfert radiatif ne nécessite pas de support matériel et se
propage en ligne droite.

Loi de Planck (puissance spectrale):
:   TODO : revoir l'unité de cette formule

   $$M_\lambda^0(T) = \frac{C_1 \lambda^{-5} }{ e^{C_2 / (\lambda T)} - 1 }$$

Où $C_{1} = 3,741.10^{8}W.m^{-2}.\mu m^{4}$ et $C_{2} = 14388 \mu m.K$

<!--
---
-->

Loi de Stefan-Boltzmann (flux total):
:  
   $$M^0(T) = \sigma T^4 \quad \text{avec} \quad \sigma = 5{,}67 \cdot 10^{-8}
   \, \text{W} \cdot \text{m}^{-2} \cdot \text{K}^{-4}$$

<!--
---
-->

Loi de Wien (longueur d'onde maximale):
:  

   $$\lambda_m T = 2898 \, \mu \text{m} \cdot \text{K}$$

<!--
--- 
-->

## Approche expérimentale 

Ce TP s'appuie sur les dispositifs suivants :

<!--
- __Cube multi-faces chauffé__ : avec des surfaces ayant des états différents (noire mate, blanche mate, aluminium poli et non poli) pour étudier l’influence de l’émissivité.
-->

Cube multi-faces chauffé: 
:   avec des surfaces ayant des états différents (noire mate, blanche mate,
aluminium poli et non poli) pour étudier l’influence de l’émissivité (voir
Figure \ref{fig:cube})

![Schéma du cube multi-faces aux quatre faces latérales différentes chauffées
par une ampoule centrale](dispositif.png){#fig:cube width=50%}

Lampe à filament de tungstène: 
:   permettant d’atteindre des températures élevées, avec T déduit de la résistance R via :


$$T = -0,053 \cdot \left(\frac{\rho_a R}{R_a}\right)^2 + 36.1 \cdot \left(\frac{\rho_a R}{R_a}\right) + 125$$

Thermopile: 
:   pour mesurer le flux radiatif net ${\Phi_{net}}$​ à partir de la tension générée:


$$U = s \cdot \Phi_\text{net} \quad \text{avec} \quad \Phi_\text{net} = \Phi_\text{émis} - \Phi_\text{absorbé}$$

Voir Figure \ref{fig:thermopile}

![Fonctionnement schématique de la thermopile](thermopile.png){#fig:thermopile}

---

### Objectif 

En combinant théorie et expérimentation, cette séance vise à :

Vérifier les lois fondamentales du rayonnement thermique.
Étudier l’influence des propriétés de surface et de la température sur le flux émis.
Analyser l’effet d’un écran en verre sur les échanges radiatifs.

Les résultats obtenus seront comparés aux modèles théoriques pour mieux comprendre les limitations expérimentales.

## Travail préparatoire

Réalisé sur AMeTICE

Notions principales abordées

# Expériences 

## Approche qualitative

L’objectif est ici de se familiariser avec la notion d’émetteur et de récepteur de rayonnement ainsi
que de dégager qualitativement des tendances de comportement de différentes surfaces.

### Sensibilisation au pouvoir émissif

En plaçant la main devant chaque face du cube, avec notre ressenti, nous avons
pu établir un classement du « pouvoir émissif ». (faire le classement de chaque
face du cube)

### Thermopile

La thermopile délivre des tensions différentes lorsqu'on la place devant des surfaces de températures différentes (étudier le signe de cette tension, évoquer la comparaison avec les sensations au dessus)

### Analyse


## Approche quantitative

------
|jvabkjbdakhbdf|
|----|
|vybfjyvbf|

: Légende du tableau - Description ou titre du tableau.