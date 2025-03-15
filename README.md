# TSE

Time-Series cultivar coefficient Estimator for DSSAT models.

* Starting with DSSAT 4.8.5 official release available at: "https://dssat.net/" the TSE (version 2.4) is included in the DSSAT shell, in the section "Accessories".

* From now on "TSE.exe" has generic name without version number being included in the name, due to path setup required for running TSE from within DSSAT shell "Accessories" section.

* PC Antivirus Exception should be given to "TSE.exe"!

In order to check what version of TSE you are running, start TSE from within DSSAT shell "Accessories" section and on top of TSE interface window TSE version is written!

If you are running the TSE from DSSAT shell "Accessories" section and get Error or, it looks like the TSE is not optimizing coefficients, then download "TSE.zip" (file zipped) from this GitHub repository (which is currently TSE version 4.2).

Before continuing with next step make a copy of TSE directory available in "C:\DSSAT48\Tools" that you can restore, if something goes wrong.

After downloading "TSE.zip" and unzipping it on your PC, copy the content of TSE folder to the "C:\DSSAT48\Tools\TSE" directory (including: "TSE.exe", "yes.ico", "no.ico, "TSE.ico", "PhenologicalEventsDAP.txt" and "ParameterProperty.txt").

After adding the files to the TSE directory, the file path should look like this: "C:\DSSAT48\Tools\TSE\TSE.exe".

If the steps are implemented as instructed, then the new version will be executed from within the DSSAT shell "Accessories" section with TSE push button.

* If you still get Error or it looks like the TSE is not conducting optimization, please contact the author of the TSE, or raise ISSUE within this GitHub repository!

------------------------------------------------------------------------------------------------------------

<pre>
├── C:/DSSAT48
│   ├── Genotype
│   ├── Pest
│   ├── Maize
│   ├── Wheat
│   ├── Soil
│   ├── ...	
│   └── Tools
│       ├── GBuild
│       ├── XBuild
│       ├── ...
│       └── TSE
│           ├── TSE.exe
│           ├── yes.ico
│           ├── no.ico
│           ├── TSE.ico
│           ├── PhenologicalEventsDAP.txt
│           └── ParameterProperty.txt

After executing "TSE.exe" a working directory "TSE_workspace" is created where optimization is conducted and optimization output files saved:

├── C:/DSSAT48
│   ├── Genotype
│   ├── Pest
│   ├── Maize
│   ├── Wheat
│   ├── Soil
│   ├── Tools	
│   ├── ...	
│   └── TSE_workspace
│       ├── *.CUL
│       ├── *.ECO
│       ├── *_backup.CUL	
│       ├── *_backup.ECO
│       ├── ...
│       ├── TSE_Opt_Comb.txt  <- In this file original and TSE "optimal" coefficient combinations are located.
│       ├── ...	  
│       └── PlantGro.OUT
</pre>
------------------------------------------------------------------------------------------------------------

TSE related journal publications:

Cultivar coefficient estimator for the cropping system model based on time-series data: A case study for soybean (Transactions of the ASABE 2021, doi: 10.13031/trans.14432)

Implementation of an automatic time‐series calibration method for the DSSAT Wheat models to enhance multi‐model approaches (Agronomy Journal 2020, DOI: 10.1002/agj2.20328)
