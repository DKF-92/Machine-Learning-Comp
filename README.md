# Machine-Learning-Comp

This repository contains comparisons between out-of-the-box machine learning algorithms. We will be using the following datasets for this project:

- MNIST: a dataset of handwritten digits
- Wine Quality: a dataset comparing the qualities of several wines
- Housing prices: a dataset with a list of housing features and there respective prices 

### MNIST Dataset

This was the first dataset I applied the models too. This dataset contains a series of handwritten digits with labels identifying each. After training the models and tracking their accuracy scores I found that the SVC (support vector classifier) model preformed most accurately of all the models. This would make sense as SVC is a classifier type model typically used for classification in supervised machine learning scenarios. 

#### Accuracy of Models against the MNIST Datasets

![Models' accuracy on test data (MNIST)](https://github.com/DKF-92/Machine-Learning-Comp/blob/544e22323bf07ac1dd260ac6916fcf923bd7aac1/MNIST_Dataset/Accuracy%20of%20models.png)

### Wine Quality

This Dataset contained a series of red and white wines, and was found on Kaggle. It is important to note that this dataset is not very balanced as it contains far more high quality wines then low. I believe this dataset gives us a good example of when machine learning may not be the best solution when used for comparisons. This is evident with a high scoring 'Dummy Classifier'.

In the future I would like to re-visit this dataset maybe with a feature selection angle in mind. I would also like to note that at the time or writing I am also working onn debugging my Neural Network model to improve the very low score I am receiving.

![Models' accuracy on test data (MNIST)](https://github.com/DKF-92/Machine-Learning-Comp/blob/b977e00730691be8257906236c8105e5583798ef/Wine_Quality_Dataset/comparison-normalized-unnormalized.png)

Update: I used the same dataset to train a Neural Network separately (wine_NN.ipynb). This time I chose to preform more feature selection work by eliminating unimportant features. This resulted with much higher accuracy results seen below.

![MAE Neural Network (MNIST)](https://github.com/DKF-92/Machine-Learning-Comp/blob/1c0372e171beedd69518188678fe686fcce38e44/Wine_Quality_Dataset/MAE%20for%20Neural%20Network%20Model.png)
![Neural Network Accuracy (MNIST)](https://github.com/DKF-92/Machine-Learning-Comp/blob/1c0372e171beedd69518188678fe686fcce38e44/Wine_Quality_Dataset/Neural%20Network%20Model%20Accuracy.png)
