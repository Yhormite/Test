# Evaluating Suitable models for predicting CO2 emissions using Regression Analysis.

**Background of Topic:** Transportation, particularly the emissions from passenger cars, is a significant contributor to greenhouse gas emissions and climate change. As a result, there is a growing emphasis on reducing CO2 emissions from vehicles. Analyzing and predicting CO2 emissions from new cars based on their properties can provide valuable insights for policymakers, manufacturers, and consumers. Through regression analysis, i explored the most effective predictive models for CO2 emissions in the context of automobile features.


**Aim:** Aim is to help establish a model that quantitatively predicts CO2 emissions for new cars based on their varying properties.


**Source of data:** Data can be found at [CO2 emissions from new passenger cars](http://co2cars.apps.eea.europa.eu/?source=%7B%22track_total_hits%22%3Atrue%2C%22query%22%3A%7B%22bool%22%3A%7B%22must%22%3A%5B%7B%22constant_score%22%3A%7B%22filter%22%3A%7B%22bool%22%3A%7B%22must%22%3A%5B%7B%22bool%22%3A%7B%22should%22%3A%5B%7B%22term%22%3A%7B%22year%22%3A2021%7D%7D%5D%7D%7D%2C%7B%22bool%22%3A%7B%22should%22%3A%5B%7B%22term%22%3A%7B%22scStatus%22%3A%22Provisional%22%7D%7D%5D%7D%7D%5D%7D%7D%7D%7D%5D%7D%7D%2C%22display_type%22%3A%22tabular%22%7D)


**Result of Predictive Model:** 


**Linear Regression:** The Mean Squared Error (MSE) is extremely high, and the R-squared is negative, which is not supposed to happen under normal circumstances.However, this suggests that the data is not suitable for a linear regression model.


**Decision Tree:** The model has an MSE of 104.26 and an R-squared of 0.96. This model performs very well. A high R-squared indicates that the model explains a significant portion of the variance in the target variable.


**Random Forest:** The Random Forest model performs the best out of the five models. It has the lowest MSE of 72.33 and the highest R-squared of 0.97, indicating it predicts the CO2 emissions very accurately.


**Gradient Boosting:** This model has a slightly higher MSE (147.59) compared to Decision Tree and Random Forest models. The R-squared is 0.94, which is slightly lower but still indicates a good model fit.


**K-Nearest Neighbors:** The KNN model has an MSE of 129.37 and an R-squared of 0.95. This model's performance is good but not as great as the Random Forest model.


In summary, based on MSE and R-squared, the Random Forest model appears to be the best model for this data, followed by the Decision Tree and K-Nearest Neighbors models. The Linear Regression model is clearly not a good fit for this dataset.


Hence, for further prediction on estimating Co2 emmissions, Random forest would give the best result of all the models 
