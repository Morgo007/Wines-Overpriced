# Wines-Overpriced

This repository contains a Jupyter Notebook that uses prediction by inference to assess whether French wines are overpriced, relative to similar wines of similar quality from different countries. 

## Table of Contents
- Introduction
- Dataset
- Notebook Contents
- Conclusions
- Contributing

## Introduction

This project showcases several techniques and tools used for data analysis. This notebook showcases how to preprocess data, explore distributions, build various models (linear regression, KNN and random forests) and implements resampling techniques (cross-validation and bootstrapping). 

## Dataset

The dataset contains information on 38,686 wine ratings and reviews from WineMag, and American magazine rating wines for consumer markets.

The dataset includes variables such as: price, wine variety, the country and province of the wines origin, text reviews, wine rating and some derived information. The notebook explains these variables in extra detail. 

## Notebook Contents

1. **Data Loading and Preparation:** Importing libraries, loading datasets and preparing the data for subsequent analysis.
2. **Data Analysis:** Performing exploratory data analysis to understand the dataset.
3. **Data Cleaning:** Encoding categorical variables and transforming data.
4. **Model Exploration:** Building a series of models to gain insight into their usefulness.
5. **Resampling Techniques:** Evaluating the performance of models and ensuring the robustness of the results.

## Conclusions

After experimenting with a various models, a KNN (where k=22) was shown to be the optimum model.

This model was used for prediction as inference, which concluded that average French wine prices were overpriced (more expensive) when compared to the same type and quality of wine for different countries. The uncertainty surrounding these values were explored, and displayed consistently higher price predictions for French wines in comparison to other countries. Despite this, there was significant distribution cross over between French and US wines which suggests that the outcome could be sensitive to the data sampling. Another interesting note, is that all distributions overlapped with the French wine distributions, but these were at the upper limits and is very unlikely to occur.

Although the conclusion is that French wines are overpriced relative to similar wines of similar quality from different countries, the KNN that explored changes in quality and its effect on price, showed slight model bias for Italian and Spanish wines. These residuals were not deemed as considerable, and was ultimately left, but it could pose potential limitations on the conclusions made and could require further investigation.

## Contributing

Contributions are welcome! If you have any improvements or suggestions, please create a pull request or open an issue.
