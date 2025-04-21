# Customer-Churn-Prediction
I made this project using Neural Networks to train data to predict whether a holder is likely to exit the bank or not

Dataset used - https://www.kaggle.com/datasets/rjmanoj/credit-card-customer-churn-prediction

-Total Entries (Rows): 10,000

-Total Features (Columns): 14 (including the target variable)

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
And the Target Variable - 'Exited'.

For preprocessing, I first checked for missing and duplicate values in the dataset and removed them. Once the dataset was cleaned, I converted all categorical features (those with string data types) into numerical values to avoid issues during model training. I then applied StandardScaler to standardize the data, ensuring that all features had a consistent scale.
Next, I split the dataset into training and testing sets using an 80/20 ratio.
For model training, I implemented a neural network with two hidden layers, each containing 11 nodes and using the ReLU activation function. The output layer had a single node with a sigmoid activation function, suitable for binary classification.
I trained the model for 100 epochs and further split the training data into training and validation sets. During training, I monitored the loss and accuracy metrics for both the training and validation data.
The model achieved an accuracy of 86.35%.
I also plotted the training and validation loss, which showed that both decreased similarly during the initial epochs. However, the validation loss eventually plateaued and remained slightly higher than the training loss. Similarly, the validation accuracy stopped improving a bit earlier compared to the training accuracy, as observed in the accuracy plot.

Through this project, I gained a foundational understanding of Neural Networks and Deep Learning models. It also helped me grasp how these concepts are applied in practical scenarios.
