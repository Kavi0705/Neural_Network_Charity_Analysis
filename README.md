# Neural_Network_Charity_Analysis

## Analysis Overview
The purpose of this project is to use deep-learning neural networks to analyze and classify the success of charitable donations. The following methods were used for the analysis: preprocess the data for the neural network model, compile, train and evaluate the model, and optimize the model.

## Results
### Data Preprocessing

- EIN, NAME, STATUS, SPECIAL_CONSIDERATIONS, INCOME_AMT, and USE_CASE columns were removed from the data set.
- The column IS_SUCCESSFUL contains binary data refering to weither or not the charity donation was used effectively. This variable is then considered as the target for our deep learning neural network.
- The following columns APPLICATION_TYPE, CLASSIFICATION, ASK_AMT, and AFFILIATION are used for creating bins for unique values. 
- Then, encoding of the categorical variables, spliting into training and testing datasets and standardization were applied.

### Compiling, Training, and Evaluating the Model

- The deep-learning neural network model is made of 4 hidden layers with 100, 50, 50 and 30 neurons respectively.
- To optimize the training process, we are using the activation function ReLU for the hidden layers. As our output is a binary classification, Sigmoid is used on the output layer.Sigmoid activation funtion was also used for the input layer.
- For the compilation, the optimizer is adam and the loss function is binary_crossentropy.
- The model accuracy is under 75%. This is not a satisfying performance to help predict the outcome of the charity donations.
- To increase the performance of the model, the number of neurons in the hidden layers were increased, an additional hidden layer was also added.
- A different activation function (tanh) was also applied to the 1st hiddent lauyer, but none of these steps helped improve the model's performance above 75%.

## Summary
The deep learning neural network model did not reach the target of 75% accuracy. Considering that this target level is pretty average we could say that the model is not outperforming. Since the deep learning module was not ideal, we could use a supervised machine learning model such as the Random Forest Classifier to combine a multitude of decision trees to generate a classified output and evaluate its performance against our deep learning model.
