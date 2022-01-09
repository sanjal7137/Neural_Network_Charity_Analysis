
# Neural_Network_Charity_Analysis

## Purpose

The purpose of this project was to use deep-learning neural networks with the TensorFlow platform in Python to analyze and classify the success of charitable donations.



## Results

### Data Preprocessing

* The target for current model was `IS_SUCCESSFUL` column, because it contained binary data refering to weither or not the charity donation was used effectively
* The following columns `APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT` considered to be the features for our model
* The columns `EIN` and `NAME` contained identification information and had been removed from the input data

### Compiling, Training, and Evaluating the Model

* This deep-learning neural network model consists of two hidden layers with 80 and 30 neurons respectively.

  The output layer is made of a unique neuron as it is a binary classification.

  To speed up the training process, `ReLU` activation function was used for the hidden layers. 

  As our output is a binary classification, `Sigmoid` is used on the output layer.

  For the compilation, the optimizer is `adam` and the loss function is `binary_crossentropy`.

* Target model performance was set to 75%. Current model was unable to reach this threshold.

* To increase the performance of the model, column `STATUS` was also removed, additional neurons added to hidden layers. Also, extra hidden layer was added.
  For activation function, the different `tanh` function was used but none of these steps helped improve the model's performance.
  
  
## Summary
  
Current model failed to reach target 75% accuracy threshold. Considering that this target level is pretty average we could say that the model is not outperforming.

Since we are dealing with binary classification, we could use a supervised machine learning model such as the Random Forest Classifier to combine a multiple decision trees to generate a classified output and evaluate its performance against current deep learning model.
