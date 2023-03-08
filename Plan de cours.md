# Objectifs d'apprentissage
- Maîtriser la configuration et l'utilisation des appareils de mesure du laboratoire (multimètre, oscilloscope, générateur de signal et alimentation).
- Pouvoir reconnaître un composant et le caractériser.
- Pouvoir extraire d'une datasheet des informations pertinentes à la conception d'un circuit.
- Sur base d'un cahier de charges, pouvoir sélectionner les composants adéquats à la confection d'un circuit électronique.
- Identifier et expliquer le rôle des composants ou groupes de composants dans un circuit complexe.
- Comprendre les spécificités des différentes technologies vues en cours.
- Pouvoir réaliser en pratique un circuit électronique sur base d'un cahier des charges non-technique.
- Argumenter la place de l'électronique dans un monde durable.

# Sujets à aborder et plan général du cours d'électronique 3BM/3BS
Le cours comprend 27 heures, soit 18 * 1 h 30 réparties comme suit :
- 6 * 2 * 1 h 30 de cours
- 5 * 1 h 30 d'exercices
- 1 * 1 h 30 de Q&A
Chaque paire de cours devrait être suivie d'une séance d'exercices.

## Rappels généraux & Intro
- Électronique moderne, domaines et applications. Spécificités liées à l'EM et à la santé.
- Lois de Kirchhoff
- Composants usuels et relations constitutives (R/C/L)
- Symboles des composants usuels (R/C/L/sources/masse/gnd)
- Comment reconnaître un composant et sa valeur, comment retrouver sa datasheet ?
	- Illustration avec des circuits intégrés
	- Présenter les différents types de packages (DIP, TO-92, TO-220, normes JEDEC)
	- Lire R/C/L (codes couleurs et chiffré)
	- Activité : Donner quelques composants à identifier à des sous-groupes en auditoire. Avoir une base de données de photos permettant de trouver la bonne réponse. Wooclap ?

## Diodes
- Principe général, reconnaître composant et retrouver son identifiant.
- Caractéristique IV avec différents niveau d'idéalité, résolution d'un circuit avec une droite de charge.
- Circuits usuels :
	- Redresseur simple/double alternance
	- Démodulateur
	- Circuit logique
	- Clipping
- Fonctionnement général d'une jonction PN
- Différentes diodes et applications :
	- Zener (protection, fonctionnement en avalanche)
	- Schottky (Vth faible, rapide)
	- Varactor (condensateur contrôlé en tension)
	- Tunnel (caractéristique particulière)
	- Metal-Oxyde Varistor (caractéristique symétrique, contrôle de moteurs)
- Analyse de datasheet, lecture et extraction des informations importantes.
- Photodiode/LED

## Amplificateur opérationnel
- Rappels de base :
	- Notion de gain (gain boucle ouverte/fermée)
	- Montage différentiel
	- Illustration de l'effet de la rétroaction négative expliquant le zéro virtuel
	- Résolution d'un montage inverseur/non-inverseur
- Montages usuels
- Imperfections et compensation (exemple de l'offset du LM741)
- Ampli d'instrumentation (différences et particularités)
- CMRR
- Applications et utilisations :
	- Amplification
	- Adaptation d'impédance
	- Filtre actif
	- Résistance négative (https://en.wikipedia.org/wiki/Negative_resistance)
	- Redresseur de précision
- Oscillateur (brièvement, fonctionnement du 555).


## Transistors
- Introduction générale au comportement et forme des caractéristiques IV
- Différents niveaux d'analyse : polarisation et petits signaux

### BJT
- Caractéristiques (transfert et sortie)
- Différence entre NPN et PNP
- Polarisation
- Petits signaux
- Circuits usuels et applications *modernes*

### MOSFET
- Caractéristiques (transfert et sortie)
- Différence entre NMOS et PMOS
- Polarisation
- Petits signaux
- Circuits usuels et applications


## Interfaçage analogique-numérique

### ADC
- Flash
- Semi-flash
- Stairstep-ramp
- Single slope
- Dual slope
- Approximations successives
- Pipeline
- Delta-Sigma

### DAC
- Chaîne de résistances
- R-2R
- Delta-Sigma

### Erreurs de conversion
- Quantification
- Offset
- Gain
- Non-linéarité


## Capteurs et bus de communication
- SPI/I2C/UART
- Comment lire une datasheet de capteur ? À quoi faut-il faire attention ?
- Capteurs intéressants qui n'ont pas encore été vus ?


## Sustainability
- Matériaux nécessaires et terres rares, illustration avec la composition d'un smartphone. Donner des pistes d'alternatives
- Effet rebond et effet parc, illustrer avec la consommation des circuits intégrés
- Analyse de cycle de vie de plusieurs éléments de base
- Analyse d'impact sur la biodiversité
- Bonnes pratiques pour améliorer la durabilité d'un projet d'électronique, par exemple :
	- Est-il nécessaire ? Peut-on adopter une alternative low-tech ?
	- Sourcer correctement ses composants (matériaux, localisation, etc.)
	- Réfléchir à la fin de vie du produit


## Hands-on -> À déplacer dans l'intro du cours ?
- Sécurité (essentiellement des composants, décharge électrostatique)
- Appareils de mesure (multimètre/oscillo en vitesse)
- Matériel d'électronique :
	- Connecteurs
	- Appareils
	- Matériel de brasage
	- Logiciels d'EDA (conception/simulation)
	- Simulation SPICE (expliquer le principe et l'existence)


# Séances d'exercices

1. Circuits de base & diodes
2. AOP
3. BJT
4. MOSFET
5. ADC/DAC/Capteurs

# Laboratoires
4 * 3 h 30 de laboratoire.

1. **À changer** Circuit(s) avec AOP/Diode et lecture de datasheet. Éviter les manipulations « recette de cuisine » ou « plan IKEA ».
Ramener le 555 dans cette manipulation, mais revoir l'approche (musique, clignoter LED ?). Il sera vu au cours dans le chapitre AOP.
2. Contrôle de lampe, **à garder**
3. Manipulation avec des BJT et MOSTFET purs pour illustrer leur comportement, l'importance de la polarisation et des petits signaux.
4. Examen