Predicting side effects caused due to drug-drug interactions

Introduction:
Pharmaceutical drugs are important part of our daily lives. While some relieve
symptoms, others help to cure disease or condition. However, these drugs also cause side effects ranging from mild to life threatening. These side effects could be caused by a single drug or due to interaction between 2 drugs. That is, some drugs produce undesirable side effects with intake of other drugs. This results in life threatening conditions and hospitalizations.

Why the need to predict?
Predicting undesirable side effects due to intake of more than one drug helps pharmaceutical companies, the patients and the doctors. Pharmaceutical companies spend millions of dollars and 15-20 years to bring a drug to the market. Only about 2-5 percentage of drugs discovered in the lab get approved by FDA and successfully reach the market. Prediction will also benefit physicians when patients encounter side effects that were not reported before. 


Sources:
1) Side effects due to drug-drug pair: Two_sides dataset http://tatonettilab.org/offsides/
    ∙ The dataset contains 
        - drug pairs labelled as drug_1 and drug_2.
        - All the side effects caused due to the drug pairs
        - 1716 unique drug pairs
        - about 200,000 drug-drug pairs containing differnt combinations of the drug drug pairs
    

2) Chemical structure profile for drugs: Pawel's Dataset :http://members.cbio.mines-paristech.fr/~yyamanishi/side-effect/
    ∙ The dataset contains 888 chemical structure profile for each of the drugs

Predictive Models:
Since the dataset is wide and 200,000 drug-drug pairs, the models were built only on a subset of the data. This subset of the data are those drug-drug pairs that have most common side effects. For example, fever, diarrhoea were the most common side effects due to drug-drug interactions. 

Each of the side effects were the target or response variable. The chemical structures were used as features or predictors. There were 888 chemical structures. Hence, this is like a multi class single label classification problem.


Tools Used:Pandas and its library scikit-learn, Seaborn

Models Used: Classification models: Logistic regression, Random 
Forest, LASSO and XGBoost

Notes on notebooks:
Each of the notebooks are organized in a stepwise manner and named accordingly along with numbering. For example 1 represents the first notebook and the description (in the case notebook 1 is importing dataset) is mentioned along with the number. 


References:
Pauwels, E., Stoven, V., Yamanishi, Y., 2011. Predicting drug side-effect profiles: a chemical fragment-based approach. BMC Bioinform. 12 (1), 169. – Source of chemical substructures data
DrugBankTM : Original source for Pauwel’s dataset
Two_sides Dataset: http://tatonettilab.org/offsides/
