# AutoML-examples


1. Create a new github repo called 'AutoML examples' 

2. Select a dataset of your own choosing (or select my modified version of SPARCS - https://raw.githubusercontent.com/hantswilliams/HHA-507-2022/main/autoML/datasets/data_sparcs.csv) 

3. Create two 'experiments' using the autoML package mljar-supervised 
One that is focused around classification (binary or multi-class outcome variable)
One that is focused around regression (continuous outcome variable) 
4. Include the output of the mljar-supervised output folder inside of the github repo (e.g., so there should be 2 folders - one for classification and one for regression) 

5. In a markdown file (readme.md): 
    - Describe the two dependent variables (outcomes) for experiment 1 and experiment 2 
    - Describe for each experiment: 
        - What was the best performing model (please interpret (a) log-loss or RMSE between models, and (b) AUC) 
        - How much better (? if any) did the model perform compared to baseline

---

# Experiment 1 Classification:

**Dependent variable:** Age Group

**Best Model:** XgBoost

**Method of Interpretation:** log-loss

**Log-loss Values:**

- Baseline = 1.54749
- Decision Tree = 1.00623
- ***Xgboost = 0.817724***
- NeuralNetwork = 0.94393
- RandomForest = 0.947229
- Ensemble = 0.817724

Compared to the baseline model, the Xgboost model performed better since it has a lower log loss value.

---

# Experiment 2 Regression:

**Dependent variable:** Total Charges

**Best Model:** Ensemble

**Method of Interpretation:** rmse

**Rmse Values**

- Baseline = 72381.7
- Decision Tree = 33807
- Xgboost = 19944.1
- NeuralNetwork = 36631.6
- RandomForest = 36887.8	
- ***Ensemble = 18837.9***

Compared to the baseline model, the Ensemble model performed better since it has a lower rsme value





