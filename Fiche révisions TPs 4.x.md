---
title: Révision des TPs 
author: Baptiste Fanget - Léo Pezard - Mécanique Energétique 3A
papersize: a4
lang: fr 
secnumdepth: 3
---

# TP 4.1 Conduction thermique

## Introduction

Ce TP a pour objectif d'explorer les mécanismes de conduction thermique dans une configuration monodimensionnelle, à travers l'étude expérimentale de barres métalliques en contact. 

En régime stationnaire, il s'agit de mesurer la conductivité thermique de deux métaux, tandis qu'en régime instationnaire, le temps diffusif et les dynamiques de stabilisation thermique sont examinés. L'utilisation de l'analogie électrique-thermique permet d'introduire des concepts clés comme la résistance thermique et la capacitance thermique. 

À l'aide d'un dispositif instrumenté de thermocouples et d'une acquisition informatique, les températures et flux thermiques sont mesurés pour comprendre les phénomènes en jeu. Ce TP fournit ainsi une première approche complète des transferts de chaleur dans des systèmes simples mais représentatifs.

## Notions clés

### Calorimétrie et énergie interne stockée
- Énergie interne stockée :  
  $E_{stock}$ = $mC_{p}$ ($T_{fin}$ - $T_{ini}$) = $\rho$ $C_{p}$ V ($T_{fin}$ - $T_{ini}$)

  où :
  - $C_{p}$  : chaleur spécifique (J/kg·K).
  - $\rho$ : masse volumique (kg/m³).
  - _V_ : volume (m³).

- Puissance stockée dans un fluide en écoulement :  
   $P_{fluide}$ = $mC_{p}$ ($T_{sortie}$ - $T_{entrée}$)  
  où ${m}$ = $\rho q$ (kg/s).

---

### Loi de Fourier

La loi de Fourier exprime le flux de chaleur en fonction du gradient de température à travers un matériau conducteur. 

- Flux d'énergie interne en conduction thermique :  $\Phi_{x}$ = -k S $\frac{dT}{dx}$
 - $\Phi_{x}$ : flux (W).
  - $k$ : conductivité thermique (W/m·K).
  - $S$ : section (m²).
  - $\phi_{x} = \frac{\Phi_{x}}{S}$ : densité de flux (W/m²).

---

## Conclusion

La conduction thermique est un mode de transfert de chaleur qui se produit à travers un matériau sans déplacement de matière. Elle repose sur la transmission de l'agitation thermique des particules voisines. Ce phénomène est décrit par la loi de Fourier, qui indique que le flux de chaleur est proportionnel au gradient de température et à la conductivité thermique du matériau. Les matériaux comme les métaux sont de bons conducteurs, tandis que le bois ou le plastique sont de mauvais conducteurs (isolants).


# TP 4.2 Rayonnement thermique

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


## Conclusion

Le rayonnement thermique est un transfert de chaleur par ondes électromagnétiques, sans support matériel, selon la loi de Planck. Le TP avec le cube de Leslie a montré que les surfaces noires et mates émettent plus de chaleur que les brillantes, illustrant la loi de Stefan-Boltzmann et l’émissivité des matériaux. L’expérience a approfondi notre compréhension de ces phénomènes et mis en évidence l’influence de la nature des surfaces. De plus, l’étude de la transmission du rayonnement a illustré l’effet de serre, reliant théorie et pratique tout en sensibilisant aux limites expérimentales.


# TP 4.3 Caméra infrarouge

## Introduction

L’imagerie infrarouge repose sur la détection du rayonnement thermique émis par les objets en fonction de leur température (loi de Planck). Une caméra infrarouge capte ce rayonnement dans la gamme 7,5-13 $\mu m$ grâce à une matrice de microbolomètres, qui convertissent l’énergie thermique en signal électrique. Le signal détecté est proportionnel au flux total reçu, comprenant le rayonnement émis par l’objet et celui réfléchi par l’environnement.


- Le signal électrique de la caméra infrarouge est proportionnel au flux total reçu par le détecteur. Ce flux comprend :
    - Le rayonnement émis par la scène thermique (proportionnel à sa température et son émissivité).
    - Le rayonnement réfléchi provenant de l’environnement.


