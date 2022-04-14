# California housing prices prediction
***
Here I am using the California housing dataset to train a model to predict housing prices in a district when certain features are fed into the system.
* The data was first divided into training and testing so that both have the same percentage of different categories. 
* Then the missing values were filled based on the median of the feature columns. 
* One hot encoding was used to transform categories (strings) into numerical quantities. 
* Some new features were added after finding linear correlation of different features and the target value. 
* Then the data was scaled so that it would be easy to train the model.
This whole process was turned into a pipeline.
***
Different models like linear regression, decision trees regressor and random forest regressor were used. They were evaluated using the RMSE score obatained after cross validation. The random forest regressor had the least RMSE score (i.e. was most accurate out of them all). So it was tuned using grid search cross validation. The final model was combined with the data preprocessing pipeline to form the final prediction model.
