---
papersize: a4
lang: fr 
secnumdepth: 3
---


# Introduction et principes généraux

La mesure de la vitesse des fluides est essentielle en mécanique des fluides pour mieux comprendre les phénomènes d'écoulement. Parmi les méthodes optiques disponibles, la vélocimétrie laser Doppler (LDV), développée dès 1964, est l’une des plus répandues en recherche et en industrie. Elle repose sur l’utilisation de particules traceuses en suspension dans un fluide transparent, permettant une mesure locale non intrusive des vitesses, allant de quelques m/s à plusieurs centaines de m/s. L’objectif de ce TP est de se familiariser avec les bases expérimentales de cette méthode.

## Présentation du banc de vélocimétrie laser

Le banc utilisé est composé d’un ensemble optique et électronique permettant de générer, focaliser et analyser des faisceaux lasers. Il inclut une diode laser verte, des éléments optiques pour diviser et orienter le faisceau, un disque tournant servant de support de particules, et un détecteur optoélectronique relié à un oscilloscope pour visualiser le signal. Ce dispositif permet de mettre en œuvre un anémomètre laser Doppler (ALD).

## Consignes de sécurité liées à l’utilisation du laser

Le laser utilisé étant de classe IIIb, des précautions strictes doivent être respectées pour éviter tout dommage oculaire. Le port de lunettes de protection adaptées est obligatoire. Il est également recommandé de :

- éviter toute exposition directe ou réflexions du faisceau,

- garder une distance suffisante (plus de 20 cm),

- ne pas aligner les yeux avec la hauteur du faisceau,

- retirer les objets réfléchissants comme montres ou bijoux.

## Principe physique : effet Doppler optique

Le fondement théorique de la LDV repose sur l’effet Doppler : une particule en mouvement modifie la fréquence de la lumière qu’elle réfléchit. La fréquence détectée dépend de la vitesse de la particule et de la géométrie du dispositif. Toutefois, comme la fréquence optique est très élevée ($\approx 10^{14}$ Hz), une mesure directe est impossible. Pour pallier cela, une méthode à franges d’interférences est utilisée.

## Principe de la vélocimétrie à franges

Deux faisceaux laser cohérents se croisent dans un volume de mesure, créant un réseau de franges stationnaires. Lorsqu’une particule traverse ce réseau, elle diffuse un signal lumineux modulé dont la fréquence dépend de sa vitesse perpendiculaire aux franges. Cette méthode permet une mesure précise, indépendante de l’orientation du détecteur, ce qui constitue un avantage majeur.

## Dispositif expérimental utilisé

Le système CA-1350 permet de reproduire le principe du LDV en laboratoire. Le faisceau laser est scindé en deux à l’aide d’un séparateur optique, puis recombiné après passage par une lentille pour créer un volume d’interférences. Un disque acrylique rotatif, sur lequel sont fixées des particules de poussière, traverse ce volume. La lumière diffusée est captée, convertie en signal électrique, puis analysée sur un oscilloscope pour en extraire la fréquence de modulation, donc la vitesse.

## Observation des franges d’interférence

Avant de passer aux mesures, une phase de familiarisation avec les franges est proposée sur un banc optique annexe, utilisant un laser rouge à 635 nm. Un disque de verre gravé de trois réseaux différents permet d’observer plusieurs interfranges en variant le pas du réseau. Cette observation se fait sans déplacer la platine, selon des consignes de sécurité strictes.

# Expériences

## Mise en place du module de convergence des faisceaux

### Lentille de mise en faisceaux parallèles

On choisit la lentille numéro 1 

## Mesure de la vitesse du son dans l'air

### Calcul de la vitesse du son 


Le montage réalisé est composé d'un générateur 40kHz, d'un émetteur et récepteur (transducteurs ultrasonores) et enfin d'un oscilloscope pour visualiser les signaux d'émission et de réception. 

Ainsi on peut observer l'évolution du signal d'émission en fonction de la distance.

