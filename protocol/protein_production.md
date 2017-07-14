# Production and purification of BglB

This is a guide to the production and purification of β-glucosidase B from *P. polymxa* beginning with purified plasmid and ending with purified protein. This protocol and the associated scripts and data in this repository are part of the [Siegel group](https://sites.google.com/site/ucdsiegellab/)'s "Bagel" project.

For this procedure, typical yields are 1.0 ± 0.4 mg/mL for the wild type protein.

Before beginning, make sure you have the following ready and standing by:

+ dry bath set to 42 C
+ 37 C standing, 37 C shaking, and 18 C shaking incubators
+ centrifuges for 50 mL Falcon tubes (up to 4,700 RPM) and 2 mL tubes (up to 14,700 RPM)

After you have designed your set of mutants, an automated Kunkel mutagenesis procedure will be carried out on [Transcriptic](https://www.transcriptic.com/)'s workcell. The wild type Bagel plasmid is mutated to your designed sequence using the procedure that's described in [Thomas Kunkel's original procedure](http://www.pnas.org/content/82/2/488.full.pdf) and in [our group's manual Kunkel protocol](https://docs.google.com/a/ucdavis.edu/folderview?usp=sharing&id=0B3zIXvOOrmpqcEM5WWRadThsVUE). If you're interested, there is  [Python code that automates the Kunkel procedure and algorithmicly evaluates sequence verification](https://github.com/dacarlin/gs-checker)

After your mutant plasmids have been sequenced, you'll get them in the mail ready for Day 1.

## Advice

*Mise en place* ("meez") is a [French culinary phrase](https://en.wikipedia.org/wiki/Mise_en_place) which means "putting in place", as in "set up". It means to organize and arrange the ingredients that a cook will require for a recipe. __Set up everything you need _before_ beginning each day's procedure.__

## Day 1: Transformation

In this step, you will transform the plasmids encoding your mutant genes into *Escherichia coli BL21(DE3)*. Transformation is the process of physically shocking the bacteria to induce them to take up foreign DNA from the environment. Today, you will heat shock the *E. coli* to induce the uptake of the plasmid encoding the mutant you designed.

Material | Concentration  | Amount per reaction | Amount for 4 mutants
---------|----------------|--------------------|-----------
Chemically-competent *Escherichia coli* BL21(DE3) | | 25 μL | 4 x 25 µL
Mutant plasmid solution | > 20 ng/μL | 1 μL | 4 x 1 µL
Terrific Broth (TB) | | 200 μL | 4 x 1 µL
LB agar plates with kanamycin | | 1 | 4
Sterile glass beads | | 5–10 |
14 mL round bottom  tubes | | 1 | 4

### _Mise en place_

+ waste bucket
+ P2 set to 1 µL
+ sterile tips for P2
+ P200 set to 200 µL
+ tube rack for 14 mL round-bottom tubes
+ ice bucket filled with fresh ice
+ dry bath pre-warmed to 42 ˚C
+ 37 ˚C shaking incubator with rack for 14 mL round bottom tubes
+ 37 ˚C standing incubator

### Instructions

1. Label the tubes, one for each mutant
1. For each mutant, dispense 1 µL of mutant plasmid into labeled 14 mL round bottom tube and set on ice
1. Incubate round-bottom tubes on ice for 2 minutes
2. While the tubes are chilling, thaw competent cells _on ice_ for 5 minutes
2. To each tube add 25 µL competent cells
3. Incubate on ice for 10 minutes
3. Heat shock at 42 C for 90 seconds
4. Incubate on ice for 90 seconds
5. To each tube, add 200 µL Terrific Broth and place in tube rack
6. Incubate tubes at 37 ˚C with shaking for 1 hour to allow cells to "recover"
6. Label the agar plates
7. After cells have recovered for 1 hour, add beads to each plate
6. Pipet 200 µL recovered cells on to plate and shake to spread out the cells
7. After waiting a minute so that the liquid is absorbed, turn the plates upside down so that the beads fall onto the underside of the lid, and deposit beads into bleach solution for later recovery
7. Incubate plate *upside down* overnight at 37 C

### Advice

+ Chemical competent cells should be kept on ice at all times and never warmed
+ Bring the ice bucket to the freezer
+ Longer recovery times (up to 2 hour) will improve transformation efficiency
+ Program the thermocycler to perform steps 1-5
+ Some tips for [troubleshooting transformations from New England Biolabs](https://www.neb.com/tools-and-resources/usage-guidelines/chemical-transformation-tips)
+ If you are getting poor transformation efficiency, try recovering with 400 µL of media for 2 hours at 37 C

## Day 2: Growth

Today, you will record the number of colonies on your selection plate and start a culture from a single colony.

Material | Amount per reaction | Amount for 4 mutants |
---------|---------------------|----------------------|
Transformation plate | 1       | 4
Terrific Broth       | 5 mL    | 25 mL
Kanamycin solution   | 5 μL    | 25 µL
Tube seal            | 1       | 4
50 mL Falcon tube    | 1       | 5

### _Mise en place_

+ waste bucket
+ rack for 50 mL Falcon tubes
+ tube seals, cut to size
+ P1000 set to 500 µL
+ P200 set to 25 µL
+ serological pipet aspirator
+ 25 mL serological pipet

### Instructions

1. Record the number of colonies on your transformation plate
1. Label tubes, one per mutant
2. To the left-over 50 mL Falcon tube, pipet 25 µL kanamycin
3. Add 25 mL TB and mix by pipeting up and down
4. For each mutant, aliquot 5 mL of TB/kanamycin mixture to labeled tube
1. For each mutant, inoculate labeled tube with a single colony. Using the P1000, carefully scrape a single colony from the plate, dip in the growth media in the Falcon tube, and pipet up and down a few times to inoculate the culture
5. Seal the cultures with tube seals (best to do this one by one as you inoculate)
6. Incubate tubes with shaking at 37 ˚C for 24 hours

### Advice

+ If you have a lot of colonies, divide the plate into quadrants, count one quadrant, and multiply the resultant number by 4 to estimate how many colonies you got
+ It's not necessary to use extremely careful sterile technique here, but the more sterile you can keep things the greater the likelihood that your experiment will go well

## Day 3: Expression cultures

In this step, you will exchange the spent growth media in your cultures with fresh growth media supplemented with [isopropyl β-D-1-thiogalactopyranoside](https://en.wikipedia.org/wiki/Isopropyl_β-D-1-thiogalactopyranoside) (IPTG). IPTG induces expression of your target protein [Molecular details of how the expression system works](http://www.genomics.agilent.com/article.jsp%3FpageId%3D472).

Material | Amount per reaction | Amount per 4 mutants |
---------|---------------------|----------------------|
Growth cultures from day 2 | 1 | 4
Terrific Broth | 5 mL          | 25 mL
IPTG solution | 5 μL           | 25 µL
Kanamycin solution | 5 μL      | 25 µL
Tube seal | 1                  | 4

_Minirecipe_: 5 mL induction medium = 5 mL Terrific Broth + 5 µL kanamycin solution + 5 µL IPTG solution

### *Mise en place*

+ tube rack
+ vortexer
+ P200 set to 25 µL
+ serological pipet aspirator
+ serological pipet tip, 25 mL
+ centrifuge set to 4,700 RPM for 10 minutes
+ shaking incubator (37 ˚C)

### Instructions

1. Centrifuge growth cultures at 4,700 RPM for 10 minutes
2. Peel the seals off and pour away supernatant from cell pellet
3. Weigh the pellet and record your pellet weight
4. Make a batch of induction media in sterile Falcon tube by adding 25 µL IPTG solution, 25 µL kanamycin solution, and 25 mL TB and mixing the three ingredients by pipeting up and down
1. Add 1 mL induction medium to cell pellet in each tube
1. Vortex to resuspend pellet
1. Add 4 mL more induction medium to tube
1. Seal with tube seals
1. Incubate with shaking at 18 ˚C for 24 hours

### Advice

+ Be as sterile as you can with these living cultures of cells
+ **Challenge**: Devise a clever way to simplify resuspension so that a robot could do it

## Day 4: Protein purification

Today, you will purify the protein you designed for testing using a technique called immobilized metal ion chromatography

Material | Amount per reaction         | Amount for 4 mutants
---------|-----------------------------|----------------------
Expression culture from day 3 | 5 mL   | 4
Wash buffer | ~ 5 mL                   | >5 mL
BugBuster | 50 μL                      | 250 µL
Dry lysis mix | 1 mg                   | 5 mg
2 mL tube | 1                          | 4
Protein buffer | 300 μL                | >1 mL
Ni-NTA resin slurry | 100 μL           | 400 µL

### _Mise en place_

+ centrifuge set to 4,700 RPM for 10 minutes
+ waste bucket
+ tube rack
+ flow-through collector
+ 1 mL protein purification columns
+ P1000 set to 500 µL
+ tips for P1000
+ tube rocker

## Instructions

1. Centrifuge expression cultures at 4,700 RPM for 10 minutes
2. While they are spinning, make lysis buffer and set on rocker. In a fresh tube, weigh 5 mg of dry lysis mix. Then, add 2250 µL wash buffer and 250 µL BugBuster  
3. Unseal cultures and pour away supernatant from cell pellet
4. Weigh your expression pellet and record the weight on the report sheet
4. Add 500 µL wash buffer to pellet and vortex to resuspend (should have about 1 mL in there)
5. Aliquot the resuspended pellets to fresh 2 mL tubes
1. Aliquot 500 µL lysis buffer into each resuspended pellet in 2 mL tube
1. Rock tubes for 30 minutes at room temperature
1. Centrifuge at 14,700 RPM for 30 minutes to clarify the lysate
1. While centrifuging, prep your columns. Set cleaned microcolumns (if necessary, rinse with water) in rack over waste collector
1. Add 100 µL Ni-NTA resin slurry to each column, making sure it settles in a nice bed on the bottom
1. Add 500 µL wash buffer and allow to drip through
1. Once the lysed cultures have finished spinning, check to make sure the lyaste is clear.
1. Load your proteins from clarified lysate to the column 500 µL at a time, allowing to drip through each time  
1. Wash each column six times with 500 µL of wash buffer, allow to drip through each time
1. Once all unwanted proteins have been washed away, transfer column to fresh tube
1. Add 150 µL protein buffer directly to beads and incubate at room temperature for five minutes
1. Add second 150 µL protein buffer and pulse in the centrifuge a couple of times to ensure you get all the liquid
1. The fresh tube contains your purified protein and can be stored at 4 ˚C for up to 48 hours
1. Wash out the columns

## Next steps

After your have purified your proteins, it's time to [determine your protein yield and purity](gel_and_yeilds.md) using UV spectroscopy and SDS-PAGE, then [determine your proteins' kinetic constants](kinetic_assay.md) and [melting temperature](thermal_stability_assay.md)
