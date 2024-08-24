# Market Basket Analysis for a Bakery Business

This repository contains a project focused on Market Basket Analysis (MBA) using transactional data from a bakery business. The aim is to uncover common product associations to devise strategies that can help increase sales.

## Project Overview

Market Basket Analysis (MBA) is a technique widely used in the retail sector to identify associations between items frequently bought together. In this project, we use the FP-growth algorithm to calculate product association rules from a dataset of bakery transactions. The insights derived from this analysis can help in making informed decisions about product placement, promotional strategies, and targeted marketing.

### Key Metrics

- **Support:** Measures how frequently an itemset appears in the dataset.
- **Confidence:** Indicates the likelihood of purchasing item Y when item X is purchased.
- **Lift:** Evaluates the strength of an association while controlling for item popularity.

## Dataset

The dataset consists of 20,507 entries, over 9,000 transactions, and 4 columns. It contains real transactional data from a bakery business, and is publicly available on Kaggle.

[Link to Dataset](https://www.kaggle.com/datasets/mittalvasu95/the-bread-basket)

## Methodology

1. **Data Preprocessing:** 
   - Loaded the dataset and cleaned the data by converting all text to lowercase.
   - Checked for and handled any missing values.

2. **Transaction Encoding:** 
   - Converted the dataset into a list of transactions.
   - Applied one-hot encoding to prepare the data for the FP-growth algorithm.

3. **Frequent Itemsets and Association Rules:** 
   - Used the FP-growth algorithm to generate frequent itemsets.
   - Calculated association rules using metrics like support, confidence, and lift.

## Results

The analysis revealed strong associations between certain bakery items, such as {cake → coffee}, with a confidence of 52.7% and a lift greater than 1.0. Based on these findings, various strategies can be implemented to increase sales:

- Placing associated items together on shelves.
- Offering promotional discounts on one of the associated items.
- Targeting advertisements based on item associations.
- Developing new products that combine frequently purchased items.


