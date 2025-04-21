# Customer-Churn-Prediction
This project is a project i made where I used neural network to train data to predict whether a holder has exited the bank or not
The features in this dataset are 
- Customer ID
- Surname
- CreditScore
- Geography
- Gender
- Age
- Tenure
- Balance
- Number of Products
- has credit card
- is Active member
- Balance
And the Target Variable - 'Exited'
for preprocessing first I checked if theres missing values and duplicated values in the datset.Then I removed these values.Once we've cleaned the dataset I had mapped all the features that had entries as a string datatype to numerical so that we wont have any issues with training the data.Then as usual I used standard scaler to scale the data before training.Then I split the data into training and testing data in a 80/20 ratio.
For the modle training I used a neural network with 2 hidden layers each with 11 nodes each using the 'Relu' activation function and one output node using the 'sigmoid' activation function
while running the data on the model I used 100 epochs and also split the training data into training and validation split with the displays of th loss functions and accuracies.
In the end i got an accuracy of 86.35%
I also displayed a plot between the loss and validation loss from which we infer that both reduce similarly in the initial iterations and eventually the loss on the validation data becomes stagnant and a little higher than the loss of the training data.
similarly we find that the validation accuracy stops increasing a bit earlier than the accuracy from the plot between the accuracy and validation accuracy.
