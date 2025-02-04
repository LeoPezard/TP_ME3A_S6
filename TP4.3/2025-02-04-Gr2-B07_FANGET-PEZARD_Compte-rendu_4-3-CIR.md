---
title : Compte rendu de TP - Caméra Infrarouge
author : Baptiste Fanget - Pezard Léo - Mécanique Energétique 3A
date : 04/02/2025
papersize : a4
lang : fr 
secnumdepth : 3
---

# Préambule

## Introduction

L’imagerie infrarouge est un outil essentiel permettant d'observer la chaleur émise par des objets, bien au-delà de ce que l’œil humain peut percevoir. Grâce à une caméra infrarouge, il est ainsi possible de repérer et étudier les changements de température d’une scène, avec des applications variées allant de l’industrie à la recherche scientifique, en passant par la thermographie des bâtiments.

Ce TP a pour but de nous familiariser avec le fonctionnement de la caméra infrarouge et de comprendre comment elle capte et traduit le rayonnement thermique en images exploitables. À travers différentes expériences, nous observerons l’influence de l’émissivité et de la température sur les images obtenues. En utilisant des sources radiatives comme un corps noir ou des surfaces aux propriétés thermiques variées, nous verrons comment interpréter correctement ces images et ce qu’elles nous apprennent sur les objets observés.

## Matériel utilisé

### Station d'imagerie et de mesure infrarouge

La chaîne de visualisation et d’acquisition d’images infrarouges comprend tout d’abord la caméra
infrarouge (modèle A40 fabriquée par FLIR) à matrice dans le plan focal de l’objectif (FPA :
Focal Plane Array) dont la surface sensible est constituée d’une matrice de 320 x 240 détecteurs
microbolométriques (voir la photo en Figure \ref{fig:camera}).

