# Prediction-of-Credit-quota
Based on the financial information of real companies, it seeks to generate a prediction model of the credit quota that could be assigned.

KEY POINTS
* Inside the cells of the Excel data there is an internal dictionary that displays the financial content of each company.
* Both P&Gs and balance sheets are different for each company, so it was necessary to find a method to keep all the information of each company.
* Most of the fields and information provided for each company are different. So, in other words same variables probably have a different name.

This is an example of the P&G of some company:

![image](https://github.com/engalejandrovargas/Prediction-of-Credit-quota/assets/77429377/30e3cf2d-2043-4b19-a9f8-38a0d3e6a250)

To solve the problem the following process was made:

![image](https://github.com/engalejandrovargas/Prediction-of-Credit-quota/assets/77429377/f3b79c54-cb13-4bc1-80ee-2c1413369be3)

Initial components: 2967 
PCA components: 190
Variance ratio: 0.990239339009448
Dimensions required for a variance of 0.99%: 190

![image](https://github.com/engalejandrovargas/Prediction-of-Credit-quota/assets/77429377/f9fbc919-74a7-4e36-b601-7f7cbd28eef1)

To initially check how different algorithms behave, orange software was used:

![image](https://github.com/engalejandrovargas/Prediction-of-Credit-quota/assets/77429377/4ccbe546-59b6-479b-baf9-b23758ff2a0c)

The quota was skewed to the right. This is a problem because most ML models do not work well with data that is not normally distributed. Was applied a log(1+x) transformation to correct the bias.
Finally the RMSE Score was compared:

![image](https://github.com/engalejandrovargas/Prediction-of-Credit-quota/assets/77429377/bde3634f-948b-496c-aa19-d44343f2a9b4)

Please have a look to the notebook for detailed information.

Thanks!!











