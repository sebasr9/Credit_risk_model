
#  Credit risk model and effects of income and climate change.

This projects provides an analysis of the borrower's medium income and the challenges that events such as climate change could bring to financial institutions. In doing so, we have developed a basic credit risk model using logistic regression to predict mortgage default probabilities (PD), and a linear regression model to predict the loss rate given default (LGD). Consequently, we analyzed the effect of including climate features into the PD and LGD model and its relation with the borrower's income.

### Part 1:

A. Data prep and importing income data

B. Describe the data using the describe method in pandas and plot the time series using matplotlib.

C. Mergin dcr and income dataset: The two dataset would be merge by 'State' and 'Time'. The income dataset was previously preprocessed in Excel and the income growth was calculated using the percentage change formula:

(( V2 - V1 ) /V1) × 100

### Part 2: PD Modelling

A. Estimate a basic credit risk model for mortgage default probabilities (PD). Include two standard explanatory variables which are FICO and LTV at origination. Do not include further variables. Compute the estimated PD for all mortgage loans and periods. Plot the average probability of default by time in a chart. Provide your code, output for the model and interpret the output.

In this first PD model, we will exclusively us two explanatory vairables which are FICO_orig_time and LTV_orig_time.

B. Estimate the PD model again by including explanatory variables in part (a), and the state-level income growth from Question 1 in one regression. Compute the estimated PD for all mortgage loans and periods. Plot the average probability of default by period in a chart

### Part 3: LGD Modelling

A. Compute the loss rate given default (LGD) for all mortgage loans and periods from the current loan to value ratio LTV assuming a 40% house price decline for all loans in all future periods and no repayment of the outstanding loan amount. Compute the hypothetical LGD for all mortgage loans and periods. Plot a histogram for the distribution of the LGD.

B. Run a linear regression model to predict LGD. Include the same set of explanatory variables used in the question 2b. Compute the estimated LGD for all mortgage loans and periods. Plot the average LGD by period

### Part 4: Expected loss

A. Compute the level of expected one-period loss for all mortgage loans and periods. PD should be inferred from question 2b and LGD should be inferred from question 3b. You may set the exposure at default to one dollar so that risk measures can be interpreted in percentages. Plot the average expected loss by time period in a chart.

### Part 5: Climate change analysis

A. Collect a time series from 2001 to 2015 of one climate feature. Build a linear regression model explaining the income growth rates from 1C (by year only) using the climate features making suitable assumptions. 

B. Collect a prediction of future values for your climate feature from 5A from 2015 onward.

For this task we have used the future prediction based on an RCP8.5 scenerio, which assumes that no significant efforts to reduce greenhouse emission (growing economica activity) would be made, consequently temperatures will continue to increase. it compraise a time period from 2015 to 2045.

C. Consider the PD and LGD over the lifetime of a 30 year mortgage loan (starting from the end of the data in 2015 until 2045). Calculate the PD and LGD term structure (by time) for a mortgage loan of a representative borrower and loan feature predictions of 5B using the model that you have developed in 5A.










