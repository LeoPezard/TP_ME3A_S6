---
title : Compte rendu TP Mécanique Energétique - Conduction Thermique
author : > 
    Baptiste Fanget - Pezard Léo - ME3A
---

# Préambule

## coucou

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
   $P_{fluide}$ = $\dot{m}C_{p}$ ($T_{sortie}$ - $T_{entrée}$)  
  où $\dot{m}$ = $\rho q$ (kg/s).

---

### Loi de Fourier
- Flux d'énergie interne en conduction thermique :  $\Phi_{x}$ = -k S $\frac{dT}{dx}$
 - $\Phi_{x}$ : flux (W).
  - $k$ : conductivité thermique (W/m·K).
  - $S$ : section (m²).
  - $\phi_{x} = \frac{\Phi_{x}}{S}$ : densité de flux (W/m²).

---


## Travail préparatoire
Réalisé sur Amétice

Notions importantes abordées :

# Travail à effectuer 

## A l'arrivée en séance

Lors de cette séance, nous avons tout d'abord vérifié que le régime était stationnaire, en nous assurant que les températures et les puissances mesurées étaient constantes.

Les données suivantes ont été relevées : 
- la tension _U_ et le courant _I_ aux bornes du collier chauffant
- le débit volumique d'eau dans la boîte à eau
- les températures de l'eau à l'entrée et à la sortie de la boîte, via le logiciel. 

Ensuite, les températures relevées par les 10 thermocouples positionnés entre le collier chauffant et la boîte à eau ont été enregistrées. 

Après validation par l'enseignant, la phase instationnaire a été initiée en augmentant la tension d'alimentation du collier chauffant de 65V à 110V, tout en prenant note de l'heure de ce changement. La séance s'est conclue par l'arrêt des acquisitions et le début des simulations numériques sous Excel pour exploiter les données collectées.

## Régime instationnaire - Simulations


