# Sampling imbalance study

Study of the impact of sample imbalance on the quality of models using the example of a churn forecast

Description of the experiment

In the course of this study, it was required to evaluate the impact of the imbalance of the objective on the quality of the classification models.

As metrics-assessments of the quality of the models, F1 was used - the harmonic mean between the recall and accuracy, and AUC-ROC - the area under the curve of the relationship between the recall of the model and the proportion of false positives.

Observations related to the outflow of customers from the bank were analyzed.

Three models took part in the experiment: logistic regression, decision tree and random forest. Each model was evaluated with default and fitted hyperparameters, with class-weighted samples, upscaling and downsampling with balanced samples.

The author experimentally proved that linear models are most sensitive to sample imbalance, and models based on decision trees are practically robust to imbalances.

At the same time, for linear models, the metrics remained at the reference values ​​regardless of the type of balancing, while tree-based models showed the best result when weighting classes.
