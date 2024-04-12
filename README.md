# Prediction-of-Product-Sales
This project aims to predict product sales using a [dataset](https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/). The dataset contains information about various products and their sales across different outlets. The project involves data cleaning, preprocessing, and exploratory data analysis (EDA) to gain insights into the dataset before building predictive models.
   -  This first project will be a sales prediction for food items sold at various stores.
   -  With these graphs and models, we can predict future product sales for our clients.

#### Author: SOUIDI Zied

## Business problem
The goal is to help the retailer understand the properties of products and outlets that play crucial roles in predicting sales.

## Methods
*   The following methods were used to clean and prepare the data for machine learning:
      -   Data Cleaning: The data was cleaned by looking for and removing duplicates, identifying null values and filling them with placeholders for EDA, and fixing inconsistencies in categorical columns.
      -   EDA: Exploratory Data Analysis was conducted and including visualizing distributions with histograms and boxplots, counts for categorical columns, and a correlation heatmap to show variable relationships.
      -   Feature Inspection: Feature inspection was completed on all features, and included univariate and multivariate visualizations to show important factors that impact sales.
      -   Machine Learning Pre-Processing: Pre-processing was completed on the data to prepare it for machine learning and inlcuded imputing the mean for numeric null values, imputing a placeholder value of "Missing" for categorical null values, OneHot and Ordinal encoding of categorical features, and scaling of numeric and ordinal features after encoding.
      -   Modeling: The following models were used to predict sales:
           *     Linear Regression
           *     Random Forest
           *     Tuned Random Forest

## Results

*   A heatmap is used to visualize the correlation between features in the dataset.
*   During the exploratory data analysis, a boxplot and histogram was visualized for each numeric datatype column.
*   A barplot was visualized for each categorical column.   


### Visual 1: Correlation heatmap
<img src="https://github.com/zyed79/Prediction-of-Product-Sales/assets/161171455/ef71b0c2-5484-4d2f-8dcd-07d261d889a8" width="800" height="600">


### Visual 2: Item MRP by Outlet Sales
<img src="https://github.com/zyed79/Prediction-of-Product-Sales/assets/161171455/2e0ae114-9962-44ec-86ac-dde81238da16" width="800" height="500">

   -   Here we can see that as the price of the item goes up, the total return goes up as well
   -   Less of those products are sold, but the higher price makes up the difference

### Visual 3: Outlet Type by Outlet Sales
<img src="https://github.com/zyed79/Prediction-of-Product-Sales/assets/161171455/b6ebe9d2-f721-4056-9453-377494e83ce3" width="800" height="500">

This visual shows Supermarket Type 3 has the highest average number of sales than the rest of the categories.

### Visual 4: Sales by Item Type (Countplot of Categorical Feature)
<img src="https://github.com/zyed79/Prediction-of-Product-Sales/assets/161171455/0ecea3d9-08d0-4e00-aa5b-27897be923cc" width="800" height="500">

The 3 most common items sold in stores are fruits/veggies, snacks, and household goods.

## Models

Machine Learning Using the Following Models:

-   Linear Regression Model
-   Random Forest Regressor Model
-   Tuned Random Forest Regressor Model


   ### Models Evaluated and Results


-   Linear Regression Model (Testing Set)

      R^2 = 0.57<br>
      RMSE = 1,092.87<br>
      MAE = 804.12<br>
      MSE = 1,194,355.77<br>
      
-   Random Forest Regressor Model (Testing Set)

      R^2 = 0.56<br>
      RMSE = 1,107.09<br>
      MAE = 773.42<br>
      MSE = 1,225,647.82<br>

-   Tuned Random Forest Regressor Model (Testing Set)

      R^2 = 0.597<br>
      RMSE = 1,054.942<br>
      MAE = 735.028<br>
      MSE = 1,112,903.139<br>

**The final model that was chosen is Tuned Random Forest Regressor Model, with max_depth of 10, n_estimators of 200 and min_samples_leaf is 4**.

## Recommendations

-  This data of big market need an update to make this model improved if we notic there is a convergence between metrics model so i think this is an 
   limitations in predction.

-  Overall, the best model is definitely the tuned Random Forest Regressor Model. There was still some bias in the model, but by far it outperformed the 
   linear regression model.
 
## Limitations & Next Steps

There are opportunities to further improve the model. Other features can explored by asking more questions such as "Why do Tier 3 locations have more sales? What kind of buyers purchase in Tier 3 locations?", or boosting the model (eg. using XGBoost).

# For Further Information

For any additional questions, please contact [zied79souidi@gmail.com](https://mail.google.com/mail/u/0/?hl=fr#inbox)
