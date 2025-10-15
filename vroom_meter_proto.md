# Vroom meter
```
  _   __                      __  ___    __         
 | | / /______  ___  __ _    /  |/  /__ / /____ ____
 | |/ / __/ _ \/ _ \/  ' \  / /|_/ / -_) __/ -_) __/
 |___/_/  \___/\___/_/_/_/ /_/  /_/\__/\__/\__/_/   
```
                                                    

## Proto numéro 1:

L'objectif de ce prototype est de tester une puce gps. Dans un premier temps,
afin de comprendre comment fonctionne la puce et les données que l'on peut en
tirer. Dans un second temps, pour tester le fonctionnement du rtk.
Ce prototype n'est pas a destination de mesures dynamiques, c'est-à-dire que le
temps caractéristique de la mesure d'un déplacement ne seras pas inférieur à
1s.
L'ensemble des manipulations de données seront fais "à la main".

Questions:
 - Quelle puce choisir ? Antenne ? 
    - Puce: ublox NEO-M8Q-(01A)
    - Antenne active cf. Max
 - Quel dispositf porteur choisir (Ordinateur, téléphone, ...) ?
    - Pour ce prototype le but n'est pas d'implémenter tout sur l'esp seulement
      de tester le post traitement des données.
 - Comment mettre en place le rtk ?
    - RTK lib sur le pc dans un script C

Diagrame du foncitonnement du proto:

GNSS (ublox neo) -> PC -> base RTK -> PC et RTK lib -> données traitées

## Prototype numéro 2 

L'objectif de ce prototype est de tenter une première approche embarqué du
logiciel. 

Objectifs:
 - Automatisation de la configuration. 
 - Mise en place d'une procédure de mesure.
