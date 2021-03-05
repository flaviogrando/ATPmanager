# ATPmanager
This code was used to generate tens of thousand simulations used in the submitted article:

GRANDO, F. L., LAZZARETTI, A. E., MORETO, M.; "The Impact of PMU Data Quality on Event Classification in Distribution Systems". Subjected to IEEE Transactions on Smart Grid in March 2021 (UNDER REVIEW).


# What is ATPmanager?

ATPmanager is software to automatically generate and control massive simulations of electrical systems using ATP (Alternative Transient Program). 

This software executes an automatic process in 3 steps: 
1) creates .atp simulation files;
2) performs simulations;
3) convert waveforms resulting (.pl4 files) in MATLAB files (.mat);

# Why is useful?
This software is useful for creating large-scale simulations (although it is possible to simulate only one case at a time). There is no limit on the number of successive simulations, without human intervention.

# How to use?

The user must configure 4 basic steps:
1) Simulation conditions (simulation step, total time, input and output file locations, etc.)
2) Parameters of the electrical system (system frequency, data format, etc.)
3) Input data (electrical grid data such as lines, loads, switches, etc.)
4) System events and conditions (load switching, capacitors, faults, etc. and associated conditions such as switching time and system loading)

Limitations:

The events that can be simulated are:
1) Faults of all types (A, B, C, AB, BC, CA, ABG, BCG, CAG, ABC and ABCG) including cable breakage situations (open circuit faults) on the source side or on the load side;
2) Lines switching;
3) Load switching;
4) Capacitor banks switching;

The software is not prepared to include ATP's TACS and MODELS routines. It also does not include transformers to avoid numerical problems associated with ATP.


![ATPmanager](https://user-images.githubusercontent.com/16105418/110058746-af295580-7d41-11eb-9f2e-e4aefb129b85.jpg)




# Where you can help?
Please send an email to: flavio.grando.eng@gmail.com

# Who maintains and contributes?
UTFPR, UFSC and Gnarus Institute
