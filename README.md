# Airbnb Data Science Project

![Seattle](seattle.jpg)

_Here is a quick overview of the project. The full project with all analysis and findings can be viewed [here](URL!)._
---
## Overview
#### What are the factors and features of a listing that make an Airbnb listing in Seattle more expensive?  
  
That is the question this project aims to answer. We start of by collecting data of listings from [Kaggle](https://www.kaggle.com/airbnb/seattle). Then, we clean the data to a preferred format for data analysis. We then do Exploratory Analysis on the data by focusing on 3 sub-problems:

1. What are the features/facilities/ammenities of a property that affect its price?
2. Are there particular locations in Seattle where AirBnB listings fetch higher prices?
3. Does textual data in the summary and sentiments of reviews affect price?

Afterwards, we do Machine Learning on the data by adpoting 6 different **Regression** models for our regression problem. They are:

1. Linear Regression
2. Random Forrest
3. XGBoost
4. CatBoost
5. Ridge Regression
6. Lasso Regression

We partitioned the data into train and test sets and evaluated the models on their prediction accuracy. Once we found the most accurate prediction model, we used that model in library called **TreeInterpreter** which decomposed the prediction into a sum of contributions from each feature `Prediction = Bias + Feature1 x Contribution1 + … + FeatureN x ContributionN`. We used this to find the most important features that affected the price of a listing.

## Getting Started

### Prerequisites

If you would like to download and run all the data analysis and prediction models on your own machine, it is recommended to use to **Anaconda** and **Jupyter Notebook**. If you use **Anaconda** most of the packages used in this project are pre-installed except the following few:

+ Graphviz
+ Langdetect
+ Wordcloud
+ XGBoost
+ CatBoost
+ TreeInterpreter

### Installing and running

Install the required packages by running the following in your terminal:

```bash
pip install graphviz
pip install langdetect
pip install wordcloud
pip install xgboost
pip install catboost
pip install treeinterpreter
```

Then clone this repo with
```bash
git clone https://github.com/mohamedirfansh/Airbnb-Data-Science-Project.git
```

You can then open `Exploratory Analysis Problem 1.ipynb`, `Exploratory Analysis Problem 2.ipynb`, `Exploratory Analysis Problem 3.ipynb` and `Machine Learning Models.ipynb` with **Jupyter Notebook**.

## Built with

+ [Python 3](http://www.python.org/) - Main programming language used & done in Jupyter Notebook
+ [Pandas](https://pandas.pydata.org/) - Primary library used to manipulate the datasets
+ [Scikit-learn](https://scikit-learn.org/stable/) - Main library used for machine learning
+ [Matplotlib](https://matplotlib.org/) - Used for graph plots and visualizations
+ [Python NLTK](https://www.nltk.org/) - Used during exploratory analysis to get further insights into the textual data
+ [XGBoost](https://xgboost.readthedocs.io/en/latest/) - Used to implement gradient boost decision trees
+ [CatBoost](https://catboost.ai/) - Used to implement gradient boost decision trees
+ [TreeInterpreter](https://pypi.org/project/treeinterpreter/) - Used to decompose predictions into a sum of contributions from each feature

## Developers

+ [Mohamed Irfan](https://github.com/mohamedirfansh)
+ Dian Wei
+ Kristy

## License

[![GitHub](https://img.shields.io/github/license/mohamedirfansh/Airbnb-Data-Science-Project)](https://github.com/mohamedirfansh/Airbnb-Data-Science-Project/blob/master/LICENSE)

This project is licensed under the **[MIT License](http://opensource.org/licenses/mit-license.php)** - see the [LICENSE](https://github.com/mohamedirfansh/Airbnb-Data-Science-Project/blob/master/LICENSE) file for more details.  
Copyright © 2020 Mohamed Irfan.

---
