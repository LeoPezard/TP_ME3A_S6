---
title: Compte rendu de TP - Spectrophotométrie - Pyrométrie 
author: Baptiste Fanget - Léo Pezard - Mécanique Energétique 3A
date: 18/03/2025
papersize: a4
lang: fr 
secnumdepth: 3
---

# Introduction

La spectrophotométrie et la pyrométrie sont deux techniques essentielles en physique permettant d’analyser les interactions entre la lumière et la matière. La spectrophotométrie repose sur l’absorption et la transmission de la lumière par un échantillon afin d’en déduire des informations telles que la concentration d’une substance ou ses propriétés optiques. La pyrométrie, quant à elle, est une méthode permettant de mesurer la température d’un objet en analysant le rayonnement qu’il émet.

## Le spectre électromagnétique

Le rayonnement électromagnétique regroupe les ondes classées selon leur longueur d’onde $\lambda$ ou leur fréquence $\nu$. Il se divise en plusieurs domaines :

Le spectre visible (380-780 nm, $\approx$ 500 THz) : perçu par l’œil humain, il correspond aux couleurs visibles des objets éclairés.
  
Les rayonnements énergétiques (longueurs d’onde courtes, hautes fréquences) :
    
- Ultraviolets (UVA, UVB, UVC) : responsables des coups de soleil.
    
- Rayons X : utilisés en imagerie médicale.
    
- Rayons gamma : issus des réactions nucléaires et cosmiques.
    
Les rayonnements moins énergétiques (longueurs d’onde longues, basses fréquences) :
    
- Infrarouges : liés au rayonnement thermique.
    
- Micro-ondes : utilisées en télécommunications et cuisson.
    
- Ondes radio et hertziennes : utilisées pour la transmission d’informations.

Un spectre représente l’intensité lumineuse en fonction de la longueur d’onde. Ce TP étudiera le rayonnement thermique et celui issu de la désexcitation des atomes et molécules d’un gaz.

![Le spectre électromagnétique](spectres.png){#fig:spectres}

## Le rayonnement thermique

Le rayonnement thermique d’une surface est comparé à celui d’un corps noir, un émetteur parfait absorbant toute la lumière incidente. Son rayonnement dépend de la température T et de la longueur d’onde $\lambda$.

**Loi de Planck**

Elle décrit l’énergie rayonnée par un corps noir à température T :

$L_{0}(\lambda, T) = \frac{C_1}{\lambda^5} \cdot \frac{1}{\exp\left(\frac{C_2}{\lambda T}\right) - 1}$



avec $C_1$​ et $C_2$​ des constantes. Elle montre que plus un corps est chaud, plus il émet d’énergie et que son spectre présente un maximum d’intensité.

**Loi de Wien**

Elle donne la longueur d’onde où l’émission est maximale :

$\lambda_{max}(\mu m)= \frac{2898}{T}$

**Émissivité et température de luminance :**

Un corps réel n’émet jamais autant qu’un corps noir et possède une émissivité $\epsilon$ inférieure à 1 :

$L(\lambda ,T)= \epsilon (\lambda ,T) \cdot L^0(\lambda,T)$


On définit aussi une température de luminance $T_L$​, toujours inférieure à la température réelle du corps. Si $\epsilon$ est constant, le corps est dit "gris".

![La loi de Planck](planck.png){#fig:planck}

\newpage

TODO : mettre la figure 2 et surtout écrire les equations correctement et faire la mise en page

## Le pyromètre optique

Un pyromètre optique mesure la température d’une source via un détecteur photoélectrique.

- Monochromatique : mesure la luminance à une seule longueur d’onde, dépendant de l’émissivité $\epsilon$.
  
- Bi-chromatique : compare la luminance à deux longueurs d’onde, évitant l’influence de $\epsilon$.
  
- À large bande : mesure l’énergie totale émise.

Les pyromètres à disparition de filament comparent la luminance d’une source à celle d’un filament de tungstène, ajusté jusqu’à disparition visuelle.

## Travaux préliminaires

1) Loi de Planck : $L_{0}(\lambda, T) = \frac{C_1}{\lambda^5} \cdot \frac{1}{\exp\left(\frac{C_2}{\lambda T}\right) - 1}$


Avec $C_1 = 2hc^2$, $C_2 = \frac{hc}{k}$.

Pour trouver le maximum de la luminance on résout : $\frac{dL_O}{d \lambda} = 0$

$\rightarrow \frac{dL_O}{d \lambda} = C_1[-5 \lambda^{-6}\frac{1}{\exp{\frac{C_2}{\lambda T}}-1} + \lambda^{-5} \cdot \frac{\frac{C_2}{\lambda^{2} T}\exp{\frac{C_2}{\lambda T}}}{(\exp{\frac{C_2}{\lambda T}}-1)^{2}}] = 0$

$\rightarrow \frac{5}{\lambda^{6}\cdot \exp{\frac{C_2}{\lambda T}}-1} = \frac{C_2 \cdot \exp{\frac{C_2}{\lambda T}}}{\lambda^{7} T \cdot \exp{\frac{C_2}{\lambda T}}-1}^{2}$


$\rightarrow \lambda = \frac{C_2 \exp\left(\frac{C_2}{\lambda T}\right)}{5T \left( \exp\left(\frac{C_2}{\lambda T}\right) - 1 \right)}$

Posons $x = \frac{C_2}{\lambda T}$, alors :

$\rightarrow \lambda = \frac{C_2 e^x}{5 (e^x - 1) T}$

En multipliant par $x$:

$5 (e^x - 1) = x e^x$

Ainsi, la longueur d'onde maximale $\lambda_{\text{max}}$ vérifie :

$x_{\text{max}} = \frac{C_2}{\lambda_{\text{max}} T} \approx 4.9651$

$\lambda_{\text{max}} = \frac{C_2}{4.9651 T}$

Avec $C_2 = 1.4388 \times 10^{-2}$, on obtient :

$\lambda_{\text{max}} = \frac{1.4388 \times 10^{-2}}{4.9651 T} = \frac{2898}{T} \quad \text{(en µm)}$


2) Déplacement du spectre d'émission

