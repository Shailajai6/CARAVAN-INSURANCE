# CARAVAN-INSURANCE
Trained  a model using deep learning techniques to predict whether a customer accepts insurance or not. The dataset was imbalanced with very few records in one of the classes, so used customized class weights to get balanced classes for training the model. Obtained an accuarcy of 88 percent with prediction of sufficient amount of records in the rarest class.
# Preprocessing steps
 Our target label is categorical variable CARAVAN with two classes 0 or 1. There are 85 features , 9822 records.
 Analysed the data-types in the dataset and found an object data-type(categorical) with column name 'MOSTYPE'with 41 classes, 'MGEMLEEF' with 6 classes, 'MOSHOOFD' with 10 classes 'MGODRK' with 10 classes ,'PWAPART' with  10 classes. Used onehot encoding to encode the categorical variables and fit it.Obtained 151 columns after one-hot encoding, (there was one missing class in the MOSTYPE variable, 6 classes missing in the feature varaible PWAPART).
Used permutations and shuffled the data. Preprocessed the data and partitioned in to training and validation data
Analysed the target variable of the dataset and found that the classes were imbalanced. For instance the category 'Not purchased' has count=9236 (the highest) and the 'purchased' is 586 in the entire 9822 records.In order to balance the classes , used weights in the ratio of the records to balance the classes.
# Analysis
The naive accuracy without training any model is approximately 94 percent as the majority class is not purchased  ,macro recall 50 percent, so if we don't train any model the records are classified as per the majority class, all were classified as class not purchased. So, as we used customized  class weights , our model was predicting the minority class with recall of around 60 percent.
