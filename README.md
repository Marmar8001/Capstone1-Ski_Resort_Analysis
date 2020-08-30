# Guided Capstone Project Report

The main objective in this capstone project was predicting ticket price for Big Mountain ski resort in Montana based on different variables. The effects  of several variables were investigated. The variables included vertical drop, snow making area, number of runs, fast quads, skiable train area, total chairs, longest run miles, days open during the year and nightskiing area. 

For predicting ticket price, two regression models were selected: Linear model and Random Forest Model. Then the prediction of these models were evaluated with two metrics: R2 score and mean absolute error. Before doing regression, the outliers in the data were removed. Then, the data was normalized by a standard scaler and null values were replaced by median and linear regression was applied using pipe. In linear regression,8 features can predict well the ticket price. The variables included vertical drop, snow making area, number of runs, fast quads, skiable train area, total chairs, longest run miles and trams. 

Using GridSearchCV in cross validation was helpful for tuning hyperparameters in the both models. Both models showed the most important features were vertical_drop, snow making area, fastQuads and runs. Both random forest and linear regression have the mean r2_score around 0.7 but random forest has lower mean absolute error and variability in comparison to linear regression. Based on these results, we used random forest for the modeling part. 

The final ticket price using the Random Forest model was $ 94.22 which was more than $13 higher than it’s real price. This price was obtained by assuming other resorts had true ticket prices based on their market value. Also visualization showed that Big Mountain resort had high ranked facilities and ticket price was the highest in the state of Montana. The below graph shows that Big mountain resort had one of the highest vertical drop and snow making areas.

Based on the model, several scenarios were investigated to see how the resort can cut the cost or increase the revenue. The investigation showed that decreasing numbers of runs decrease the total revenue.

The most effective scenario was increasing vertical drop by 150 feet. For this purpose, one run should be added and an additional chair is needed. By doing that, the model predicted more than $3000000 increase in revenue. Other features were not very effective in increasing revenue.
