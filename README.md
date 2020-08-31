Build and evaluate several machine learning models to assess credit risk, using data from LendingClub; a peer-to-peer lending services company. Finally, recommend whether they should be used to predict credit risk

## Machine learning models assessed with analysis

### Naive Random Oversampling model
 - Using this model, we come up with a balanced accuracy score of 64
 - Based on the imbalanced classification report:
   - The precision for predicting low risk (1.0) is higher than the precision for predicting high risk (0.01)
   - The recall(sensitivity) values are the same for predicting both low risk and high risk credit - 0.64

### SMOTE Oversampling model
 - Using this model, we come up with a balanced accuracy score of 66
 - Based on the imbalanced classification report:
   - The precision for predicting low risk (1.0) is higher than the precision for predicting high risk (0.01)
   - The recall(sensitivity) values for predicting low risk credit is higher (0.69) compared to the high risk credit (0.63)

### Undersampling using the Cluster Centroids Algorithm
 - Using this model, we come up with a balanced accuracy score of 53
 - Based on the imbalanced classification report:
   - The precision for predicting low risk (1.0) is higher than the precision for predicting high risk (0.01)
   - The recall(sensitivity) values for predicting low risk credit is lower (0.40) compared to the high risk credit (0.66)

### SMOTEENN algorithm
 - Using this model, we come up with a balanced accuracy score of 64
 - Based on the imbalanced classification report:
   - The precision for predicting low risk (1.0) is higher than the precision for predicting high risk (0.01)
   - The recall(sensitivity) values for predicting low risk credit is lower (0.57) compared to the high risk credit (0.72)

## Analysis
 - Between the four models, 3 of them have similar accuracy score except for the Undersampling method.
 - The precision for predicting low risk is much better compared to high risk credit for all the four models
 - The recall (sensitivity) for predicting high risk credit is much better with the SMOTEEN model compared to the other three models
 - Even though all the four models do not have a good accuracy score and the recall values for predicting high risk credit is at a max value of 72, it would be appropriate to go with the SMOTEENN model due to the capability to predict high risk credit more accurately
