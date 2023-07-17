# MACHINE LEARNING TRADING BOT

### LEGAL DISCLAIMER

*The content contained in this code module is for informational purposes only. You should not construe any such information or other material provided pursuant to the developer (the “Materials”) as investment, financial, tax, legal or other advice. The Materials are not investment advice and any observations concerning any security, trading algorithm or investment strategy provided in the code is not a recommendation to buy, sell or hold such investment or security or to make any other investment decisions. Any use of the Materials, and any decisions made in reliance thereon, including any trading or investment decisions or strategies, are made at your own risk. You should seek the advice of a competent, licensed professional if you require investment, trading or other advice.*

## OVERVIEW

The landscape of the investment world is changing in more ways than just the ebb and flow of the stock market. The advent of cutting edge strategies and technologies are now coming to the forefront which offer the prospect of making immense amounts of money - and yet, they also open the door to taking substantial losses. In a global market in which millions of participants are all trying to find ways to come out on top, every advantage counts. This is especially true in the realm of institutional investing. The capital we are able to secure for our clients will either make or break our careers and the success and reputation of the firm itself. Our clients don't want to hear that we didn't make them money because we are in a bear market or recession, they want results, that's why they hire us to do the job for them. Though a disruptor in the field, and one that many are still hesitant to embrace, the union of machine learning and algorithmic trading and financial analysis presents a lucrative opportunity to streamline strategies and execute transactions at a far higher clip than the traditional stock broker. Using historical stock data, this module will not only demonstrate such a strategy, the strategy will be tested, compared, and analyzed to discern the best course of action. In this comprehensive Machine Learning Trading Bot the following objectives will be completed:

1. Establish a baseline performance.

2. Tune the baseline trading algorithm.

3. Evaluate a new machine learning classifier.

4. Create an Evaluation Report.



## TECHNOLOGIES

In order for this algorithmic trading bot to run, the installation requirements are as follows:

[Python](https://www.python.org/downloads/) - Enables the user to use the powerful Python programming language.

[JupyterLab](https://jupyter.org/) - Access to the web-based IDE JupyterLab.  

[Pandas](https://pandas.pydata.org/) - Grants access to the open-source Pandas data analysis tool, which is powered by Python.

[Scikit-Learn](https://scikit-learn.org/stable/install.html) - Provides users with a library of tools for predictive data analysis.

[Microsoft Excel](https://www.microsoft.com/en-us/microsoft-365/excel) - Enables the user to read compiled historical stock data.


## USAGE

In order to execute this Machine Learning Trading Bot, you must run the following imports:

```python
machine_learning_trading_bot.ipynb
import pandas as pd
import numpy as np
from pathlib import Path
import hvplot.pandas
import matplotlib.pyplot as plt
from sklearn import svm
from sklearn.preprocessing import StandardScaler
from pandas.tseries.offsets import DateOffset
from sklearn.metrics import classification_report
from sklearn.ensemble import AdaBoostClassifier
from sklearn.linear_model import LogisticRegression
from sklearn.tree import DecisionTreeClassifier
```

Accessing JupyterLab in Bash: `Jupyter Lab`



## ANALYSIS REPORT

After the analysis of the SVM, ADABoost, Logistic Regression, and Decision Tree classifier models to train and test the historical stock data to determine the best trading strategy, the conclusion is represented in the following metrics:

   
**SVM MODEL**

   precision    recall  f1-score   support

        -1.0       0.43      0.04      0.07      1804
         1.0       0.56      0.96      0.71      2288

    accuracy                           0.55      4092
   


**ADABOOST MODEL**

  precision    recall  f1-score   support

        -1.0       0.44      0.08      0.13      1804
         1.0       0.56      0.92      0.70      2288

    accuracy                           0.55      4092
   

**LOGISTIC REGRESSION MODEL**

precision    recall  f1-score   support

        -1.0       0.44      0.33      0.38      1804
         1.0       0.56      0.66      0.61      2288

    accuracy                           0.52      4092
  


**DECISION TREE MODEL**

precision    recall  f1-score   support

        -1.0       0.44      0.77      0.56      1804
         1.0       0.55      0.22      0.32      2288

    accuracy                           0.46      4092

**CONCLUSION:**

As you can see, based on the model statistics, two of the four classifier models yielded better results: The SVM classifier, and the AdaBoost classifier. In terms of accuracy, they both produced identical results at 55%. Though it received a slightly lower score than the top two performers, the Logistic Regression classifier model would also be a valid model to use due to the fact that it is above 50% just as the two models preceding it are. The only true underperformer in the squad was the Decision Tree classifier model which produced an accuracy of 46%. In the gallery section directly below, you will find the images of the plot results for each of the classifier models.



## GALLERY

**SVM PLOT**



**ADABOOST PLOT**



**LOGISTIC REGRESSION PLOT**



**DECISION TREE PLOT**





## CONTRIBUTORS

*Marcus LeGare (Author, Developer)*

### LICENSE

**COLUMBIA UNIVERISTY FINTECH BOOTCAMP**