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

Le rayonnement électromagnétique regroupe les ondes classées selon leur longueur d’onde λλ ou leur fréquence νν. Il se divise en plusieurs domaines :

Le spectre visible (380-780 nm, ~500 THz) : perçu par l’œil humain, il correspond aux couleurs visibles des objets éclairés.
  
Les rayonnements énergétiques (longueurs d’onde courtes, hautes fréquences) :
    
- Ultraviolets (UVA, UVB, UVC) : responsables des coups de soleil.
    
- Rayons X : utilisés en imagerie médicale.
    
- Rayons gamma : issus des réactions nucléaires et cosmiques.
    
Les rayonnements moins énergétiques (longueurs d’onde longues, basses fréquences) :
    
- Infrarouges : liés au rayonnement thermique.
    
- Micro-ondes : utilisées en télécommunications et cuisson.
    
- Ondes radio et hertziennes : utilisées pour la transmission d’informations.

Un spectre représente l’intensité lumineuse en fonction de la longueur d’onde. Ce TP étudiera le rayonnement thermique et celui issu de la désexcitation des atomes et molécules d’un gaz.

TODO : Mettre la figure 1 du TP

## 1.2 Le rayonnement thermique

Le rayonnement thermique d’une surface est comparé à celui d’un corps noir, un émetteur parfait absorbant toute la lumière incidente. Son rayonnement dépend de la température T et de la longueur d’onde λ.

Loi de Planck

Elle décrit l’énergie rayonnée par un corps noir à température T :

L0(λ,T)=C1λ5⋅1exp⁡(C2/λT)−1

L0​(λ,T)=λ5C1​​⋅exp(C2​/λT)−11​

avec C1​ et C2​ des constantes. Elle montre que plus un corps est chaud, plus il émet d’énergie et que son spectre présente un maximum d’intensité.

Loi de Wien

Elle donne la longueur d’onde où l’émission est maximale :

λmax(μm)=2898T

λmax​(μm)=T2898​

Émissivité et température de luminance

Un corps réel n’émet jamais autant qu’un corps noir et possède une émissivité ε inférieure à 1 :

L(λ,T)=ε(λ,T)⋅L0(λ,T)

L(λ,T)=ε(λ,T)⋅L0​(λ,T)

On définit aussi une température de luminance TL​, toujours inférieure à la température réelle du corps. Si ε est constant, le corps est dit "gris".

TODO : mettre la figure 2 et surtout écrire les equations correctement et faire la mise en page

## 1.3 Le pyromètre optique

Un pyromètre optique mesure la température d’une source via un détecteur photoélectrique.

- Monochromatique : mesure la luminance à une seule longueur d’onde, dépendant de l’émissivité ε.
  
- Bi-chromatique : compare la luminance à deux longueurs d’onde, évitant l’influence de ε.
  
- À large bande : mesure l’énergie totale émise.

Les pyromètres à disparition de filament comparent la luminance d’une source à celle d’un filament de tungstène, ajusté jusqu’à disparition visuelle.

## 1.4 Travaux préliminaires

1)

## Dispositif expérimental

L'étude est réalisée à l'aide d'un banc d'essai (voir Figure \ref{fig:dispositif}) permettant de générer un écoulement d'air autour de surfaces chauffées et d'en mesurer les effets thermiques. Le montage expérimental comprend :

- Un film chauffant (résistance électrique) pris en sandwich entre deux plaques de cuivre de $3.8$ cm de large, $6.4$ cm de long et $2$ mm d'épaisseur.
- Un tube en Plexiglas dans lequel circule l'air à différentes vitesses générées par un ventilateur.
- Une sonde à fil chaud permettant de mesurer la vitesse de l'écoulement.
- Une alimentation en courant continu avec affichage de la tension et du courant appliqués à la résistance chauffante.
- Un thermocouple de type K placé sur la plaque pour mesurer la température de surface.

