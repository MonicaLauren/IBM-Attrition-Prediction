# Phase-3-Project

# Summary

![download-2](https://user-images.githubusercontent.com/91205382/164997352-f53ed5f5-b406-458a-ad4d-8f496e443fa6.png)

## What are some of the characteristics of a loyal employee? What about employees who are on their way out? Can we model Employee Attrition?

Using employee-specific data from IBM, these are some of the questions we sought to answer.

Our model(s) relied on several predictors (among others):
  - Job type/department/role
  - Tenure
  - Salary
  - Age
  - Number of companies worked for previously
(and four or five others).

These predictors/features were determined first by availability -- what did we actually know about an employee? And secondly, by feature selection and feature importance.

Ultimately, no single factor proved overwhelmingly telling in predicting whether an employee would quit or not. However, longevity at IBM, as measured in a variety of ways -- years at IBM (obviously!), years with current manager, years in current role, etc -- was the strongest predictor of retention/attrition (in the case of longevity at IBM, retention).

As for our model, a Logistic Regression model (with tuned hyperparameters) was most successful. Given the imbalanced target class (see piechart above) and not overly large data set (<1500 data points), we our model selection and model tuning decisions often came down to maximizing Recall, or the ability to sucessfully predict the employees in our test set who DID leave IBM (our 'Yes's / 1s). The results of our final model are below. Later on, we will explain in greater detail the process that led us to this particular model and model-specifications.


<img width="734" alt="Screen Shot 2022-04-24 at 17 49 27" src="https://user-images.githubusercontent.com/91205382/164998074-08f09f0b-e07d-4e5d-88e1-ecaec8158263.png">



# Repository

This GitHub includes the following documents, which together comprise our project.

1. Three Python Notebooks. Generally, these notebooks each cover a seperate process of our project.
  Monica.ipynb - Data cleaning, filtering, description, and EDA.
  Graphs.ipynb - Further data description displayed in graphical form.
  Modeling.ipynb - Pipelines, Models, Model-Tuning, and Results.
  
2. df.pkl - Our Pickled data post-cleaning, filtering, etc.

3. Phase 3 Presentation.pdf - Our final PowerPoint, presented to class on 4/22.

4. WA_Fn-UseC_-HR-Employee-Attrition.csv - Our data.

5. README.md - This README!

# Modeling
