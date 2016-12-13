## INFO 4250 Final Project
This repo contains material pertaining to my INFO 4250 - Surveillance and Privacy final project.  The project looks at COMPAS risk scores that are used in bail and sentencing decisions.  
One of the models is a Neural Net classifier, the other, a multi-class Support Vector Machine (SVC) classifier, both using only a small number of basic features:  
*'sex',
*'age',
*'race',
*'juv_fel_count',
*'juv_misd_count',
*'juv_other_count',
*'priors_count',
*'c_charge_degree'])  

to predict a risk score:
*'High',
*'Medium',
*'Low'.

#### Sources
The data csv files come from [ProPublica's repo](https://github.com/propublica/compas-analysis) of data they collected from FOIA requests (thanks for doing all the hard work!). 
Besides scikit-learn, tools from [Artem Golubim's library](https://github.com/rushter/MLAlgorithms) of simple ML implementations are used. This can be found in the MLA folder.