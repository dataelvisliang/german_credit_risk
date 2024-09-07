# german_credit_risk

## About Dataset
The original dataset contains 1000 entries with 20 categorical/symbolic attributes prepared by Prof. Hofmann. Each entry represents a person applying for credit at a bank, classified as either a good or bad credit risk based on a set of attributes. The link to the original dataset can be found below.

## Content
The original dataset is complex due to its system of categories and symbols. To simplify, a Python script was written to convert it into a readable CSV file. Some columns were omitted due to their perceived lack of importance or unclear descriptions. The selected attributes are:

- **Age** (numeric)
- **Sex** (text: male, female)
- **Job** (numeric: 0 - unskilled and non-resident, 1 - unskilled and resident, 2 - skilled, 3 - highly skilled)
- **Housing** (text: own, rent, free)
- **Saving accounts** (text: little, moderate, quite rich, rich)
- **Checking account** (numeric, in DM - Deutsche Mark)
- **Credit amount** (numeric, in DM)
- **Duration** (numeric, in months)
- **Purpose** (text: car, furniture/equipment, radio/TV, domestic appliances repairs, education, business, vacation/others)

## Acknowledgements
Source: [UCI Machine Learning Repository - German Credit Data](https://archive.ics.uci.edu/dataset/144/statlog+german+credit+data)

## Contexts
Through visual analysis, we performed an initial exploration of the data and used cluster analysis to classify customers into different risk groups. Since the dataset lacked direct loan risk labels, accuracy of the risk classification could not be directly assessed. Therefore, a second round of cluster analysis was conducted (excluding loan risk characteristics) and the data was divided into four categories. The classification results aligned with reality, which allowed us to build a random forest model to identify key factors in risk classification. Although the model's accuracy can't be precisely evaluated, it remains an effective tool for preliminary risk assessment, enhancing risk identification efficiency.