Une deuxième configuration intègre une ailette en cuivre de 50 cm de long, 3 cm de large et 1 mm d'épaisseur, permettant d'analyser son impact sur l'amélioration des échanges thermiques.

![Dispositif expérimental](dispositif.png){#fig:dispositif}

\newpage


## Effet des ailettes

L'ajout d'ailettes est une technique courante pour augmenter les échanges de chaleur entre un solide et un fluide. En augmentant la surface d'échange, elles permettent une meilleure dissipation thermique. Le principe repose sur deux phénomènes :

1. **Augmentation de la surface d'échange** : Plus la surface est grande, plus le flux thermique total $\Phi$ est important.
2. **Conduction et convection combinées** : La chaleur est transférée par conduction le long de l'ailette, puis dissipée par convection.

La température d'une ailette suit une décroissance exponentielle donnée par :  
$$
T(x) = T_{\infty} + (T_0 - T_{\infty}) e^{-\frac{x}{L}}
$$
où :

- $T(x)$ est la température à une distance $x$ de la base de l'ailette.
- $T_{\infty}$ est la température du fluide ambiant.
- $T_0$ est la température de la base de l'ailette.
- $L$ est la longueur caractéristique de l'ailette :  
  $$
  L = \sqrt{\frac{k S}{h P}}
  $$
  avec $k$ la conductivité thermique du matériau, $S$ la section de l'ailette et $P$ son périmètre.

Le flux total évacué par l'ailette est donné par :  
$$
\Phi = h P L (T_0 - T_{\infty})
$$
Cette expression permet d'évaluer l'efficacité des ailettes en fonction du coefficient d'échange convectif $h$, de la conductivité thermique $k$ et de la géométrie de l'ailette.



# Expériences

## Détermination des coefficients d'échange convectifs h

### Procédure à suivre

 Afin de déterminer le coefficier d'échange convectif $h$, on fixe une vitesse d'écoulement $v$ sur le ventilateur. Un thermocouple nous permet d'obtenir la température $T_0$ à la sortie (une fois la température stabilisée).

Une tension est ensuite imposée sur la résistance dans la plaque chauffante, créant ainsi une puissance $P$. Cette puissance sera utilisée ainsi que la surface de la plaque chauffante $S$ pour déterminer le coefficient d'échange convectif $h$ grâce à la formule : 

$$
  P = UI = \Phi_{cv} = h \cdot S \cdot \Delta T
$$

Les différences de température sont prises lorsque une tension est appliquée à la résistance, permettant d'obtenir le terme $\Delta T$.

On obtient $h$ avec nos mesures $P = f(S.\Delta T)$, ainsi $h$ est le coefficient directeur de la droite.

$$\rightarrow h = \frac{\Phi_{cv}}{S \cdot \Delta T}$$

Ainsi, voici nos coefficients d'échanges convectifs pour chaque vitesse :

|Vitesse (m/sec) | Coefficient d'échange convectif $h$ (W/m².°C)|
|:----:|:----:|
|6,52|96,25|
|4,26|76,65|
|3,52 |70,44 |


Voici nos graphiques de $P=f(S.\Delta T)$ pour différentes vitesses :

![$P = f(S.\Delta T)$ pour une vitesse de 6,52 m/sec](flux_v1.png){width=80%}

![$P = f(S.\Delta T)$ pour une vitesse de 4,26 m/sec](flux_v2.png){width=80%}

![$P = f(S.\Delta T)$ pour une vitesse de 3,52 m/sec](flux_v3.png){width=80%}


\newpage

### Dépendance du coefficient d'échange

Pour déterminer la dépendance du coefficient d'échange, $h$ à la vitesse $v$, on trace $h = f(v)$.

![Coefficient d'échange en fonction de la vitesse](h_f(v).png){#fig:h_v width=80%}


### Nu en fonction du Reynolds

Pour tracer $Nu = f(Re)$ on a $Re = \frac{\rho U L}{\mu}$ et $Nu = \frac{h L}{k}$

On utilise la longueur de la plaque $L = 6,8\cdot 10^{-2}m$ et en se référant aux tables à notre disposition on a pour l'air $\rho_{air} =1,16 \text{ } kg.m^{-3} , \mu_{air} = 184,6\cdot 10^{-7} \text{ } N.s.m^{-2}, k_{air} = 26,3\cdot 10^{-3} W.m^{-1}K^{-1}$

|Vitesse (m/sec) | Re | Nu |
|:----:|:----:|:---:|
|6,52| 27860  | 248,86  |
|4,26| 18203| 198,18  |
|3,52 |15041 | 182,13  |

Nous avons des nombres de Reynolds inférieurs à $3\cdot 10^{5}$  donc le régime est Laminaire.

La théorie montre que dans ce type d'écoulements, $Nu = 0,665\cdot Re_{L}^{0,5} \cdot Pr^{\frac{1}{3}}$

Donc $Nu$ évolue en fonction de la racine du Reynolds, nos graphiques (Figure \ref{fig:h_v} et \ref{fig:Nu_Re}) de $h = f(v)$ et $Nu = f(Re)$ démontrent bien cette évolution car avec un profil de puissance nous obtenons une puissance proche de 0,5 dans les deux cas.

![Nombre de Nusselt en fonction du nombre de Reynolds](Nu_f(Re).png){#fig:Nu_Re width=80%}


## Profils d'ailette

Travaillons maintenant avec le dispositif grandes dimensions, constitué d'une ailette de 50cm de long à l'extrémité de deux plaques de cuivres rectangulaires prenant en sandwich un film chauffant.

### Mesures du profil stationnaire de température dans l'ailette

Pour cela, nous chauffons à l'origine de la plaque et imposons une vitesse de 5,48 m/sec à l'écoulement, puis de 3,25 m/sec.

Nous obtenons un profil des températures le long de la plaque pour chaque vitesse.



On remarque la forme d'une exponentielle décroissante dans les deux cas car d'après l'énoncé : $T(x) = T_{\infty} + (T_0 - T_{\infty}) e^{-\frac{x}{L}}$

D'où : $ln(\frac{T(x)-T_{\infty}}{T_0-t_{\infty}}) \propto -\frac{x}{L}$

Ainsi, le tracé de la température le long de la plaque chauffante est tracé pour chaque vitesse (voir Figure \ref{fig:profil_temperatures})

![Fonction T*(x) =  $ln(\frac{T(x)-T_{\infty}}{T_{0}-T_{\infty}})$ en fonction de la distance par rapport à la plaque chauffante](profil_temperatures.png){#fig:profil_temperatures}


### Détermination de la longueur caractéristique

Nous trouvons ainsi les coefficients $\frac{1}{L}$, pentes des courbes, nous donnant $L$, longueur caractéristique, pour chaque vitesse de l'écoulement. On obtient donc L = 6,98 cm pour une vitesse de 3,25 m/sec et L = 5,75 cm pour une vitesse de 5,48 m/sec.

On remarque donc que plus la vitesse est élevée, moins la longueur caractéristique est grande car il y a un plus grand flux d'air qui permet de diminuer la température de la surface (atteindre $T_{\infty}$ plus rapidement).


# Conclusion

Les expériences menées ont permis d’analyser l’influence de la vitesse d’écoulement sur le coefficient d’échange convectif h et d’observer que h suit une loi en racine de Reynolds, conformément aux modèles théoriques. L’ajout d’ailettes s’est révélé efficace pour améliorer le transfert thermique, en augmentant la surface d’échange et en favorisant la dissipation de chaleur. La diminution de la longueur caractéristique avec l’augmentation de la vitesse confirme que le flux thermique est mieux réparti à grande vitesse. Enfin, les résultats expérimentaux sont cohérents avec les prédictions théoriques, validant ainsi les modèles utilisés.
