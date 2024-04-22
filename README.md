1.Goal:We aim to use regression models to predic a person has depression or not.

2.Dataset:from Kaggle, https://www.kaggle.com/datasets/indubarnwal/depression-dataset

2.1  Response variable: Depression(0:no depression; 1: have depression)

    8 predictors
    
    1 variables identified as int64 by default
    
    7 variables identified as object by default

2.2  Contents( since there are similar names, we need to change the names)

      Int: 
      
        Age
        
      Catagorical:
      
        1.Family Problem: yes, no

        2.Ignored(people don't care too much about): Sleep quality,	Exercise, Diet 

        3.Social Support: Low, Moderate, High  →  Low_Social_Support， Moderate_Social_Support， High_Social_Support

        4.Gender: Male, Female

        5.Demographics: Rural, Urban

        6.CGPA: Low, Moderate, High  →  Low_CGPA， Moderate_CGPA， High_CGPA

        7.Financial Problem: Mild, Moderate, Significant  →  Mild_Financial_Problem，Moderate_Financial_Problem， Significant_Financial_Problem	
    
2.3  Manage the imbalance:

        method of "upsample"

        Ratio of classes is 0 : 1 =  95715 : 4285 → 0 : 1 =  95715 : 95715
        

2.4 Visualisation

3.Model

  3.1  Logistic Regression Model

        1.  Use Dummy Variables to repalce original columns

        2.  Train the data

        3.  Measure the performance

            Accuracy: 0.875

            AUC: 0.95

  3.2  Decision Tree 

      1. Accuracy(depth=3):0.862
      2. Accuracy(depth=4):0.872
      3. Random forest:0.896

4.Conclusions

  1.Outcome: Random Forest has the best performance in predicting.
  
  2.Age and gender do not greatly effect feeling depression in this dataset.
   
    High CGPA
   
    Significant Financial Problem
   
    Low Social Support
   
    Rural in Demographic
   
    Having Family Problem
    
    Although these factors are not necessarily causally related to depression. People with the above characteristics have higher possibility to have mental problem. 
    
  3.Though logistic regression model is easy to handle, decision trees method is still significant in getting a model with higher accuracy

Each individual contribution in the project:

Liang Jianpeng:

    1.Initial data-driven Insights from the dataset 
    
    2.Manage the imbalance 
    
    3.Exploratory Data Analysis 
    
    4.Logistic Regression Model

Tang Yeqing:

    1.Improvement for Initial data-driven Insights from the dataset 
    
    2. Improvement for Exploratory Data Analysis 
    
    3.Decision Tree 

Joint completion:

    1.Search for datasets 
    
    2.Slides 
    
    3.Film

Reference：

https://www.nickmccullum.com/python-machine-learning/logistic-regression-python/

https://www.statisticssolutions.com/dummy-coding-the-how-and-why/#:~:text=Dummy%20coding%20is%20a%20way%20of%20incorporating%20nominal,value%20%28such%20as%20grade%20point%20average%2C%20or%20GPA%29.

https://elitedatascience.com/imbalanced-classes


