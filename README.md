# Deep-learning-assignment1
# CS6910 Assignment 1


Team members: REDDY JOSHNA MANOJ (EE21S113),AKSHAY G RAO(CS21S003)
# type the function name in search(ctrl+f)in the notebook to go to particular code
Complete code is in the Assignment_1.ipynb
1.Code Starts with importing libraries and intailization of wandb
# Question 1
Next code to the Question 1 starts in the thrid cell of notebook program, reads the data from `keras.datasets`, picks one example from each class and logs the same to `wandb`.
# Question 2 
The neural network is implemented by the  class ANNModel()(type the function name in search to go to particular code)
Executing feed forward neural network model with setting proper hyper parameters , following is the method
 model = runModelOnDataWithHP(config=None,x_train=x_train,x_valid=x_valid,y_train=y_train,y_valid=y_valid,activation_per_layer='tanh',epochs=10,hidden_layer_size=3,learning_rate=0.0001,num_neuron_per_hidden_layer=128,optimizer='nesterov',batch_size=128)
 **epochs**  
    The Batch Size and epochs is passed as an integer that determines the size of the mini batch to be taken into consideration per epoch.
**hidden_layer_size** - integer
**num_neuron_per_hidden_layer**-Integer
# Question 3
**Backpropogation**
complete Backpropogation Algorthim with choice of gradient update(cross entropy /MSE) is written in the function:
back_prop(self,y_pred,y_train) and computeLossGradient(self,y_pred,y_actual,loss)
**optimizers**
All the optimizers codes : are written in  the method updateParameters(self,optimizer='vanilla',learning_rate=1)
(sgd,momentum based gradient descent,nesterov accelerated gradient descent,rmsprop,adam,nadam)

# Question 4,5,6
All the sweeps and runs are done by using the function hpTuningWithWandb(config=None)
Detail explaination is given in the wandb report that is shared in gradescope
# Question 7
Best  model with best hyperparameters are run on test data to get test accuracy and confusion matrix
the function and  run command is  runBestModelAndPlotConfusionMatrix()
# Question 8
Best model with hyperparameters that is giving  high accuracy is run by changing one hyperparameter ( "gradient loss" from cross entropy to MSE(Mean Square error))
plots are generated by wandb and compared (please refer the report)





