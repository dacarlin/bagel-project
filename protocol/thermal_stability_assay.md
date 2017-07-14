# Assay to determine functional thermal stability of β-glucosidase mutants

This procedure is made to measure stability changes caused by mutations to BglB, which as a Tm of 40 C under these conditions. Therefore, we use a gradient of 30-50 C. In general, you can adjust the gradient of temperatures on the thermal cycler to center on the Tm of your protein. 

## Materials

Material | Concentration | Amount per sample
---------|---------------|------------------
Purified protein | about 1 mg/mL | 140 µL
2 mL tube | | 1
[substrate stock](stock_recipes.md) | 100 mM | 800 µL per plate
15 mL Falcon tube | | 1
assay plate | | 1
PCR plate | | 1
plate seal | | 1

## Mise en place

+ repeater pipet
+ P300 multichannel pipet and tips
+ thermal cycler
+ plate reader

## Method

### Dilute and thermal cycle proteins  

1. For each mutant, mix 140 µL of the purified protein and 1260 µL of protein buffer in a 2 mL tube
4. Aliquot 50 µL of diluted protein solution into PCR plate. Use three columns per mutant
5. Incubate PCR plate for 30 min in the thermal cycler with a gradient from 30 C to 50 C

### Prepare substrate plate 

6. Mix 800 µL of substrate solution and 7.2 mL of protein buffer in a 15 mL Falcon tube
3. Use a repeater or multichannel pipet to transfer 75 µL of diluted substrate into all 96 wells of the assay plate
6. Using a multichannel, transfer 25 µL of each well of the PCR plate to the corresponding well in the assay plate

### Assay and data analysis 

7. Monitor absorbance at 420 nm for 30–60 min using the plate reader and Gen5 software 
8. Verify statistical analysis of production formation rates ("MaxV" in units of OD/min in Gen5 software)
9. Record table of well indices (e.g., "A8"), rates (unit of OD/min), and sample names (e.g. "E164A") in the Google Doc 
10. Determine Tm from experimental data using the notebooks in `bagel-thermal` or the `bagel-fitter` 

## Notes 

+ Only measure the rate when product formation is linear with time (steady state)