![Distance en fonction du temps](celerité.png){#fig:celerité}


On observe une courbe affine, le coefficent directeur de cette droite permet de calculer la vitesse expérimentale du son dans l'air. 

On a donc dans notre cas une vitesse du son d'environ $\boxed{324,11 \text{ m/sec}}$

On note ici que la température de la pièce est de 20,5°C

On sait que la vitesse du son dans l'air pour une température de 20°C est de 340 m/s.
On a donc un erreur relative de $\frac{|324-340|}{340} = 0.047$ Soit 4,7% d'erreur.

Cette erreur peut provenir de la température de la pièce qui n'est pas exactement à 20°C mais également de l'interprétation graphique de $\Delta t$ en fonction de la distance ainsi que de la précision des curseurs sur l'oscilloscope.

### Echantillon intercalé entre l'émetteur et le récepteur

Lorsqu'on intercalle des échantillons entre l'émetteur et le récepteur, on observe une diminution de l'amplitude du signal reçu.

En effet lorsqu'il n'y a pas d'objet entre l'émetteur et le récepteur, l'intensité du signal reçu est différente de lorsqu'il y a un échantillon :

|Echantillon | $\Delta E (V)$| Atténuation (%) |
|:---:|:---:|:---:|
|Sans échantillon | 136| 0 |
|Faux plafond | 36 | 73,5 |
|MDF | 30| 77,9 | 77,9 |
|Mousse absorbante | 38 | 72,1 |
| MDF + mousse absorbante | 12 | 91,2 |


L’atténuation du signal peut être due à l’absorption, la réflexion, la diffusion, ou la transmission partielle à travers les matériaux.

Les matériaux comme le MDF (panneau de fibres de bois) ont probablement une forte capacité à bloquer ou réfléchir les ondes.

La mousse absorbante est conçue pour absorber les ondes, notamment dans les domaines acoustiques ou électromagnétiques.

Ensemble, MDF + mousse absorbante combinent leurs propriétés, ce qui explique la très faible amplitude du signal reçu. C'est donc le moyen le plus efficace pour atténuer le son.


## Niveaux acoustiques, atténuation, traitement du signal

![Schéma simplifié du montage du TP](montage.png)


### Démarrage / Calibration

Grâce au fichier calibration sur python le bruit blanc est d'amplitude 80 dB. Nous pourrons par la suite étudier l'effet de différents matériaux pour atténuer ce son.


### Effet du caisson

Nous pouvons interprêter l'effet du caisson sur le bruit blanc. On observe une amplitude de 68,8 dB donc une réduction de l'amplitude de de 11,2 dB par rapport au bruit blanc "normal". On sait que tous les 3dB le son est perçu deux fois plus fort ou inversement. Avec le caisson, le son est donc perçu 4 fois moins fort que sans les parois.

Ainsi le caisson est très efficace car il réduit très fortement le niveau sonore perçu à l'extérieur, cela s'explique également par la présence de mousse absorbante sur l'ensemble des parois.


### Effet d'une paroi isolante

On place différents matériaux entre l'enceinte et le micro.

| Matériau                  | Niveau sonore (dB) | Atténuation (dB) |
|:-------------------------:|:------------------:|:----------------:|
| white noise - caisson     | 68,8            | -- |
| faux plafond              | 63,2             |5,6 |
| laine de roche            | 65,8             | 3 |
| MDF                       | 61,8             | 7 |
| MDF - mousse              | 58,4             | 10,4 |
| mousse - MDF              | 61,5             | 7,3 |
| plexiglass                | 58,8             | 10 |


Ces mesures montrent que tous les matériaux testés atténuent le niveau sonore par rapport à la référence sans obstacle (68,8 dB), mais avec des degrés d’efficacité variables. Les combinaisons de matériaux, notamment MDF - mousse (10,4 dB) et plexiglas (10 dB), offrent les meilleures performances d’atténuation, soulignant l’intérêt de combiner absorption (mousse) et réflexion (matériau dense). L’ordre des couches a aussi un impact : placer la mousse du côté de la source sonore améliore l’efficacité. En revanche, des matériaux comme la laine de roche ou le faux plafond sont moins performants seuls, ce qui peut s’expliquer par leur moindre densité ou leur capacité d’absorption limitée dans cette configuration.

### Effet d'une paroi copmposée


| Matériau                  | Niveau sonore (dB) |Atténuation (dB) |
|:-------------------------:|:------------------:|:----------------:|
| MDF gris              | 57,4             | 11,4 |
| MDF gris + porte      | 65,8             | 3 |
| MDF gris sans porte   | 65,0             |  3,8 |

On sait que les dimensions de la porte sont de 10,5cm par 19cm soit $0,02 m^{2}$ et que la surface de la plaque est de  $0,27 m^{2}$.

On peut calculer la résistance acoustique du matériau avec la formule :

$$ \Sigma_i S_i \cdot 10^{-R_i/10} = S_T \cdot 10^{-R/10}$$

où $R_i$ est la résistance acoustique du matériau, $S_T$ est la surface totale des matériaux, et $S_i$ est la surface d'un matériau.

On a donc ici $S_T = 0,27 m^{2}$, $S_{porte} = 0,02 m^{2}$, $S_{sans porte} = 0,25 m^{2}$, $R_{MDF + porte} = 3 dB$, $R_{MDF} = 11,4 dB$ et $R_{MDF sans porte} = 3,8 dB$

Ainsi :

$$ 0,27 \cdot 10^{-3/10} = 0,25 \cdot 10^{-3,8/10} + 0,02 \cdot 10^{-R_{bois}/10}$$
$$ \Rightarrow R_{bois} = -10\cdot \log(\frac{0,27 \cdot 10^{-3/10} - 0,25 \cdot 10^{-3,8/10}}{0,02}) \approx -1,9 dB$$

On prend 1,9 dB car ce n'est pas cohérent d'avoir une valeur négative.


# Conclusion

Ce TP a permis d’explorer de manière expérimentale les propriétés physiques des ondes sonores et les phénomènes associés à leur propagation, leur atténuation et leur analyse spectrale. À travers différentes expériences, nous avons mesuré la vitesse du son dans l’air avec une bonne précision (4,7 % d’erreur), puis étudié comment divers matériaux influencent l’intensité du signal reçu.

Nous avons montré que certains matériaux comme le MDF ou le plexiglas, seuls ou combinés à de la mousse absorbante, atténuent fortement les ondes sonores, notamment grâce à leurs propriétés de réflexion et d’absorption. L’ordre des couches dans une paroi composite s’est révélé déterminant dans l’efficacité de l’atténuation. Enfin, l’analyse d’un caisson insonorisé a confirmé l’impact significatif d’une bonne isolation acoustique. Ce TP met ainsi en évidence l’importance du choix des matériaux et de leur agencement pour le contrôle des nuisances sonores.
