## INFO 4250 Final Project
This repo contains material pertaining to my INFO 4250 - Surveillance and Privacy final project.  The project looks at COMPAS risk scores that are used in bail and sentencing decisions.  

One of the models is a Neural Net classifier, the other, a multi-class Support Vector Machine (SVC) classifier, both using only a small number of basic features:  
* sex
* age,
* race,
* juvenile felony count,
* juvenile misdemeanor count,
* other juvenile count,
* priors count,
* charge degree

to predict what the COMPAS violent recidivism risk algorithm would have assigned a given example:
* high,
* medium,
* low.

### Models
The model built out in nnet-risk-model.ipynb returned better results than that of svc-risk-model.ipynb, and as such, more in-depth work is presented in this notebook.  

The output at the very bottom of svc-risk-model.ipynb contains all the interesting information for that model.  For nnet, it is spread throughout the notebook but annotated with comments. I tried to put in clarifying blocks of text throughout to explain what is happening / being shown.  Let me know if you have any questions!

### Sources
The data csv files come from [ProPublica's repo](https://github.com/propublica/compas-analysis) of data they collected from FOIA requests (thanks for doing all the hard work!). 
Besides scikit-learn, tools from [Artem Golubim's library](https://github.com/rushter/MLAlgorithms) of simple ML implementations are used. This can be found in the MLA folder.