## Bunq Data Science Intern Assignment

Author: Liang Huang. 
Date: 14 March 2019.
Email: liang.huang@student.uva.nl

## Objective: 

### 1. Find an optimal credit assignment given a finite budget.
### 2. Maximize the combined ROI (Return on Investment) of the individual campaigns.

## My Approach: 

### 1. Clean the input data. (Data corruption from row 763 to raw 1144).
### 2. Visualize the covariance among features.
### 3. Feature engineering and build the learning model. (Decision Tree, SVM, K-arm bandit)
### 4. Analysis of the results and select the best performing model.
### 5. Bring it to production.

## Conclusion.
### In this assignment, I provide two approaches to optimize our bidding strategy. One is to use regression models to predict the ROI(return on investment) based on the user's profile; another approach is to use a classification model to classify our target customers. 

### In practice, two approaches can be combined to find an optimal credit assignment given a finite budget. For example,  given a collection of candidate users and their profile, we can use classification model to filter out the non-target users first, then we can use a regression model to predict the ROI for each target user. Finally, we can sort the target users based on their ROI value and choose the top n users for our advertisement campaign. 

### By doing that, we can reduce a considerable amount of unnecessary cost by selecting the most suitable users. Therefore, we implicitly optimized our bidding strategy. However, if we need to predict the best price for bidding in the campaign, we can train a regression model to predict the money we should spend on each selected user. I didn't implement such a model here because that required much more historical dataset and parameter-tunning to build a usable model. If you are interested, I am looking forward to discussing it with you in the next interview.

### Thanks for reviewing my code, I am enjoying this assignment because I feel excited to find useful patterns of data by using machine learning techniques( using sk-learn libraries actually). Since I am just a beginner in data science so I might make some obvious mistakes somewhere, if you have any suggestions, please don't hesitate to tell me so I can do a better job next time. (liang.huang@student.uva.nl).
