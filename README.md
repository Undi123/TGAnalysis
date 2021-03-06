# TGAnalysis
ThermoGravimetric Analysis (TGA) helps in understanding and optimising pyrolysis process.

    Note
1.  TG = ThermoGravimetry graph measures mass loss vs time graph for a sample during pyrolysis.
2.  DTG = Differential TG with respect to time graph.
3.  T = Temperature.
4.  DTA = Differential Thermal Analysis graph measures dT/dt from reference vs T during pyrolysis.
5.  DSC = Differential Scanning Calorimetry graph measures dH/dt from reference vs T during pyrolysis.
6.  HHV = Higher Heating Value.
7.  ANN = Artificial Neural Networks.
8.  Components = It refers to the sub components of the material like cellulose, lignin etc. in case of biomass.

## Problem Statement
   **The main aim of this repository is to extract components, kinetic parameters and higher heating value from TG data beside sample segregation and identification. It is assumed that the overall DTG is the linear combination of DTGs of individual components.**

    Code Structure and Run Order
1.  Initialistion.m : The first file to be run, loads the dataset
2.  MixtureModel.m : This file uses Mixture Modelling to deconvolute the DTG dataset to extract individual components.
3.  Components.m : Extracting individual components
4.  RecordBiasVariance.m : Analyses error in mixture modelling and noise reduction.
5.  AnalysisKTD.m : Kinetic & Thermal parameter estimation from various methods, reaction order and kinetic error analysis.
6.  HHVAnalysis.m : Multiliear Regression on described model for HHV estimation.
7.  NeuralFitting.m : ANN fitting for HHV estimation.
8.  SOMClustering.m : Clustering for determining relationship between variables.
9.  PatternRecognition.m : Pattern in sample origin and characteristics.
10. PlotSave.m : Saving and generating all plots.

###### Beside the above 10 .m files all the other files are either dependencies or additonal files and folders.

    Made by:
> Mayank Mahawar **|** Indian Institute of Technology(IIT), Delhi **|** mayankskii@gmail.com