![Photo de la caméra infrarouge utilisée](camera.png){#fig:camera}

Cette chaîne est schématisée sur la Figure \ref{fig:scene}. L’objectif (ou optique sur le schéma) est constitué
de lentilles en Germanium (transparent dans l’infrarouge, traité antireflet). La matrice de microbo
lomètres, placée après l’objectif, reçoit le flux radiatif venant d’une surface de la scène thermique
correspondant à la surface conjuguée de la matrice à travers l’objectif de la caméra (voir Figure \ref{fig:scene}).

![Schéma de la scène thermique vers la matrice de détecteurs puis vers l'image infrarouge](scene.png){#fig:scene}

Chaque détecteur de la matrice est sensible dans la gamme 7,5-13 $\mu m$. Il faut noter que à température ambiante (environ 20-25°C), la majorité des rayonnements thermiques des objets est émise dans cette plage de 7 à 13 $\mu m$. Cela permet à la caméra de capter le maximum d'énergie thermique des objets sans être trop influencée par d'autres sources de rayonnement, comme la lumière visible ou l'infrarouge proche.

Ces détecteurs sont des microbolomètres, de la famille des détecteurs thermiques, dont le principe est
basé sur l’échauffement du détecteur consécutif à l’absorption du flux infrarouge pendant une durée
donnée, appelée « temps d’intégration ». Cet échauffement du détecteur induit une variation de sa ré
sistance électrique dont la mesure est alors proportionnelle au flux infrarouge absorbé. Les tensions
délivrées, alors, par tous les détecteurs de la matrice sont lues puis numérisées et transmis à l'ordinateur.

### Sources radiatives

#### Corps noir
\

La source radiative de référence (ou « référence thermorayonnante ») utilisée est un corps noir de
laboratoire (Figure \ref{fig:corps_noir}).

Il s’agit d’une cavité cylindrique à fond conique, revêtue d’un
matériau très absorbant, à facteur de forme élevé (profondeur > diamètre), chauffée de façon isotherme
par des résistances électriques. Il est équipé d’un disque percé de diaphragmes de tailles différentes
qui peuvent se placer devant l’entrée de la cavité. La gamme de température qu’il peut couvrir va
de l’ambiante à 1000 degrés, elle est mesurée par une sonde platine en fond de cavité. L’image que l’on a
en observant un tel corps noir placé par exemple à 100 degrés dans un environnement à 20 degrés est donc
un disque (« fort » flux quittant la cavité) se détachant de son environnement.

![Corps noir de laboratoire](corps_noir.png){#fig:corps_noir}

#### Cube de Leslie
\

Ce cube (Voir Figure \ref{fig:cube}) présente 4 facettes latérales en aluminium chauffées par une ampoule de 100W placée au centre. La temérature de chaque face peut être supposée uniforme. Les quatre faces présentent un état de surface différent : peinture noire, peinture blanche, aluminium non poli, aluminium poli.

Lors du TP précédent, nous avons pu faire un classement des émissivités de chaque face:


| Face | Émissivité ($\epsilon_{0.4 - 40 \mu m}$) |
|:----------------:|:-----------:|
| Noire                | 0.94|
| Blanche              | 0.92|
| Polie                | 0.05|
| Non polie            | 0.1 |

:Émissivités de chaque face calculées lors du TP précédent.


Nous avions également pu réaliser un classement des faces en fonction de leur pouvoir réfléchissant, par ordre croissant : Face noire, face blanche, face non polie puis face polie.

La réflexion de rayonnement par la face en aluminium poli est de type spéculaire (rayons concentrés dans 1 seule direction), alors que pour les autres faces, elle pourra être considérée diffuse (rayonnement réparti sur une plus grande surface).

Un pouvoir réfléchissant élevé signifie que le flux de chaleur ne passe pas à travers la surface, il est donc réfléchi par celle-ci, ainsi la chaleur est renvoyée sur la thermopile.

![Cube de Leslie](cube.png){#fig:cube}


#### Plaque chauffante à différentes émissivités

Il s’agit d’une plaque en cuivre régulée en température dont la surface est peinte en noir. Locale
ment, comme vous pouvez l’observer sur la Figure \ref{fig:plaque}, l’émissivité de la surface a été modifiée par
l’ajout d’adhésifs en aluminium (de gauche à droite : adhésif seul, adhésif + scotch blanc, adhésif +
vernis). 

La visualisation de cette plaque par la caméra infrarouge permettra donc de s’intéresser aux
conséquences de l’émissivité d’une surface sur son image infrarouge, pour une température identique
(que l’on suppose non modifiée par l’ajout de l’adhésif).

![Plaque chauffante à différentes émissivités](plaque.png){#fig:plaque}

## Travail préparatoire

Réalisé sur Amétice.

Notions importantes abordées :

- Le signal électrique de la caméra infrarouge est proportionnel au flux total reçu par le détecteur. Ce flux comprend :
    - Le rayonnement émis par la scène thermique (proportionnel à sa température et son émissivité).
    - Le rayonnement réfléchi provenant de l’environnement.


- L'expérience d'étalonnage d'une caméra infrarouge consiste à viser un corps noir à température connue et enregistrer la tension délivrée par le détecteur infrarouge de la caméra.
    
    Par exemple, si une caméra infrarouge vise une surface « réelle » (c'est à dire « non-noire ») de température réelle inconnue et placée dans un environnement de température inconnue et indique que sa température apparente corps noir de 57°C, cela signifie que 
    cette surface envoie un flux infrarouge vers la caméra qui correspond à celui qu'émettrait le corps noir à 57°C


- La caméra infrarouge mesure une température apparente corps noir, mais la température vraie de la surface dépend de son émissivité et du rayonnement réfléchi par l’environnement.



# Expériences

## Observation d'un corps noir et de surfaces non noires en environnement uniforme

### Introduction

L’étalonnage de la caméra infrarouge consiste à enregistrer la réponse (en V) de la caméra face à un corps noir de laboratoire à température variable $T^{0}$​. La tension mesurée $\Delta V_{0}(T_{0})$ est liée à la température $T^{0}$ par la formule suivante :

$$\Delta V^0(T^0) = k \int_{\lambda} R(\lambda) L^{0}(\lambda, T^{0}) \, d\lambda \tag{1}$$

Avec : 

- $R(\lambda)$ la sensibilité spectrale relative du détecteur dans la bande $\Delta \lambda$.
- k une constante dépendant de la sensibilité maximale (en V/W) du détecteur, du gain de la chaîne
d’amplification et des grandeurs relatives à la géométrie de la détection.

Lors de la mesure sur un corps réel, l'émissivité $\epsilon (\lambda)$ influence la tension mesurée $\Delta V_{mes}$​, qui peut être exprimée par :

$$\Delta V_{mes} = k \int_{\lambda} R(\lambda) \varepsilon(\lambda) L^0_{\lambda} (\lambda, T) \, d\lambda + k \int_{\lambda} R(\lambda) \left[ 1 - \varepsilon(\lambda) \right] L^0_{\lambda} (\lambda, T_a)  d\lambda \tag{2}$$

Soit  :

$$\Delta V_{mes} = \epsilon_{\Delta \lambda} \Delta V^0(T) + (1 - \epsilon_{\Delta \lambda}) \Delta V^0(T_{a}) = \Delta V^0(T^0) \tag{3}$$

Avec : 

$$ \epsilon_{\Delta \lambda} = \frac{\int_{\lambda} \epsilon(\lambda)R(\lambda)L^0_{\lambda}(\lambda,T) d\lambda}{\int_{\lambda} R(\lambda)L^0_{\lambda}(\lambda,T) d\lambda} \tag{4}$$

La température apparente du corps réel, $T^{0}_{mes}$​, est calculée en fonction de $\Delta V_{mes}$​, offrant ainsi une estimation de la température du matériau observé.

$$(T^{0}_{mes})^{4} = \epsilon_{\Delta \lambda} T^4 + (1-\epsilon_{\Delta \lambda})T^4_{a} \tag{5}$$

Avec : 

- $T^{0}_{mes}$ la température apparente corps noir
- $\epsilon_{\Delta \lambda}$ l’émissivité spectrale de la surface dans la bande spectrale de la caméra.
- T la vraie température
- $T_{a}$ la température de l'environnement

Donc, plus l'émissivité de la surface est grande (proche de 1), plus la température mesurée sera proche de la température vraie.
Inversement, si l'émissivité est faible (proche de 0), la température mesurée sera proche de la température ambiante.

### Travail à réaliser

Pour commencer, un étalonnage de la caméra est nécessaire, pour cela il faut utiliser un corps noir à température connue (affichage sur un régulateur).

Cet étalonnage est réalisé en placant le corps noir devant la caméra (Voir Figure \ref{fig:exp1}) et en vérifiant que la température mesurée par la caméra correspond bien à la température mesurée sur le régulateur.

![Schéma du montage pour l'étalonnage devant le corps noir de laboratoire ](exp1.png){#fig:exp1}


Cette expérience permet d'obtenir la température du corps noir grâce à $T_{mes}$ ainsi que la vraie température donnée par les thermocouples. La température ambiante $T_{a}$ et l'équation (5) sont également nécéssaires pour déterminer l'émissivité du corps noir.

$$\epsilon = \frac{T^{4}_{mes} - T^{4}_{a}}{T^{4} - T^{4}_{a}} = \frac{352.05^{4}-294.15^{4}}{353,21^{4}-294.15^{4}} \approx 0.97$$

Cette émissivité est proche de 1 (émissivité d'un corps noir), l'écart relatif est de $\frac{\epsilon_{mes} - 1}{1} \approx 3$%

Il est intéressant de mettre différents objets devant la caméra pour observer les variations de température au sein des objets et également de mettre en évidence leurs différences d'émissivité et de transmitivité.

![Photo d'un camarade avec lunettes](adrien.jpeg){#fig:adrien width=60%}


\begin{figure}
    \centering
    \begin{minipage}{0.45\textwidth}
        \centering
        \includegraphics[width=\linewidth]{baptiste.jpeg}
        \caption{Photo de Baptiste à la caméra thermique}
    \end{minipage}
    \hfill
    \begin{minipage}{0.45\textwidth}
        \centering
        \includegraphics[width=\linewidth]{leo.jpeg}
        \caption{Photo de Léo à la caméra thermique}
    \end{minipage}
\end{figure}


Nous remarquons ainsi que les lunettes de notre camarade sont très foncées à la caméra, cela s'explique du fait que la 
transmitivité du verre est quasiment nul dans l'infrarouge (Etudié au TP précédent - Rayonnement Thermique).



Maintenant que la caméra est étalonnée, il est possible de faire la mesure sur des corps réels comme indiqué sur la Figure \ref{fig:exp2}.
Une plaque chauffante (Voir Figure \ref{fig:plaque}) sur laquelle sont placés différents matériaux, faisant donc varier les émissivités des parties de la plaque.

![Schéma du montage pour la mesure sur un corps réel (plaque chauffante)](exp2.png){#fig:exp2}


Pour calculer les émissivités des différentes surfaces on peut utiliser la formule (5).

|Surface observée|Température T du thermocouple associé (°C)|Température $T_{mes}$ relevée par la caméra (°C)| Emissivité $\epsilon$|
|:-----:|:-----:|:-----:|:-----:|
|Aluminium| 38,89 | 24,9    | 0,17    |
|Aluminium + vernis|38,92 | 37,1 |0,87 |
|Aluminium + scotch|38,93  | 33,7 | 0,68 |
|Noire| 38,92 |38,5 | 0,97 | 

: Tableau des mesures et des émissivités calculées

Pour résumer : 

Les surfaces qui sont peintes en noir ou qui ont des propriétés similaires à celles d'un corps noir auront une émissivité proche de 1. Cela signifie qu'elles émettent presque tout le flux qu'elles reçoivent.

Les surfaces métalliques ou brillantes, en revanche, auront une émissivité plus faible, ce qui signifie qu'elles reflètent une grande partie du flux incident et émettent moins de chaleur, on remarque ici que le vernis est plus émissif que l'adhésif.

__Remarque :__ 

Lorsque nous passons devant le dispositif (et derrière la caméra), la plaque réfléchissante renvoie le flux de chaleur de notre corps sur la caméra et une différence de température mesurée est remarquable. (Voir Figures \ref{fig:reflet1} et \ref{fig:reflet2})

\newpage

\begin{figure}
    \centering
    \begin{minipage}{0.45\textwidth}
        \centering
        \includegraphics[width=1.1\linewidth]{reflet1.jpeg}
        \caption{Vue de la caméra sans reflet de chaleur de notre corps}
        \label{fig:reflet1}
    \end{minipage}
    \hfill
    \begin{minipage}{0.45\textwidth}
        \centering
        \includegraphics[width=1.1\linewidth]{reflet2.jpeg}
        \caption{Vue de la caméra avec reflet de chaleur de notre corps}
        \label{fig:reflet2}
    \end{minipage}
\end{figure}

La zone mesurée est l'encadré bleu prenant toute la largeur en haut de l'image sur les deux photos.

Les températures comparées sont les températures encadrées en gras en bas de l'image (21,6°C et 25,6°C).

Nous remarquons une augmentation de la température moyenne mesurée sur la zone de reflet de notre chaleur corporelle.



## Influence d’un environnement non uniforme sur l’observation d’objets non noirs : réflexions parasites


On chauffe un premier cube à 30°C, où l'on va mesurer les températures des faces noire, métallique non polie puis blanche. Dans un second temps on chauffe un deuxième cube à 130°C, placé (perpendiculairement) au premier pour créer une zone pertubée devant le cube à 30°C. (Voir figures \ref{fig:exp3} et \ref{fig:exp3_bis}).


![Surfaces de différentes émissivités (3 faces du cube multifaces) observées dans un environnement
uniforme (à gauche), puis perturbé par une source de rayonnement chaude et émissive (à
droite), qui est la face noire du second cube multifaces](exp3.png){#fig:exp3}

\newpage

![Observation du cube multiface dans un environnement uniforme (en haut) et dans un environnement perturbé (en bas)](exp3_bis.png){#fig:exp3_bis}


\begin{figure}
    \centering
    \begin{minipage}{0.45\textwidth}
        \centering
        \includegraphics[width=1.1\linewidth]{courbe2.png}
        \caption{Observation des variations de température pour chaque face du cube dans un environnement uniforme}
        \label{fig:courbe2}
    \end{minipage}
    \hfill
    \begin{minipage}{0.45\textwidth}
        \centering
        \includegraphics[width=1.1\linewidth]{courbe1.png}
        \caption{Observation des variations de température pour chaque face du cube dans un environnement perturbé}
        \label{fig:courbe1}
    \end{minipage}
\end{figure}

D'après le profil des températures de chaque face en environnement uniforme (Figure \ref{fig:courbe2}), on peut établir un classement d'émissivité des faces. Par ordre croissant cela donne : face non polie, face noire puis face blanche. La température est le critère de classement, on remarque que la température est plus élevée pour la face blanche, cela s'explique par la plage de longueur d'onde de la caméra (entre 7 et 13 $\mu m$). Dans cette zone l'émissivité de la face blanche est plus élevée que celle de la face noire.


Il est possible de remarquer que les profils de température sont différents dans la deuxième situation (Figure \ref{fig:courbe1}). En effet, la température observée le long de la face du cube décroit en fonction de sa distance au cube chaud. 

Pour la face non polie, la pente de décroissance est plus importante que pour les pentes des faces blanches et noires, c'est-à-dire que la température de la surface décroit plus rapidement en fonction de la distance. C'est à dire que plus nous prenons des mesures de températures loin du cube chaud, moins les températures mesurées sont élevées.

Ces observations pouvaient se prévoir car la face non polie est très peu émissive mais plutôt réflective, contrairement aux faces blanches et noires.


On peut donc faire un classement de chaque face en fonction de leur réflectivité. Par ordre croissant cela donne : Face noire, face blanche puis face non polie.



TODO : Faire schéma des flux recueillis par la caméra dans les deux environnment + légender photos

\begin{figure}
    \centering
    \begin{minipage}{0.45\textwidth}
        \centering
        \includegraphics[width=1.1\linewidth]{env_unif.jpeg}
        \caption{Environnement uniforme - La température est quasi constante dans la totalité de la surface}
        \label{fig:env_unif}
    \end{minipage}
    \hfill
    \begin{minipage}{0.45\textwidth}
        \centering
        \includegraphics[width=1.1\linewidth]{env_perturb.jpeg}
        \caption{Environnement perturbé - La température varie par rapport à la distance de la source chaude}
        \label{fig:env_perturb}
    \end{minipage}
\end{figure}


Dans la figure \ref{fig:env_unif}, la couleur de la surface est uniforme, cela indique que la température est quasiment la même sur toute cette surface du cube.


Dans la figure \ref{fig:env_perturb},le flux de chaleur se propage dans la direction des flèches blanches.
On peut observer différents niveaux de couleurs sur la face du cube observé.


Nous pouvons ajouter que une image infrarouge ne donne pas directement une cartographie exacte de la température, mais plutôt une mesure du rayonnement thermique, qu'il faut corriger en fonction de l'émissivité pour obtenir la température réelle.

La caméra infrarouge mesure donc une température apparente corps noir, mais la température vraie de la surface dépend de son émissivité et du rayonnement réfléchi par l'environnement.
Il est ainsi possible de retrouver la vraie température en conaissant la température ambiante, la tempéraure mesurée et l'émissivité de la surface.

# Conclusion

Ce TP nous a permis de mieux comprendre le fonctionnement et l'interprétation des images obtenues avec une caméra infrarouge. Nous avons observé l'influence de l'émissivité des matériaux sur la température apparente mesurée, ainsi que l'importance des réflexions parasites dans un environnement non uniforme.

Les expériences réalisées ont mis en évidence que les surfaces à haute émissivité, comme la peinture noire, permettent une mesure plus fiable de la température réelle, tandis que les surfaces réfléchissantes faussent la mesure en captant et en renvoyant le rayonnement de leur environnement. De plus, nous avons pu constater que des éléments comme le verre ou l'aluminium poli influencent fortement la captation du rayonnement infrarouge.

Ces observations soulignent l'importance de bien comprendre les propriétés des matériaux lors de l'utilisation d'une caméra thermique, notamment dans des domaines comme l'industrie, le bâtiment ou la recherche. Ce TP nous a ainsi apporté une vision concrète des phénomènes thermiques liés au rayonnement infrarouge et de leur impact sur la mesure et l'analyse des températures.