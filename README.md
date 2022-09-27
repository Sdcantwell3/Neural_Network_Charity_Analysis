# Neural Network Charity Analysis
Analyzing the viability of charities using Neural Networks 

## Project Overview
The goal of this analysis was to create a binary classifier that is capable fo predicting whether applicants will have continued success after they are funded by Alphabet Soup.

### Purpose
More specifically I used the Python TensorFlow library to create a binary classifier that was then used to predict whether non-profit applicants will have continued success after the funds from our foundation Alphabet Soup have been spent.  This Machine Learning model is aimed at ensuring that the foudnation's money is not being distributed to foundations that are likely to fail in the near future.  Through marchine learning we created a deep learning neural network with the capacity to interpret large data sets efficienctly. 

### Results

#### Data Preprocessing
 - The target for my model is the variable IS_SUCCESSFUL
 - The features of my model are the variables ASK_AMOUNT, APPLICATION_TYPE, INCOME_AMOUNT, CLASSIFICATION, USE_CASE, ORGANIZATION, and STATUS.
 - I dropped EIN and NAME from the data set because they were not useful as a target nor a feature.
 
 #### Compiling, Training, and Evaluating the Model
 - I experimented with 2 and 3 hidden layers for the multiple attempts at this.  
 ##### Attempt 1
 - 2 hidden layers Fist layer had 80 nodes and the second layer had 30.  I ran the algorithm for 100 epochs and used "relu" for the two hidden layers and "sigmoid" for the output layer.
 
 ![2L8030e1002relu1sigmoid](https://user-images.githubusercontent.com/104606589/192430924-9ff68eab-158e-48ec-bab8-429ac80200d4.png)
 
 ##### Attempt 2 (opt/opt1)
 - 3 hidden layers Fist layer had 100 nodes, the second layer had 60, and the third layer had 10.  I ran the algorithm for 150 epochs and used "relu" for the first and third hidden layers and "sigmoid" for the second hidden layer and  output layer.
 
 ![opt](https://user-images.githubusercontent.com/104606589/192431331-cf627008-dda0-49f1-b4d6-1ca0440f102e.png)
 
 ##### Attempt 3 (opt2)
 - 3 hidden layers Fist layer had 100 nodes, the second layer had 80, and the third layer had 10.  I ran the algorithm for 150 epochs and used "relu" for all 3 hidden layers and "sigmoid" for the output layer.
 
 ![opt2](https://user-images.githubusercontent.com/104606589/192432067-d8cddf68-bbb9-4abf-8400-b878154e8d1d.png)

 ##### Attempt 4 (opt3)
 - 3 hidden layers Fist layer had 100 nodes, the second layer had 70, and the third layer had 30.  I ran the algorithm for 150 epochs and used "relu" for the first hidden layer and  "sigmoid" for the second, third, and  output layer.
 
![opt3](https://user-images.githubusercontent.com/104606589/192432422-1cac4a87-ff25-4aff-bdaf-14c1325611c3.png)

#### Outcome
- I was not able to achieve the goal of getting to 75% accuracy.

### Summary
I had the best results 72.6% when I ran the model with 2 hidden layers for 100 epoch's.  I was unable to reach my goal of 75% through manipulating the hidden layers and would recommend eliminating some more of the "noise" form the data.  I would also consider running the data through a random forest classifier model to see if I could come up with a more accurate predictor.

 


 


