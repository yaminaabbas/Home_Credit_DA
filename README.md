## Crédit à la Consommation (Home Credit)

Énoncé du problème :

Home Credit recherche des motifs dans ses données concernant le risque de défaut des prêts à la consommation. Menez une analyse pour faire ressortir les motifs notables liés au risque de défaut.


Our goal is to analyze this dataset and explore for notable patterns regarding the default risk of consumer loans.  As was done for Option 1, we will follow the given process:

1. Look at the complete dataset and identify an approach.
1. Clean the data with rationale-backed handling of null or missing values.
1. Join the datasets together into a single dataframe.
1. Analyze default risk results.

This dataset is considerably more complicated than the Grocery Sales dataset; it is taken from [a Kaggle competition](https://www.kaggle.com/c/home-credit-default-risk/data), which provides the following diagram to explain its contents:
<img src='./Kaggle - Home Credit Schema.png'>

We are also provided with a definition of every column in every dataset, and an example submission file for Kaggle.

Of the three datasets, this is the most involved.  There are many potential connections, and the initial train/test datasets are the most complete of any on offer.

So, my strategy here will be slightly different.  I will first import a portion of the large, complete dataset (`application_train.csv`), then explore the potential for expanding it to add detail or answer new questions.


### 1. Look At The Data!

By printing the first few columns of each dataset, we can see how they might be combined to open up opportunities for analysis.  To do this, we need to import libraries, load the datasets into variables, and print their heads.