Lorsque la température d'un objet augmente, son spectre d'émission se décale vers de plus petites longueurs d'onde car :

$\lambda_{\text{max}} \propto \frac{1}{T}$


3) Apparition des couleurs visibles

Lorsque la température d'un objet augmente petit à petit, la première couleur visible est le rouge, car il émet d'abord dans l'infrarouge. Ensuite, la longueur d'onde diminue pour tendre vers le bleu.

4) Relation entre luminance et émissivité

$L(\lambda, T) = \varepsilon(\lambda, T) \cdot L_0(\lambda, T)$

$\Rightarrow L(\lambda, T) = L_0(\lambda, T_L) \cdot \exp\left(-\frac{C_2}{\lambda T}\right)$

$\Rightarrow \exp\left(-\frac{C_2}{\lambda T_L}\right) = \varepsilon(\lambda, T) \cdot \exp\left(-\frac{C_2}{\lambda T}\right)$

En appliquant $\ln$ :

$-\frac{C_2}{\lambda T_L} = -\frac{C_2}{\lambda T} + \ln(\varepsilon(\lambda, T))$

$\Rightarrow \frac{1}{T_L} = \frac{1}{T} - \frac{1}{C_2} \ln(\varepsilon)$

Avec : $A.N. \text{  } \frac{1}{T_L} = 6,73 \times 10^{-4} \ \text{K}^{-1}$ $\Rightarrow T_L = 1488 \ \text{K}$

$A.N. \text{  } \frac{1}{T_L} =  8,03 \times 10^{-4} \ \text{K}^{-1}$ $\Rightarrow T_L = 1245 \ \text{K}$

On en conclut que plus l’émissivité est faible, plus la température de luminance $T_L$ est supérieure à la température réelle $T$.
Un pyromètre monochromatique est très sensible à l’émissivité.


5) Nouvelle expression de la luminance

$L(\lambda, T) = \varepsilon(\lambda, T) \exp\left(-\frac{C_2}{\lambda T}\right)$

$v_{\lambda_1} = K(\lambda_1) \varepsilon(\lambda_1) \exp\left(-\frac{C_2}{\lambda_1 T}\right)$

Avec :

$K(\lambda_{1}) = R \cdot S_{\lambda_{1}} \cdot T_{\rho_{\lambda_{1}}} \cdot d\lambda_{1} \cdot T_{0\lambda} \cdot \Omega \cdot S \cdot \tau_{1\lambda}$
