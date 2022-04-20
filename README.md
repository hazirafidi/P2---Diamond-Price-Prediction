# P2 - Diamond Price Prediction

Diamond price prediction using Deep Learning Feedforward Neural Network
 
## 1. Project Summary

 The aim of this project is to construct and train a model that can predict the price of diamonds based on the features data. The features are as follows:-
 1. carat
 2. cut
 3. colour
 4. clarity
 5. depth
 6. table
 7. dimension (x, y, z)

## 2. IDE and Framework

The project is built with Jupyter Notebook as the main IDE and trained using Google Colab. The main frameworks used in this project are TensorFlow, Numpy, pandas, Matplotlib and Scikit-learn.

## 3. Methodology

The methodology of this project involve three stages whereby the first stage are data loading, data cleaning and data pre-processing where the data is observe missing or null and converting all the categorical values into numerical encoding. The second stage are building a model and compiling it. The model is constructed using tensorflow Fucntional API with Input layer, five hidden layers with 'relu' activation function and output layer with 'linear' activation function. The model is compiled with 'Adam' as the optimizer, 'MSE' as the loss and 'MAE' as the accuracy parameters.

### 3.1 Data Pipeline

The dataset is in the format of csv file. The csv file is loaded via pandas read. The data is further splitted into train and test data using Sciki-learn with the ratio of 80:20. The images are splitted into train and validation data in the ratio of 80:20.

### 3.2 Model Pipeline

The model architecture can be illustrated as in figure below.

![image](https://user-images.githubusercontent.com/100177902/163922216-bb36ef95-90b7-4103-9db8-88344d1a8321.png)

The model is trained with epochs set to 100. Early stopping is applied in the model training to avoid overfitting. The training stops at epoch 79 and the model performance is evaluated and the results are as shown in figure below.

![image](https://user-images.githubusercontent.com/100177902/163922463-f2816439-e24b-4001-823b-7d141452952e.png)

![image](https://user-images.githubusercontent.com/100177902/163922893-fa89b6d2-6bce-4bf5-ac40-e446f5fdd97a.png)

The model performance curve which are Training vs Validation Loss and Training vs Validation Accuracy can be refer as in figure below.

![image](https://user-images.githubusercontent.com/100177902/163923106-74760cfa-04b5-403a-acea-17929ee04858.png)

![image](https://user-images.githubusercontent.com/100177902/163923132-7b161310-ae1e-4b61-9fa6-14b9f9328048.png)

## 4. Result

The result of the model training can be visualize as prediction against label graph. The graph is plotted as below.

![image](https://user-images.githubusercontent.com/100177902/163923286-159ae282-17ba-47af-b5a4-27718437e93a.png)

From the graph above we can see the the predictions and labels are perfectly linear without outliers. The prediction price range is quite close to the labels price range. Overall, the model performance is quite good and can be imporoved if more data is feed into the model. 



