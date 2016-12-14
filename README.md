## INFO 4250 Final Project
This repo contains material pertaining to my INFO 4250 - Surveillance and Privacy final project.  The project looks at COMPAS risk scores that are used in bail and sentencing decisions.  

### Models
I try two model types: a Neural Net classifier ([nnet-risk-model.ipynb](https://github.com/rae83/info4250/blob/master/nnet-risk-model.ipynb)) and a multi-class Support Vector Machine (SVC) classifier ([svc-risk-model.ipynb](https://github.com/rae83/info4250/blob/master/svc-risk-model.ipynb)).  The Neural Net performed considerably better, and as such, all follow-up work can be found in the [nnet-risk-model.ipynb](https://github.com/rae83/info4250/blob/master/nnet-risk-model.ipynb) file.  This is the file that constitutes the majority of this project.

All models are trained on a subset of the following features (with the subset clearly marked in the code notebooks):  
* sex
* age,
* race,
* juvenile felony count,
* juvenile misdemeanor count,
* other juvenile count,
* priors count,
* charge degree.

Models 1-3 are used to predict the COMPAS risk score level (High, Medium, or Low) that was assigned for a given example.  There are two types of risk scores: general risk and violent risk.  I train and provide side-by-side results for each type or risk score.

Model 4 predicts the 2-year rate of recidivism (will this person commit a crime again within the next two years?) for both general recidivism and violent crime redivisim.  The model presented here considerably outperforms COMPAS risk scores in predicting both types of recidivism.

I tried to put in clarifying blocks of text throughout to explain what is happening / being shown.  In the nnet notebook, The blocks of output text on a red background can be ignored; it is just output pertaining to training each model.  Let me know if you have any questions!

### Sources
The data csv files come from [ProPublica's repo](https://github.com/propublica/compas-analysis) of data they collected from FOIA requests (thanks for doing all the hard work!). 
Besides scikit-learn, tools from [Artem Golubim's library](https://github.com/rushter/MLAlgorithms) of simple ML implementations are used. This can be found in the MLA folder.