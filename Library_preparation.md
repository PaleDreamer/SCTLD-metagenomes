# Library preparation for enriched coral microbiome DNA
This protocol has been adapted from the NEB protocol for Illumina NGS library preparation: 

https://www.neb.com/protocols/2017/10/25/protocol-for-fs-dna-library-prep-kit-e7805-e6177-with-inputs-greater-than-or-equal--to-100-ng

The protocol consists of 5 steps. Safe stopping points will be **indicated**. 

### Fragmentation
##### *Remove yellow tubes from the freezer boxes and place in ice box and Crosslink PCR tubes for 2 min, 2x the amount of samples*

1. Pipette the reaction buffer up and down after thawing & vortex the FS exzyme mix 5-8 seconds before use. 
2. Add 26 µl of enriched microbial DNA from each sample 
3. Add 7 µl of NEBNext Ultra II FS Reaction Buffer to each tube
3. Add 1 µl of NEBNext Ultra II FS Enzyme Mix
4. Total volume ~34 µl
5. Vortext for 5 sec and breifly spin down in microcentrifuge
6. Run the following program in the thermocycler
   -  Lid heated to 75 ºC
   -  5 min at 37 ºC
   -  30 min at 65 ºC
   -  Hold at 4 ºC 


### Adaptor ligation
##### *Remove red tubes from the freezer boxes and place in ice box until needed*

1. In each tube add 30 µl of NEBNext Ultra II Ligation Master Mix (Pipette ligation master mix up and down prior to use)
2. Add 1 µl of NEBNext Ligation Enhancer
3. Add 2.5 µl of NEBNext Adaptor for Illumina
4. Pipette the mixture up and down (at least 10x) to mix thoroughly
5. Incubate at 20 ºC for 15 min in the thermocycler with the heated lid off (set total volume to 50 µl)
6. Add 3 µl of USER® Enzyme
7. Mix well and incubate at 37 ºC for 15 minutes with the lid heated to ≥ 47 ºC (set total volume to 50 µl)
 

### Size Selection of Adaptor-ligated DNA for DNA Input > 100 ng.
1. Bring your mixture to 100µl by adding 29.5 µl of 0.1X TE (1X TE Buffer in 1:10 in water)
2. Vortex your AmPureXP beads and add 20 µl of AmPureXP beads to the mix
3. Pipette up and down to homogenize 
4. Incubate at room temperature for at least 5 min 
5. Place tubes on magnetic stand and wait until solution is clear (~5 min)
6. Transfer supernatant (~140 µl) to a new tube (discard beads)
7. Add 10 µl of AmPureXP beads to the sample and pipette up and down at least 10x
8. Incubate on the benchtop for 5 min 
9. Place on magnetic stand (~5 min, or until clear)
10. Carefully remove the supernatant and discard 
11. Add 200 µl of 80% ethanol to the tube in the magnetic stand
12. Incubate for 30 seconds then carefully discard the supernatant
13. Add 200 µl of 80% ethanol to the tube in the magnetic stand
12. Incubate for 30 seconds then carefully discard the supernatant (Remove ALL ethanol here)
13. Air dry the beads for *up to* 5 min while on the magnetic stand 
14. Remove from magnetic stand and elute DNA with 17 µl of 0.1X TE buffer
15. Pipette up and down 10x to mix well & incubate at room temperature for 2 minutes
16. Place in magnetic stand (~5 min, or until clear)
17. Transfer 15 µl to a new PCR tube 

***Samples can be stored overnight at -20°C.*** 


### PCR Enrichment of Adaptor-ligated DNA

##### *Using the forward and reverse primers that are already combined protocol*
###### These steps are using the blue set of reagents

1. Add 25 µl of NEBNext Ultra II Q5 Master Mix to the tube with your Adaptor Ligated DNA Fragments
2. Add 10 µl of Index/Universal Primer 
3. Total volume 50 µl 
4. Use a pipette to mix the solution about 10x 
5. Run the following protocol in the thermocycler 
   -  30 sec at 98 ºC
   -  10 seconds at 98 ºC
   -  75 seconds at 65 ºC
   -  Add GO TO --> step 2 (5 reps)
   -  5 min at 65 ºC 
   -  Hold at 4 ºC
   

### Cleanup of PCR reaction 

```diff
# Note: The volumes of SPRIselect or NEBNext Sample Purification Beads provided here are for use with the sample contained in the exact buffer at this step. AMPure XP beads can be used as well. If using AMPure XP beads, allow the beads to warm to room temperature for at least 30 minutes before use. These volumes may not work properly for a cleanup at a different step in the workflow. For cleanups of samples contained in different buffer conditions, the volumes may need to be experimentally determined. in gray
```
1. Vortex AmPureXP beads and add 45 µl to the PCR product (Mix well by pipetting ~10x)
2. Incubate on the bench for 5 min 
3. Place on magnetic stand and wait until clear (~5 min)
4. Remove and discard supernatant 
5. Add 200 µl of 80% ethanol to the tube in the stand 
6. Incubate on the benchtop for 30 seconds
7. Remove and discard supernatant 
8. (Repeat) Add 200 µl of 80% ethanol to the tube in the stand 
6. Incubate on the benchtop for 30 seconds
7. Remove and discard supernatant (Remove all visible EtOH here)
8. Air dry beads for *up to* 5 min while on the magnetic stand
9. Elute DNA by adding 33 µl of 0.1X TE buffer 
10. Mix well by pipetting up and down 10x 
11. Place in magnetic stand (~5 min, or until clear)
12. Transfer 30 µl to a new PCR tube 
  
  ***In this step you can store at -20 ºC or continue with the protocol***
   


### Assess Library Quality on a Bioanalyzer or TapeStation 
##### IF NEEDED 
###### This is using the Aligent High Sensitivity D1000 ScreenTape Quick Guide for TapeStation Systems

1. Allow tape station reagents to equillibrate at room temp for 30 minutes prior to use
2. Launch Aligent TapeStation Controller Software
3. Flick the High Sensitivity D1000 ScreenTape device and insert into nest of TapeStation 
4. Select sample positions on the computer
5. Refill any consumables required by the station (pipette tips)
6. Vortex and spin down reagents and samples 
7. Add 2 µl High Sensitivity Sample Buffer and 2 µl of High Sensitivity D1000 ladder at the A1 position 
8. For each sample add 2 µl of High Sensitivity Sample Buffer and 2 µl of sample DNA
9. Vortex samples at 2000 rpm for 1 minute
10. Briefly spin down tube strip 
11. Load into TapeStation, remove caps, and hit start

  ***Note that the ladder is in the inner most position of the machine***











