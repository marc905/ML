# ML

Coursera Machine Learning Final Project
author: "Marc Reitz"
date: "November 12, 2018"

This repository holds the final project created R/knitr for the Coursera ML course.  

Citation:   Data for this project was sourced from:  http://groupware.les.inf.puc-rio.br/har

Objective:  The goal of your project is to predict the manner in which they did the exercise. 
            This is the "classe" variable in the training set. You may use any of the other 
            variables to predict with. You should create a report describing how you built 
            your model, how you used cross validation, what you think the expected out of 
            sample error is, and why you made the choices you did. You will also use your 
            prediction model to predict 20 different test cases.

Submission: Apply your machine learning algorithm to the 20 test cases available in the test 
            data above and submit your predictions in appropriate format to the Course Project
            Prediction Quiz for automated grading.

Summary:    For this analysis, the base data was subsetted to remove a large number of factors that predominantly
            recorded a value of 0 or NA.  With what remained, a validation data set was carved out and three models
            were applied:  a random forest model, a generalized boosted regression model and a combination of the two.
            The parallel processing methodology suggested by the instructor in the course forums was applied, which
            significantly reduced the time required to process the models.  From these model results, the random forest 
            model (99.1% accuracy) performed better than the GBM model (95.99%).  The combo model did not appear to add any 
            additional accuracy over the RF model, so the RF model on its own will be used for the final predictions.
