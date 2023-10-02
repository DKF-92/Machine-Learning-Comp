# Machine-Learning-Comp

This repository contains comparisons between out-of-the-box machine learning algorithms. We will be using the following datasets for this project:

- MNIST: a dataset of handwritten digits
- Wine Quality: a dataset comparing the qualities of several wines
- Housing prices: a dataset with a list of housing features and there respective prices 

## MNIST Dataset

This was the first dataset I applied the models too. This dataset contains a series of handwritten digits with labels identifying each. After training the models and tracking their accuracy scores I found that the SVC (support vector classifier) model preformed most accurately of all the models. This would make sense as SVC is a classifier type model typically used for classification in supervised machine learning scenarios. 

### Accuracy of Models against the MNIST Datasets

![Models' accuracy on test data (MNIST)](https://github.com/DKF-92/Machine-Learning-Comp/blob/544e22323bf07ac1dd260ac6916fcf923bd7aac1/MNIST_Dataset/Accuracy%20of%20models.png)

## Wine Quality Dataset

This Dataset contained a series of red and white wines, and was found on Kaggle. It is important to note that this dataset is not very balanced as it contains far more high quality wines then low. I believe this dataset gives us a good example of when machine learning may not be the best solution when used for comparisons. This is evident with a high scoring 'Dummy Classifier'.

In the future I would like to re-visit this dataset maybe with a feature selection angle in mind. I would also like to note that at the time or writing I am also working onn debugging my Neural Network model to improve the very low score I am receiving.

![Models' accuracy on test data (MNIST)](https://github.com/DKF-92/Machine-Learning-Comp/blob/b977e00730691be8257906236c8105e5583798ef/Wine_Quality_Dataset/comparison-normalized-unnormalized.png)

Update: I used the same dataset to train a Neural Network separately (wine_NN.ipynb). This time I chose to preform more feature selection work by eliminating unimportant features. This resulted with much higher accuracy results seen below.

![MAE Neural Network (MNIST)](https://github.com/DKF-92/Machine-Learning-Comp/blob/1c0372e171beedd69518188678fe686fcce38e44/Wine_Quality_Dataset/MAE%20for%20Neural%20Network%20Model.png)
![Neural Network Accuracy (MNIST)](https://github.com/DKF-92/Machine-Learning-Comp/blob/1c0372e171beedd69518188678fe686fcce38e44/Wine_Quality_Dataset/Neural%20Network%20Model%20Accuracy.png)

## Hosuing Prices Dataset

This dataset contains a series of houses with additional information such as Lot Area, Pool Area, Sale Condition, ect..... The training information comes with price values while the test data contains no pricing information. This project was part of a Kaggle competition with a goal of predicting an accurate sale price for each test house id. 

![Housing Pricing Accuracy Chart](https://github.com/DKF-92/Machine-Learning-Comp/blob/7bc02183624ec51d08b9d8041f97cc57085f1f36/Housing_Dataset/Accuracy%20of%20models.png)

# Models I used for this project

My goal with this project was to compare several machine learning models by testing them against different datasets. Below are breif descriptions of the models I used

### Linear Regression

Linear regression is a machine learning model that simply put uses independent variables to plot a line of best fit within the data. This can be used to predict outcome values of dependant variables. This simple yet powerful machine learning model is used for predictive analysis problems. 

This model will use the values between X and Y to plot a line of best fit on a graph. Using this plot, we can then use the value of X we have to try and make a prediction for the value of Y we want. 

### Logistic Regression

Logistic Regression uses the relationship between two data factors to create a ratio that can be used to make predicts. Outcomes in logistic regression must be a categorical or discrete value however, meaning that values received can be either yes or no, true or false, 0 or 1, ect.

A good example of logistic regression is whether or not a baseball pitcher will throw a strike, if the probability that the pitcher will throw a strike is 0.75 then the probability that the pitcher won’t throw a strike is 1 - 0.75 = 0.25. 

n the MNIST dataset this type of model was used to predict the probability that the image matched a numerical digit. For example if an image of a handwritten one scored 0.95 for 1, 0.56 for 2, and 0.23 for 3, the model will pick that the image is that of a handwritten one. 
