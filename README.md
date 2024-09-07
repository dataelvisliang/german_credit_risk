# german_credit_risk

About Dataset
The original dataset contains 1000 entries with 20 categorial/symbolic attributes prepared by Prof. Hofmann. In this dataset, each entry represents a person who takes a credit by a bank. Each person is classified as good or bad credit risks according to the set of attributes. The link to the original dataset can be found below.

Content
It is almost impossible to understand the original dataset due to its complicated system of categories and symbols. Thus, I wrote a small Python script to convert it into a readable CSV file. Several columns are simply ignored, because in my opinion either they are not important or their descriptions are obscure. The selected attributes are:

Age (numeric)
Sex (text: male, female)
Job (numeric: 0 - unskilled and non-resident, 1 - unskilled and resident, 2 - - skilled, 3 - highly skilled)
Housing (text: own, rent, or free)
Saving accounts (text - little, moderate, quite rich, rich)
Checking account (numeric, in DM - Deutsch Mark)
Credit amount (numeric, in DM)
Duration (numeric, in month)
Purpose (text: car, furniture/equipment, radio/TV, domestic appliances repairs, education, business, vacation/others)
Acknowledgements
Source: https://archive.ics.uci.edu/dataset/144/statlog+german+credit+data

Contexts
Through visual analysis, we conducted an initial exploration of the data and used cluster analysis to classify customers into different risk groups. Since the dataset lacked direct customer loan risk labels, we couldn't directly assess the accuracy of the risk classification. Therefore, we performed another round of cluster analysis (without considering customer loan risk characteristics) and divided the data into four categories. The classification results aligned with reality, allowing us to build a random forest model to identify key factors in risk classification. Although the model's accuracy cannot be precisely evaluated, it can still serve as an effective tool for preliminary risk assessment, thus improving the efficiency of risk identification.
