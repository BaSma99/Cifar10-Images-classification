# Cifar10-Images-classification

## Cifar10 images dataset:

   - This dataset consists of 10 classes.
   
   - The data consists of 60000 images, so this assignment runs on 16000 sample for training and 4000 sample for testing, according to the computation power.

![image](https://user-images.githubusercontent.com/54502733/210863047-31aa91b1-3df6-428d-a886-c97fb039091d.png)

 ## Implematation Steps:
    
    1- Split the dataset into training and testing datasets.
    
    2- Reshape the image data and perform scaling.
    
    3- Apply KNN classifier.
   
![image](https://user-images.githubusercontent.com/54502733/210863433-5474a060-79ad-4653-bd3e-35d82ae8590d.png)

![image](https://user-images.githubusercontent.com/54502733/210863508-f36a8cc3-1258-4ae3-890f-b85129395ece.png)

    4- Apply LOgistic Regression model and OVR method.
    
![image](https://user-images.githubusercontent.com/54502733/210863682-a3fde09b-d9b3-4d04-b69f-84d64478a750.png)

   5- Apply SVM model and OVR method.
   
![image](https://user-images.githubusercontent.com/54502733/210863840-de6e9e67-8401-41b9-a6d0-b7a46b6de5f8.png)

   - After developing the KNN model, the accuracy score = 0.302 for the optimal k where k = 10, and the KNN model cann't clasify the classes well. 


- The logistic regression model using a developed function for OVR strategy, the accuracy score = 0.38875, the model can not classify the 10 classes well, but the model can classify each class against all the classes well, as it shown in the accuracies of each model in the 10 models.


- The LinearSVC model has an accuracy score = 0.391 and this is not enough for classification tasks.


- So, apply the tuning will increase the accuracy, when taking a range for the cost parameter, the accuracy score = 0.40300 when c = 0.0010


- When applying the L1 regularization with a range of cost parameter, the accuracy score = 0.396 when C = 0.0100, there is no sign for overfitting, as the model didn't learn well from the data.


- When applying the cost parameter with gamma parameter with a range:
       
       
       - The accuracy score = 0.48225 when c = 1.00 and gamma = 0.01
       
       - The accuracy score = 0.49475 when c = 10.00 and gamma = 0.01
       
       - The accuracy score = 0.49500 when c = 100.00 and gamma = 0.01
 
 - So, the accuracy increased when gamma = 0.01

- After applysing PCA dimensionality reduction, the accuracy is not good enough for classifying the images.

- Finally, the classical supervised machine learning models are not good to classify images data. 
