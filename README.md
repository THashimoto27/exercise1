# Readme: Exercise 1

The difference between my way and the original instruction

## 1. The number of steps
[Original Instruction has 3 steps]
- 1. Split the data into a training and a testing set.
- 2. Run K-nearest-neighbors, for many different values of K, starting at K=2 and going as high as you need to. For each value of K, fit the model to the training set and make predictions on your test set.
- 3. Calculate the out-of-sample root mean-squared error (RMSE) for each value of K.

[My way has 5 steps]
- 1. Made two dataset for each trim of 350 and 65 AMG

<Run 10 times>
- 2. Split the data into a training and a testing set with probability of 0.8 by each trim.
- 3. Set K-nearest-neighbors with 2-100 values of K.
- 4. For each value of K, Run regression of knnreg and fit the model training set to calculate the out-of-sample root mean-squared error (RMSE) for each value of K by each trim.
<up to this>

- 5. From the 10 times average of RMSE, we get the optimal value of K by each trim
- 6. we predict the model with the optimal K.

 ### Why?
 My steps calculate the 10-times average of the data split with the probability of 0.8 that is shown in the slide(intro-learning "Measuring model accuracy, revisited")
 
 # 2. The way of prediction
 The instruction says that we need to make predition while going to calculate K-nearest neighbors at the same time.
 But I did find the opitmal calculate of K at the first, and then made prediction with its K.
 I will ask TA on it.
 
 # 3. K-fold cross validation
 I did not use K-fold cross validation because this prompt of the problem looks like it was not requried. But this is just my impression and might be not correct. I will ask TA about it.
 
 # 4. The part of "Which trim yields a larger optimal value of K? Why do you think this is?"
 I haven't finished answering this question because I have no any idea! Please tell me your idea

