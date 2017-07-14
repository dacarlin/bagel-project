# Assay to determine kinetic parameters of β-glucosidase B

This assay assumes that you have followed the protein production and purification steps in `production.md` in this repository.

## _Mise en place_

+ waste bucket
+ pipet reservoir basin
+ P200 and tips
+ Multi-channel P50 and tips
+ Multi-channel P300 and tips

## Software

+ purified protein from day 4
+ substrate stock (you will need 2 mL)
+ protein buffer
+ 2 mL tubes
+ 1 strip of PCR tubes

## Instructions

### Before you begin

1. Prepare your <em>mise en place</em>: put everything in place
1. Thaw your substrate stock and vortex if necessary until completely clear (no precipitate), it may look a little bit yellow due to background pNPG hydrolysis, this is normal

**Advice:** Read through twice before beginning. Take a deep breath. Focus.

### Perform a qualitative test of enzyme activity for each sample

1. In a PCR strip, aliquot 9 µL of substrate stock, 1 well per mutant
1. Aliquot 1 µL of each mutant, 1 well per mutant
3. Incubate at room temperature for 5 minutes
3. **If the sample turns yellow**:
   + make a 1/100 dilution
   + in a fresh tube mix 10 μL purified protein and 990 μL wash buffer
4. **Else**:
   + make a 1/10 dilution
   + in a fresh tube mix 100 μL purified protein and 900 μL wash buffer

Use the diluted purified protein for the remainder of the procedure. The undiluted stock can be used to run a gel and quantitate protein concentration by A280.

### Prepare a substrate plate

First, make the substrate plate. For this mixing step, use a PCR plate.

Pour some protein buffer into a reservoir before you start.

1. Using a single-channel pipet, dispense 150 μL of substrate stock into row A (12 wells)
2. Using a multi-channel pipet, dispense 112.5 μL of protein buffer into rows B, C, D, E, F, G, H (84 wells)
1. Using the multi-channel pipet, remove 37.5 μL from the first row and add to second row, and mix three times
3. Repeat this procedure for the second, third, forth, fifth, and sixth rows
4. Remove 37.5 uL from the seventh row, and throw away the liquid with the tips. Do not touch the last row in this step
6. Verify that every well in the plate is the same volume (112.5 µL)

### Prepare a protein plate

Now that you have created the gradient of substrate concentrations in the PCR plate, aliquot your proteins into the assay plate. This is the plate that will be going into the plate reader.

1. For each mutant, aliquot 25 µL of **diluted** purified protein into three columns of the plate (24 wells)

### Initiate assay

To initiate the assay, transfer 75 µL from each well in the substrate plate into the assay plate containing your aliquotted protein. Before you begin the instructions below, set the plate reader to monitor absorbance at 420 nm every minute for 60 minutes.

1.  Using the multichannel pipet, transfer 75 µL from the bottom row of the substrate plate into the bottom row of the assay plate
2.  Repeat for the rest of the rows (bottom up)
3.  Place the plate on the prepared plate reader and press Enter (run time: 1 hour)

### Record your data

4.  Fill out the "Information" panel for the plate in the Gen5 software with your name, the mutants you are testing, and the dilutions that you used. Use this format:

> Alex. Cols 1-3: WT @ 100X, cols 4-6: E164A @ 10X, 7-9: I300L @ 100X, cols 10-12: E353A @ 10X

### Data analysis

2. Once the assay has finished, remove your plate and examine your data. **Note**: make sure that the Gen5 is set to calculate rates based on at least 10 points, and that the rates are reported in units of OD/min. These settings can be found under "Data Reduction > Calculation Options"
3. Visually check and assess R-squared values for the 96 individual rates calculated in the assay. There is one per well. R-squared values closer to 1 are better. Mask points as necessary to compensate for detector limit (it can't read above OD 3.75) as well as correct erroneous rates resulting from detector noise (such as pNP formation rates that are negative)
4. Use the [web app for fitting your data to the Michelis-Menten model of enzyme kinetics](http://bagel.genomecenter.ucdavis.edu). Instructions for interpreting assay data can be found in the file `data_reporting_guidelines.md`
8. Enter the assay data in the `kinetic_data` sheet of the report
