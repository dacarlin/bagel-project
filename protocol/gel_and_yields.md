# SDS-PAGE

This document contains instructions for sodium dodecyl sulfate polyacrylamide gel electrophoresis (SDS-PAGE) for determination of protein yield and purity. You will run a gel after you have purified your proteins, either on Day 4 or Day 5. See the [protein production and purification procedure](https://github.com/dacarlin/bagel-protocol/blob/master/protein_production.md) for the procedure preceding this one.

## Materials

Material | Amount per sample
-------------|-----------
Purified protein | 12 µL
4x loading dye (Lamelli sample buffer with β-mercaptoethanol | 4 µL
PCR tube | 1

Material | Amount per gel
----------|------------
Protein gel | 1
BioRad Kaleidoscope Ladder | 8 µL
20x MES running buffer | 25 mL
Coomassie Blue protein gel stain | 10 mL

## Hardware

+ 500 mL graduated cylinder
+ gel box and clamp  
+ gel power box

## Procedure

1. **Prepare samples**. Pipet 4 µL of 4x concentrate loading dye in each labeled PCR tube
2. Pipet 12 µL of protein into each PCR tube. Pipet up and down slowly to mix well
3. Heat to 95 C for 10 minutes in thermocycler
4. **Prepare protein gel and electrophoresis apparatus**. Remove the comb from the well on top of the gel, and remove the tape from the back.
5. Assemble gel electrophoresis apparatus. Lock in gel, also assemble electrodes: red to red, black to black.
6. Create 1x MES Buffer Solution from 20X stock. To make 500 mL, mix 25 mL 20X MES buffer and 475 mL MilliQ water in a graduated cylinder.
7. Pour 1X Buffer Solution into gel electrophoresis apparatus to cover the gel
8. **Load the protein standard and samples**. Load 6 µL of BioRad Keleidoscope protein standard into one well
9. Load 12 µL of the heated, dyed protein into gel wells (make sure to note the which protein is in which well)
10. **Run the gel**. Set machine for 165 Volts and 400 milliamps for 35 minutes
12. After 35 minutes, remove the gel from the apparatus.
13. Carefully crack open plastic around gel and slide gel into Tupperware filled with deionized water.
14. Rinse with water once or twice.
15. Pour away all the water and pour in just enough Comassie Blue gel strain to barely submerge gel (10 mL or so)
14. Shake stained gel for 1 hour (overnight is OK too)
15. Pour off stain and refill Tupperware with deionized water to destain the gel
16. Shake gel 12+ hours (overnight is OK too)
17. **Take a gel image**. Get plate reader ready. Wash off the white gel plate with deionized water and dry with kim wipes
19. Remove gel from the water and plate in the center of the white tray
20. Read image using BioRad ImageLab software
21. **Annotate gel lanes with protein and ladder labels**.
21. Save your data in the "Gels" directory with your name and the date in the title

## Advice

+ Observe lots of small bubbles streaming from the electrode: this indicates that the gel is running properly
+ If you are running more than one gel it is a good idea to load the ladder into different positions in each gel to make distinguishing between them easier

# Quantitation of protein yield by A280

## Software

+ eluted protein samples
+ protein storage buffer

## Hardware

+ plate reader
+ Take3 micro-well plate

## Mise en place

+ P10 and tips
+ waste bucket

## Instructions

1. Aliquot 2 µL protein storage buffer to first well
1. For each of your samples, transfer 2 µL to the next well
1. Read using Gen5 program "Protein A280"

## Advice 

+ high background reads are bad
+ cross-check with the gel to make sure that the yield makes sense before reporting it
+ a typical yield for wild type BglB is 1.0 mg/mL
