# Dynamic Selection of Ensembles

In this study, we consider three ensembles, Adaboost, Random Forest,and Voting and Validation, and train them on twenty four software  datasets to predict whether a class is buggy or not. We use Dynamic Selection of Ensemble (DSE) algorithm to select an ensemble learner out of these three ensembles for a new class instance, based on these learners performance on the software dataset containing the specific class instance. After training these datasets on the three ensembles, and training DSE to select the best ensemble based on the ensemble’s performance for each software, it was found DSE performs significantly better than all of the individual ensembles using Friedman test based on AUC.

## Dataset used
All datasets for the purpose of this project have been taken from the PROMISE repository of open source software- http://openscience.us/repo/defect


## Using this repository
dataset/dataset contains all the preprocessed datasets which are input to DSE pipeline  
dataset/annotated contains output of first fold of cassification, including results of all three base ensembles and best ensemle for it  
dataset/DSE contains additional columns containing predictions of DSE and probabilities  
dataset/metrics includes performance metrics of all base ensmebles on softwares   
results contain performance metrics of DSE 
