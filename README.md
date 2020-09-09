# Coursera_Applied-Data-Science-Capstone
This project will be mainly used for the Applied Data Science Capstone, which is the icing on the cake of the DataSc Professional certificate by IBM.

# Introduction
Road traffic injuries are currently estimated to be the eighth leading cause of death across all age groups globally, and are predicted to become the seventh leading cause of death by 2030.

Analysing a significant range of factors, including weather conditions, special events, roadworks, traffic jams among others, an accurate prediction of the severity of the accidents can be performed.

These insights, could allow law enforcement bodies to allocate their resources more effectively in advance of potential accidents, preventing when and where a severe accidents can occur as well as saving both, time and money. In addition, this knowledge of a severe accident situation can be warned to drivers so that they would drive more carefully or even change their route if it is possible or to hospital which could have set everything ready for a severe intervention in advance.

Governments should be highly interested in accurate predictions of the severity of an accident, in order to reduce the time of arrival and thus save a significant amount of people each year. Others interested could be private companies investing in technologies aiming to improve road safeness.

This project consist of several parts divided in two different notebooks.

# Feauter Selection
This first notebook contains all the steps and transformations I performed for the feature selection. You can find the information on the raw data in the following kaggle page. The kaggle datasets contain an extended descriptions of different aspect of the accidents, thus I've selected the most relevant and useful data for my analysis.
# Predicting Traffic Accident Severity
- Data Description -
- Data Cleaning -
- EDA -
- Model Development -
     - Random Forest -
     - Logistic Regression -
     - KNN -
     - SVM -
- Results -:

| Algorithm | Jaccard |f1-score | Precision | Recall |	Time(s) |
| ---------- | -------|---------|-----------|--------|-----------|
| Random Forest	| 0.722 |	0.72 |	0.724 |	0.591 |	6.588 |
| Logistic Regression |	0.661 |	0.65 | 0.667 |	0.456 |	6.530 |
| KNN	| 0.664	| 0.66 | 0.652 | 0.506 | 200.58 |
| SVM	| 0.659	| 0.65 | 0.630 | 0.528 | 403.92 |

For this specific problem precision means the % of predicted severe accidents that were truly severe. The recall instead, is the % of truly severe accidents that were properly predicted. For this specific problem, the recall is more important than the precision as a high recall will favor that all required resources will be equipped up to the severity of the accident.
In this case, the recall is more important than the precision as a high recall will favor that all required resources will be equipped up to the severity of the accident. The logistic regression, KNN, and SVM models have similar accuracy, however the computational time from the regression is far better than the other two models. With no doubt the Random Forest is the best model, in the same time as the log. res. it improves the accuracy from 0.66 to 0.72 and the recall from 0.45 to 0.59.