- L'expérience d'étalonnage d'une caméra infrarouge consiste à viser un corps noir à température connue et enregistrer la tension délivrée par le détecteur infrarouge de la caméra.
    
    Par exemple, si une caméra infrarouge vise une surface « réelle » (c'est à dire « non-noire ») de température réelle inconnue et placée dans un environnement de température inconnue et indique que sa température apparente corps noir de 57°C, cela signifie que 
    cette surface envoie un flux infrarouge vers la caméra qui correspond à celui qu'émettrait le corps noir à 57°C


- La caméra infrarouge mesure une température apparente corps noir, mais la température vraie de la surface dépend de son émissivité et du rayonnement réfléchi par l’environnement.


L’émissivité d’un matériau influence directement son apparence en imagerie thermique. Une surface noire et mate, fortement émissive, émet plus de rayonnement et paraît plus chaude qu’une surface brillante ou réfléchissante, qui renvoie une partie du rayonnement ambiant. Ainsi, la température mesurée par la caméra est une température apparente, dépendant de l’émissivité et du rayonnement réfléchie.

| Face | Émissivité ($\epsilon_{0.4 - 40 \mu m}$) |
|:----------------:|:-----------:|
| Noire                | 0.94|
| Blanche              | 0.92|
| Polie                | 0.05|
| Non polie            | 0.1 |

:Émissivités de chaque face calculées lors du TP précédent.


## Conclusion 


L’interprétation des images infrarouges nécessite donc de corriger ces effets pour obtenir des mesures précises. L’étalonnage avec un corps noir permet d’établir une référence fiable, en enregistrant la tension délivrée par la caméra pour une température connue. Cela est crucial, car une surface réelle n’émet pas forcément le même flux qu’un corps noir à même température.

Grâce à cette technologie, il est possible d’analyser la répartition thermique des objets avec précision, ce qui la rend essentielle dans des domaines variés, tels que la thermographie des bâtiments, l’industrie et la recherche scientifique.


# TP 4.4 Sillage et traînée

## Introduction

Ce travail pratique a pour objectif d'étudier l'écoulement autour et en aval d'un cylindre, en utilisant le tube de Pitot pour mesurer la vitesse du fluide. Il s'agit également d'exploiter les notions de mécanique des fluides abordées au semestre S5 afin de déterminer la force de traînée exercée sur le cylindre. L'analyse repose sur le nombre de Reynolds, qui gouverne les différentes structures d'écoulement, allant d'un régime symétrique à l'apparition d’une allée tourbillonnaire de Bénard–von Kármán. La traînée est ensuite déterminée par une approche indirecte, basée sur la mesure du champ de vitesse en aval et l'application des principes de conservation de la quantité de mouvement.

## Ecoulement autour d'un cylindre

Dans cette partie nous allons étudier l'écoulement de l'air autour et en aval d’un cylindre. A l'aide d'un tube de Pitot la vitesse de l’air est mesurée, on pourra également calculer la force de traînée qui agit sur le cylindre. L’écoulement autour du cylindre est influencé par le nombre de Reynolds $({Re})$, qui dépend de la vitesse de l'air $(U_{\infty})$, du diamètre du cylindre $(D)$ et de la viscosité du fluide $(\mu)$. Ce nombre est un indicateur clé pour savoir si l’écoulement est laminaire ou turbulent.

$$Re_{D} = \frac{\rho D U_{\infty}}{\mu} \tag{1}$$

Lorsque Re est faible (lorsque l'inertie du fluide est faible par rapport aux effets visqueux), l'écoulement est symétrique de part et d'autre du cylindre. Mais à mesure que Re augmente, l'écoulement devient de plus en plus instable, et on observe la formation de tourbillons dans le sillage du cylindre. À partir de $Re_{D} \geq 50$, ces tourbillons commencent à se détacher du cylindre à une fréquence régulière, créant une structure tourbillonnaire très spécifique, connue sous le nom d’« allée de Bénard–von Kármán » (Voir Figure \ref{fig:regime_laminaire}).

## Force et coefficient de traînée

Ces tourbillons créent des forces variables sur le cylindre, appelées forces de traînée, qui oscillent au rythme de l’émission des tourbillons. Bien que ces forces fluctuent dans le temps, l’ingénieur se concentre souvent sur la moyenne de ces forces, particulièrement pour la traînée, qui est la composante de la force agissant dans la direction de l’écoulement.

Formule du coefficient de trainée : 
$$C_{x} = \frac{T}{\frac{1}{2} \rho U^{2}_{\infty} D L} = f(Re_{D}) \tag{2}$$


## Mesure de la traînée

La traînée est la résistance opposée par le fluide à l’objet qui s’y déplace.

L’un des moyens les plus directs pour mesurer ces forces est d'utiliser une balance aéro-dynamique, mais ici, nous recourons à une méthode indirecte : en mesurant le champ de vitesse autour du cylindre avec un tube de Pitot, puis en appliquant le théorème de conservation de la quantité de mouvement pour estimer la force de traînée. 

On obtient ainsi l'équation reliant la trainée moyenne par unité de longueur de cylindre T aux valeurs des vitesses et pression moyenne aux frontières du domaine de contrôle :

$$T = -\int\int_{U^{4}_{i=1}S_{i}}\rho U_{x}(\vec{U}.\vec{n})dS - \int\int_{U^{4}_{i=1}S_{i}} \rho \vec{n}.\vec{e_{x}}dS \tag{3}$$


## Dispositif expérimental

La soufflerie utilisée dans ce TP est une soufflerie Eiffel à veine fermée et circuit ouvert, avec une section d’essai de 0,2 × 0,3 $m^{2}$. L’air est mis en mouvement par un ventilateur en aval, et la vitesse de l’écoulement (1 à 15 m/s) est contrôlée par un régulateur. 

Des cylindres de différents diamètres peuvent être fixés au centre de la veine d’essai. Un dispositif de visualisation par filets de fumée permet d'observer les trajectoires des particules fluides. 

Une sonde Pitot, reliée à un manomètre différentiel, permet de mesurer :

- la différence entre la pression d'arrêt (extrémité du cube) et la pression statique (corps du
 tube), utile pour mesurer la vitesse dans l'écoulement.
- la différence entre la pression atmosphérique et la pression statique, utile pour mesurer la pression statique dans l'écoulement.

Ce dispositif nous permettra ainsi de mesurer la traînée et d'analyser les résultats en fonction des paramètres d'écoulement.


Le sillage désigne la zone de perturbation laissée derrière un corps en mouvement dans un fluide, caractérisée par des tourbillons et des variations de pression. La traînée, quant à elle, correspond à la force résistante exercée par le fluide sur l’objet, influencée par la viscosité et les effets de turbulence. Comprendre ces phénomènes est essentiel en aérodynamique et en hydrodynamique pour optimiser les performances et réduire la résistance au déplacement.


# TP 4.5 Convection et effet d'ailettes


## Introduction

L'échange de chaleur entre un solide et un fluide environnant se fait principalement par convection. Ce transfert dépend de l'écoulement du fluide autour du solide et est caractérisé par un coefficient d'échange convectif $h$. 

L'objectif de ce TP est d'étudier la variation de $h$ en fonction de la vitesse d'écoulement autour d'une plaque rectangulaire horizontale, ainsi que l'effet des ailettes pour améliorer ces échanges thermiques. Ce principe est largement utilisé dans des systèmes comme les radiateurs de microprocesseurs ou les convecteurs domestiques.

## Concepts théoriques clés

- **Convection forcée** : Transfert thermique par un fluide en mouvement imposé (ventilation). Le flux thermique convectif est donné par :  
  $$
  \Phi_{cv} = h \cdot S \cdot \Delta T
  $$
  où $S$ est la surface d'échange et $\Delta T$ la différence de température entre le fluide et le solide.

- **Couche limite thermique** : Région proche de la paroi où la température évolue progressivement vers celle du fluide ambiant.

- **Nombre de Nusselt $Nu$** : Rapport entre transfert thermique par convection et par conduction, défini par :  
  $$
  Nu = \frac{h L}{k}
  $$
  où $L$ est une longueur caractéristique et $k$ la conductivité thermique du fluide.

- **Nombre de Reynolds $Re$** : Paramètre déterminant le régime d'écoulement (laminaire ou turbulent) :  
  $$
  Re = \frac{\rho U L}{\mu}
  $$
  où $\rho$ est la masse volumique du fluide, $U$ la vitesse d'écoulement, $L$ une longueur caractéristique et $\mu$ la viscosité dynamique du fluide.

- **Nombre de Prandtl $Pr$** : Rapport entre la diffusion thermique et la diffusion visqueuse, défini par :  
  $$
  Pr = \frac{\mu C_p}{k}
  $$
  où $C_p$ est la capacité calorifique du fluide.

Dans le cas d'une plaque plane en régime laminaire ($Re_L < 3 \cdot 10^5$), la relation entre ces nombres est :  
$$
Nu_L = 0.665 \cdot Re_L^{0.5} \cdot Pr^{1/3}
$$
Pour un écoulement turbulent ($Re_{T} > 5 \cdot 10^5 Pr > 0.5$) :  
$$
Nu_T = 0.035 \cdot Re_T^{4/5} \cdot Pr^{1/3}
$$

## Dispositif expérimental

L'étude est réalisée à l'aide d'un banc d'essai (voir Figure \ref{fig:dispositif}) permettant de générer un écoulement d'air autour de surfaces chauffées et d'en mesurer les effets thermiques. Le montage expérimental comprend :

- Un film chauffant (résistance électrique) pris en sandwich entre deux plaques de cuivre de $3.8$ cm de large, $6.4$ cm de long et $2$ mm d'épaisseur.
- Un tube en Plexiglas dans lequel circule l'air à différentes vitesses générées par un ventilateur.
- Une sonde à fil chaud permettant de mesurer la vitesse de l'écoulement.
- Une alimentation en courant continu avec affichage de la tension et du courant appliqués à la résistance chauffante.
- Un thermocouple de type K placé sur la plaque pour mesurer la température de surface.

Une deuxième configuration intègre une ailette en cuivre de 50 cm de long, 3 cm de large et 1 mm d'épaisseur, permettant d'analyser son impact sur l'amélioration des échanges thermiques.


## Conclusion

Les expériences menées ont permis d’analyser l’influence de la vitesse d’écoulement sur le coefficient d’échange convectif h et d’observer que h suit une loi en racine de Reynolds, conformément aux modèles théoriques. L’ajout d’ailettes s’est révélé efficace pour améliorer le transfert thermique, en augmentant la surface d’échange et en favorisant la dissipation de chaleur. La diminution de la longueur caractéristique avec l’augmentation de la vitesse confirme que le flux thermique est mieux réparti à grande vitesse. Enfin, les résultats expérimentaux sont cohérents avec les prédictions théoriques, validant ainsi les modèles utilisés.



# TP 4.6 Spectrophotométrie - Pyrométrie

## Introduction

La spectrophotométrie et la pyrométrie sont deux techniques essentielles en physique permettant d’analyser les interactions entre la lumière et la matière. La spectrophotométrie repose sur l’absorption et la transmission de la lumière par un échantillon afin d’en déduire des informations telles que la concentration d’une substance ou ses propriétés optiques. La pyrométrie, quant à elle, est une méthode permettant de mesurer la température d’un objet en analysant le rayonnement qu’il émet.


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

$L(\lambda ,T)= \epsilon (\lambda ,T) \cdot L_0(\lambda,T)$


On définit aussi une température de luminance $T_L$​, toujours inférieure à la température réelle du corps. Si $\epsilon$ est constant, le corps est dit "gris".

## Conclusion

Ce travail a permis d'explorer la spectrophotométrie et la pyrométrie pour analyser le rayonnement lumineux et mesurer la température. Les résultats obtenus par spectrophotométrie ont confirmé les caractéristiques des différentes sources lumineuses, tandis que les mesures pyrométriques ont validé la relation entre température et rayonnement. Les courbes de pyrométrie montrent une bonne cohérence avec la théorie, et l'utilisation d'un pyromètre bichromatique s'est révélée plus précise, car elle élimine l'influence de l'émissivité. En somme, ces techniques offrent une meilleure compréhension des phénomènes thermiques et des outils plus fiables pour mesurer la température.
