---
papersize: a4
lang: fr
secnumdepth: 3
toc-depth: 2
---


# Introduction

Ce TP porte sur l'étude d'une pompe à chaleur mécanique fonctionnant avec le fluide frigorigène R134a. L'objectif est d'analyser les cycles thermodynamiques théoriques et réels de cette pompe à chaleur à partir de mesures expérimentales de température et de pression. L'influence d'un échangeur de chaleur sur les performances du système sera également évaluée. Le TP permettra de comparer différents régimes de fonctionnement: à température de condensation fixée et à température d'évaporation fixée. L'accent sera mis sur l'analyse des puissances thermiques à l'évaporateur et au condenseur, ainsi que sur les puissances mécaniques et électriques au niveau du compresseur, en fonction des conditions de fonctionnement.


## Concepts théoriques clés

Les principales formules utilisées sont:

- Puissance au condenseur: $Q_{COND} = \dot{m}_{R134a} \cdot (h_2 - h_4)$
- Puissance à l'évaporateur: $Q_{EVAP} = \dot{m}_{R134a} \cdot (h_1 - h_4)$
- Puissance du compresseur: $W_{COMP} = \dot{m}_{R134a} \cdot (h_2 - h_1)$
- Rendement isentropique de compression: $\eta_{isen.} = \frac{(h_2 - h_1)_{isen.}}{(h_2 - h_1)_{rel}}$
- Puissance thermique via bilan enthalpique: $P_{enth} = \dot{m} \cdot c_p \cdot (θ_s - θ_e)$
- Coefficient de Performance en mode froid: $COP_{f} = \frac{P_{évap}}{P_{comp}}$
- Coefficient de Performance en mode chaud: $COP_{c} = \frac{P_{cond}}{P_{comp}}$
- COP de Carnot en mode froid: $COP_{f,C} = \frac{θ_{SF}}{θ_{SC} - θ_{SF}}$
​​- COP de Carnot en mode chaud: $COP_{c,C} = \frac{θ_{SC}}{θ_{SC} - θ_{SF}}$


## Dispositif expérimental

L'installation expérimentale se compose des éléments suivants:

- Un compresseur alternatif bi-cylindre entraîné par un moteur asynchrone
- Un condenseur à eau avec débit contrôlé et mesuré
- Un évaporateur alimenté par une résistance électrique
- Une vanne de détente réglée pour assurer 5°C de surchauffe en sortie évaporateur
- Un débitmètre pour le fluide R134a en phase liquide
- Un échangeur R134a/R134a optionnel permettant de sous-refroidir le liquide sortie condenseur et de surchauffer la vapeur sortie évaporateur

L'instrumentation comprend:

- 8 thermocouples de type K implantés à différents points du circuit
- Des manomètres haute pression (HP) et basse pression (BP)
- Un voltmètre et un ampèremètre pour mesurer les puissances électriques
- Un tachymètre pour déterminer le facteur de puissance du moteur électrique
- Une vanne trois voies permettant de faire fonctionner le système avec ou sans l'échangeur de chaleur

Cette installation permet d'étudier deux modes de fonctionnement principaux:

- En mode réfrigérateur: variation de la température d'évaporation à température de condensation fixe
-En mode pompe à chaleur: variation de la température de condensation à température d'évaporation fixe


# Expériences


# Conclusion

