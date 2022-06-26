# Challenge-13-StartupRiskAnalysis
Create a binary classification model using a deep neural network to predict Startup Success
Optimize the model by changeing 
*    Number of hidden layers
*    Number of nodes in each layer
*    #epochs
*    Dropping features
    
# Results and conclusions
Per the instructions in the starter files, I created the model with 2 hidden layers and used the mean of Input feature and output node to decide the number of nodes in first hidden layer and mean of nodes in first layer and output layer to decide th number of neurons in the second layer. After compile the model and fitting it the evaluation on the test data showed accuracy of 0.73. I though the result of 0.73 accurcy was very good for a probles like which startup will succeed. If the model actually can predict will this accuracy, I would like to find a way to get into Venture Capital world. 

The second part of the Challenge was to optimize the model. In the origianl Jupyter notebook venture_funding_with_deep_learning.ipynb I developed 2 alternates models. 
* The first model has 2 hidden layers but I did change the number of neurons in these 2 layers. I did itterate quite a bit with different numbers but the accuracy would not improve.
* In the second alternated model I changed the number of hidden layers.I did experiment with different number of hidden layers and different number of neurons in each layer. The accuracy did not go above the accuracy of the original model. In the final ittertion which is submitted it has 4 hidden layers. I have also increased the #Epochs to 100

Then I made 4 copies of  started files to try and see if dropping feature would increase accuracy. I dropped features as follow
*    in Jupyter notebook venture_funding_with_deep_learning_optimize1.ipynb I dropped the APPLICATION TYPE feature
*    in Jupyter notebook venture_funding_with_deep_learning_optimize2.ipynb I dropped the CLASSIFICATION feature
*    in Jupyter notebook venture_funding_with_deep_learning_optimize3.ipynb I dropped the STATUS feature
*    in Jupyter notebook venture_funding_with_deep_learning_optimize2.ipynb I dropped all 3 features APPLICATION TYPE, CLASSIFICATION, STATUS
    
I observed that in all cases dropping features reduced the accuracy.
