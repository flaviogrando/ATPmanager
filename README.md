![ATPmanager](https://user-images.githubusercontent.com/16105418/110210945-05e27c80-7e73-11eb-9028-aea0171c8537.jpg)

# ATPmanager
This code was used to generate tens of thousand simulations used in:

 GRANDO, F. L., LAZZARETTI, A. E., MORETO, M., LOPES, H. S.; "Fault Classification in Power Distribution Systems using PMU Data and Machine Learning". Presented in: 2019 20th International Conference on Intelligent System Application to Power Systems (ISAP). Available in: https://ieeexplore.ieee.org/document/9065966.

 GRANDO, F. L., LAZZARETTI, A. E., MORETO, M.; "The Impact of PMU Data Quality on Event Classification in Distribution Systems". Subjected to IEEE Transactions on Smart Grid in March 2021 (UNDER REVIEW).

IMPORTANT: The codes and procedures for this study will be released with the publication of this last paper.

# What is ATPmanager?

ATPmanager is a software to automatically generate and control massive simulations of electrical systems using ATP (Alternative Transient Program). 

This software executes an automatic process in 3 steps: 
1) creates .atp simulation files;
2) performs simulations;
3) converts waveforms resulting (.pl4 files) in MATLAB files (.mat);

# Why is useful?
This software is useful for large-scale simulations (although it is possible to simulate only one case at a time). There is no limit of successive simulations without human interaction.

# How to use?

The user need download and install 3 softwares:

1) LabVIEW (any version, including student and trial licenses).
2) ATP (Alternative Transient Program)
3) Converter pl42mat.exe

For more details on the use of the platform, please access: LINK!?

Limitations:
The software is prepared for circuit simulations with basic elements such as branches (RLC elements), swithces and sources. It is not prepared to include ATP's TACS and MODELS routines.

Ohter possible limitations:
This application was developed for simulations of the  1992 IEEE test feeders available in: https://site.ieee.org/pes-testfeeders/resources/. Other test cases have not been evaluated. Additionally, we opted to replace transformers with equivalent impedances, this avoids possible numerical problems associated with ATP. This issue would go unnoticed in a large volume of simulations. For our cases, this simplification does not affect the purpose of the studies.




# Where you can help?
Please send an email to: flavio.grando.eng@gmail.com

# Who maintains and contributes?
UTFPR, UFSC and Gnarus Institute
