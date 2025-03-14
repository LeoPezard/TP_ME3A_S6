---
title : Compte rendu de TP - Rayonnement Thermique
author : Baptiste Fanget - Pezard Léo - Mécanique Energétique 3A
date : 28/01/2025
papersize: a4
lang: fr 
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
:   

   $$M_\lambda^0(T) = \frac{C_1 \lambda^{-5} }{ e^{C_2 / (\lambda T)} - 1 }$$

Où $C_{1} = 3,741.10^{8}W.m^{-2}.\mu m^{4}$ et $C_{2} = 14388 \mu m.K$


Loi de Stefan-Boltzmann (flux total):
:  
   $$M^0(T) = \sigma T^4 \quad \text{avec} \quad \sigma = 5{,}67 \cdot 10^{-8}
   \, \text{W} \cdot \text{m}^{-2} \cdot \text{K}^{-4}$$

Cette loi correspond à l'intégrale de la fonciton de Planck sur tout le spectre mais également au flux émis par $1m^{2}$ de corps noir dans toutes les directions pour toutes les longueurs d'onde.


Loi de Wien (longueur d'onde maximale):
:  

   $$\lambda_m T = 2898 \, \mu \text{m} \cdot \text{K}$$


## Approche expérimentale 

Ce TP s'appuie sur les dispositifs suivants :

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
:   pour mesurer le flux radiatif net ${\Phi_{net}}$​ à partir de la tension générée (Voir Figure \ref{fig:thermopile}):

$$U = s \cdot \Phi_\text{net} \quad \text{avec} \quad \Phi_\text{net} = \Phi_\text{émis} - \Phi_\text{absorbé}$$



![Fonctionnement schématique de la thermopile](thermopile.png){#fig:thermopile width=70%}

\


## Objectif 

En combinant théorie et expérimentation, cette séance vise à :

Vérifier les lois fondamentales du rayonnement thermique.
Étudier l’influence des propriétés de surface et de la température sur le flux émis.
Analyser l’effet d’un écran en verre sur les échanges radiatifs.

Les résultats obtenus seront comparés aux modèles théoriques pour mieux comprendre les limitations expérimentales.

## Travail préparatoire

Réalisé sur AMeTICE

Notions principales abordées : 

- En rayonnement, un rayon monochromatique signifie un rayon d'une seule longueur d'onde
- Un flux absorbé par une surface à tendance à réchauffer la surface
- Un flux émis par une surface à tendance à refroidir la surface
- Un flux transmis ou réfléchi par une surface ne modifie pas la température
- Le flux partant ${\phi^{partant}}$ d'une surface opaque S d'émissivité $\epsilon$ à température T faisant face à une surface environnante assimilée au corps noir à température $T_{a}$ s'exprime par :
 $${\phi^{partant}} = \epsilon \cdot \sigma \cdot T^{4} + (1+\epsilon) \cdot \sigma \cdot {T_{a}}^{4}$$

- Un flux émis par un expérimentateur peut se réfléchir sur le cube vers la thermopile


# Expériences 

## Approche qualitative

L’objectif est ici de se familiariser avec la notion d’émetteur et de récepteur de rayonnement ainsi
que de dégager qualitativement des tendances de comportement de différentes surfaces.

### Sensibilisation au pouvoir émissif

En plaçant la main devant chaque face du cube, avec notre ressenti, nous avons
pu établir un classement du « pouvoir émissif ».


| Face noire | Face blanche | Face polie | Face non polie |
|:------------:|:---------------:|:---------------:|:-----------------:|
| Semble être la plus chaude de toutes les faces | Semble être la deuxième la plus chaude    | Semble être la face la moins chaude     | Est légèrement plus chaude que la face polie mais moins chaude que la face blanche   |


:Sensibilisation au pouvoir émissif - Ressenti à l'approche de chaque face du cube.

Le classement des faces en fonction de leur pouvoir émissif par ordre décroissant est donc : Face noire, face blanche, face non polie puis face polie.

Un pouvoir émissif élevé signifie que le flux de chaleur passe à travers la surface, il est donc peu absorbé par celle-ci, donc la chaleur est ressentie à l'extérieur du cube.

### Thermopile

La thermopile délivre des tensions différentes lorsqu'on la place devant des surfaces de températures différentes.

Etude du signe de la tension de la thermopile :

- Cas T = $T_{a}$, la tension mesurée est de 0 mV
- Cas T < $T_{a}$ (température extérieure) : tension mesurée -1,4 mV
- Cas T < $T_{a}$ (température du frigo) : tension mesurée -2.0 mV
- Cas T > $T_{a}$ (température corporelle), la tension mesurée est de 0,7 mV

Plage du spectre mesuré : 0,5 à  40 $\mu m$.

On remarque que lorsque la température est inférieure à la température ambiante, la tension mesurée par la thermopile est négative.


### Analyse

La thermopile est disposée face à une face du cube $T_{a}$, puis cette face est éclairée avec un flux issu de la face noir d'un autre cube à $T \approx$ 50 °C.

Il est possible d'en déduire un classement des surfaces en terme de « pouvoir réfléchissant » de chaque face du cube à $T_{a}$ :


| | Face noire | Face blanche | Face non polie | Face polie | 
|:--------:|:-------------:|:-----------------:|:-----------------:|:-----------------:|
| Tension mesurée (mV) | 0   |   0  |   0,8  |  1,2   |


:Sensibilisation au pouvoir réfléchissant - Mesure de tension à l'approche de chaque face du cube.

Le classement des faces en fonction de leur pouvoir réfléchissant par ordre croissant est donc : Face noire, face blanche, face non polie puis face polie.

Un pouvoir réfléchissant élevé signifie que le flux de chaleur ne passe pas à travers la surface, il est donc réfléchi par celle-ci, ainsi la chaleur est renvoyée sur la thermopile.

La loi du rayonnement thermique constatée est la loi de Kirchhoff exprimée par $\epsilon = 1 - \rho$ où $\epsilon$ est l'émissivité et $\rho$ est la réflectivité. (ici transmittivité $\tau = 0$ ).


## Approche quantitative

### Influence de la nature de la surface et de sa température

Détail de chaque composante de l'équation (15):
 

$$U(V) = s [\phi^{incident}_{capteur} - \phi^{partant}_{capteur}] = -s \phi^{net}_{capteur} = s [\phi^{absorbé}_{capteur} - \phi^{émis}_{capteur}] = U(V)$$



- $U(V)$ ici représente la tension mesurée par la thermopile. Cette tension est directement proportionnelle à la différence entre le flux incident $\phi^{incident}_{capteur}$​ et le flux partant $\phi^{partant}_{capteur}$ sur la face avant du capteur.
L'équation montre que U(V) est également lié au flux net ($\phi^{net}_{capteur}$​).

- $\phi^{incident}_{capteur}$ correspond au flux incident, c'est-à-dire le rayonnement thermique qui arrive sur la face avant du capteur.
Ce flux dépend de la température $T_{objet}$​ de l'objet observé, ainsi que de son émissivité ($\epsilon_{objet}$​) et du facteur de forme ($F_{capteur \rightarrow objet}$​) entre le capteur et l'objet (ici supposé à 1).

- $\phi^{partant}_{capteur}$ représente le flux partant, c'est-à-dire le rayonnement thermique émis par la face avant du capteur en direction de l'objet.
Le flux partant est constant si la température de la face avant du capteur ($T_{capteur}$​) reste proche de la température ambiante ($T_{a}$​), ce qui est le cas grâce à la faible résistance thermique de l'élément sensible (fine feuille de métal noircie).

- $\phi^{net}_{capteur}$ Le flux net est défini comme la différence entre le flux incident ($\phi^{incident}_{capteur}$​) et le flux partant ($\phi^{partant}_{capteur}$​).
Il représente le bilan global de rayonnement thermique sur le capteur, qui est à l'origine de la tension mesurée U(V).

- $\phi^{absorbé}_{capteur}$ correspond au flux thermique effectivement absorbé par la face avant du capteur.
Ce flux dépend des propriétés optiques du capteur, notamment de son émissivité ($\epsilon_{capteur}$​), et de l'énergie apportée par le rayonnement incident.

- $\phi^{émis}_{capteur}$ représente le flux thermique émis par la face avant du capteur en raison de sa propre température $T_{capteur}$.
Ce flux reste constant si $T_{capteur}$​ s'élève peu et reste proche de $T_{a}$​ (température ambiante).

- $s$ est la sensibilité du capteur, exprimée en mV/mW. Elle quantifie la relation entre la variation de flux thermique (en milliwatts) et la tension mesurée (en millivolts).

\

Pour démontrer l'équation (16), nous partons de $U(V) = s [\phi^{absorbé}_{capteur} - \phi^{émis}_{capteur}]$

$\phi^{émis}_{capteur} = \sigma \cdot \epsilon \cdot T^{4}_{a}$, or pour un corps noir, $\epsilon = 1$, donc $\phi^{émis}_{capteur} = \sigma \cdot T^{4}_{a}$

Il faut déterminer $\phi^{absorbé}_{capteur} = \phi^{émis}_{cube} = \phi^{réfléchi}_{cube}$, avec $\phi^{émis}_{cube} = \epsilon_{cube} \cdot \sigma \cdot T^{4}$ 

Avec : $\phi^{réfléchi}_{cube} = (1-\epsilon_{cube}) \cdot (\sigma - T^{4}_{cube})$

Donc $U(V) = s \cdot [\epsilon_{cube} \cdot \sigma T^{4}_{cube}] + (1- \epsilon) \cdot \sigma T^{4}_{cube} - \sigma \cdot T^{4}_{a}$

Finalement :
 $$U(V) = \sigma \cdot \epsilon_{cube} \cdot s \cdot(T^{4}_{cube} - T^{4}_{a})$$

Avec $\epsilon_{cube}$ l'émissivité du cube et s la sensibilité du capteur.

Graphe de U(V) en fonction de $\sigma \cdot [T^{4} - T^{4}_{a}]$ :

![Tension mesurée en fonction des différences de température pour chaque face du cube](graphe1.png){#fig:graphe1}

Les tensions calculées par la thermopile ont été mesurées sur chaque face par palier de 10 degrés (de 20 à 100 degrés). Ces mesures ont donc permis d'établir la relation entre la tension mesurée et l'émissivité, notamment grâce à la formule démontrée auparavant :
$$U(V) = \sigma \cdot \epsilon_{cube} \cdot s \cdot(T^{4}_{cube} - T^{4}_{a})$$
Les pentes nous permettent donc de calculer l'émissivité de chaque face, il est donc intéréssant de comparer les pentes entre elles afin de déterminer l'émissivité de chaque surface du cube.

Les relations sont données, pour chaque face par U(V) = $\sigma \cdot \epsilon_{face_{cube}} \cdot s \cdot(T^{4}_{cube} - T^{4}_{a})$

Donc $Rapport_{pente} = \frac{\epsilon_{face_{1}}}{\epsilon_{face_{2}}}$

Sachant que $\epsilon_{noire_{0.4 - 40 \mu m}} = 0,94$, il est possible de déterminer $\epsilon_{blanc}$ grâce à :

$\epsilon_{blanc_{0.4 - 40 \mu m}} \, = \frac{epsilon_{noire}}{rapport_{pente}}$ Donc $\epsilon_{blanc_{0.4 - 40 \mu m}} \, = \frac{0,94}{\frac{2.04766}{2.02426}} \approx 0.92$

De même avec la face polie et non polie :

$\epsilon_{polie_{0.4 - 40 \mu m}} \, = \frac{epsilon_{noire}}{rapport_{pente}}$ Donc $\epsilon_{polie_{0.4 - 40 \mu m}} \, = \frac{0,94}{\frac{2.04766}{0.111334}} \approx 0.05$

$\epsilon_{non polie_{0.4 - 40 \mu m}} \, = \frac{epsilon_{noire}}{rapport_{pente}}$ Donc $\epsilon_{non polie_{0.4 - 40 \mu m}} \, = \frac{0,94}{\frac{2.04766}{0.205029}} \approx 0.1$

Il est possible de remarquer que entre les faces de couleur (noire et blanche) et la face polie, le rapport des émissivités est d'environ 19.

Cet ordre d'émissivité correspond avec nos ressentis de début de TP. (Voir tableau 1). L'émissivité de la face noire est supérieure aux autres, suivi de la face blanche, de la face non polie puis, de la face polie, possédant l'émissivité la plus faible.

Voici le graphe complété de la réflectivité en fonction de la longueur d'onde pour la peinture blanche et la peinture noire :

![Réflectivité en fonction de la longueur d'onde](graphe2.png){#fig:graphe2}

Il est possible de remarquer que la réflectivité de la peinture blanche est élevée dans le domaine du visible, contrairement à la peinture noire. Cela explique pourquoi des couleurs sombres tiennent chaud en été, car elles ne reflètent pas la chaleur, donc l'absorbent, contrairement au blanc.

On remarque une similitude entre les deux courbes dans l'infrarouge, car les deux couleurs ne permettent pas une réflectivité dans ce domaine de longueur d'onde.
\

### Transmission du rayonnement

Lors de l'expérience précédente, nous avons pu remarquer que la tension mesurée par la thermopile était nulle lorsque une plaque de verre était placée entre la face noire et la thermopile.

Nous pouvons en déduire que le verre à une transmittivité nulle car nous sommes dans l'infrarouge.

_Transmissivité dans le visible :_
Le verre est transparent dans le visible $\lambda \approx 0.4 \, \text{à} \, 0.7 \mu m$, donc la transmissivité $\tau$ est proche de 1 dans cette plage.

_Transmissivité dans l’infrarouge :_
Le verre est opaque aux longueurs d’onde infrarouges $\lambda \geq 0.7 \mu m$, donc $\tau$ chute brutalement vers 0. Cela explique l’effet de serre, car les rayonnements infrarouges émis par les objets chauffés ne traversent pas le verre.

Graphique complété :

![Transmissivité du verre en fonction de la longueur d'onde](graphe3.png){#fig:graphe3 width=50%}

Dans le visible : $\tau \approx 1$ (ligne horizontale haute). Dans l’infrarouge : $\tau \approx 0$ (ligne horizontale basse après le visible).

\

__Application : __

Dans une voiture avec pare-brise, le tableau de bord chauffe davantage à cause de l’effet de serre :

- Flux solaire ($\Phi_{solaire}$​) : Le rayonnement visible traverse le pare-brise et est absorbé par le tableau de bord noir.
- Émission infrarouge ($\Phi_{IR}$​) : Le tableau de bord réémet de l’énergie en infrarouge, mais le pare-brise bloque ce rayonnement, le piégeant dans l’habitacle.
- Isolation thermique : Le pare-brise limite les pertes par convection et conduction, augmentant encore la température.

__$\rightarrow$__ Sans pare-brise, les flux infrarouges s’échapperaient et le tableau de bord serait moins chaud.

Voir Figure \ref{fig:voiture}


- 1) Flux émis par le soleil $\Phi_{solaire}$
- 2) Flux réfléchi par le pare brise $\phi^{reflechi}_{pare-brise} = \phi^{transmis}_{pare-brise} - \Phi_{solaire}$ 
- 3) Flux transmis par le pare brise $\phi^{transmis}_{pare-brise}$
- 4) Flux absorbé par le tableau de bord
- 5) Flux réfléchi par le tableau de bord (infrarouge)
- 6) Flux réfléchi par le pare-brise venant du tableau de bord.

![Schéma de l'effet de serre dans une voiture](voiture.png){#fig:voiture}

\

# Conclusion

Ce TP nous a permis d’approfondir notre compréhension du rayonnement thermique 
et des principes qui influencent ce comportement. Grâce aux différentes expériences, nous 
avons pu mettre l'accent sur l’influence de la nature et de l’état de surface 
des matériaux sur l’émissivité et la réflectivité. Les résultats obtenus, 
notamment les valeurs d’émissivité des différentes faces du cube, sont 
cohérents avec les modèles théoriques et nos observations qualitatives.

L’expérience sur la transmission du rayonnement a également illustré 
concrètement le phénomène de l’effet de serre, en mettant en évidence 
l’opacité du verre aux infrarouges. Ce TP nous a donc permis de relier 
théorie et pratique tout en nous sensibilisant aux limites des mesures 
expérimentales et aux erreurs potentielles.