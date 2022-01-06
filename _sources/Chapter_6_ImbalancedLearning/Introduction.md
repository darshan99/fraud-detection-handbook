(Imbalanced_Learning)=
# Introduction

Imbalanced learning addresses classification problems where the number of examples representing one class is much lower than the ones of the other classes. Learning from imbalanced datasets is a difficult task since most learning algorithms are not designed to cope with a large difference between the number of cases belonging to different classes. Classification algorithms are often biased toward the majority class examples, so that minority ones are not well modeled into the final system {cite}`fernandez2018learning,chawla2009data,chawla2004special`. 

Credit card fraud is an example of imbalanced problem, since the proportion of frauds in real-world datasets can be as low as 0.01\% {cite}`lucas2020credit,ECB2020,dal2015adaptive`.  Imbalanced datasets are more generally encountered in many application domains such as telecommunication, bioinformatics, or medical diagnosis, and have been considered one of the top ten problems in data mining and pattern recognition {cite}`JMLR:v18:16-365`. 

Many solutions have been proposed to deal with this problem, both for standard learning algorithms and ensemble techniques. Imbalanced learning techniques can be broadly categorized into *cost-sensitive* and *resampling* methods. In *cost-sensitive* methods, algorithms are adjusted to favor the detection of the minority class. This usually implies a modification of the optimization function in the training step of the learning algorithm. On the contrary, *resampling* methods operate at the data level, by adding a pre-processing step to rebalance the dataset before the training algorithm is applied. Resampling can be achieved by removing examples of the majority class (*undersampling* techniques), adding examples of the minority class (*oversampling* techniques), or relying on a combination of undersampling and oversampling  {cite}`fernandez2018learning,dal2015adaptive`.   

The chapter is structured as follows. [Section 6.2](Cost_Sensitive_Learning) first covers cost-sensitive methods. [Section 6.3](Resampling_Strategies) then covers resampling strategies. [Section 6.4](Ensembling_Strategies) finally covers methods that rely on ensemble techniques. 