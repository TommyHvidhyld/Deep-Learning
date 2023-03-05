# Deep-Learning
Creating a binary classifier to predict whether venture applications will be successful if funded by the nonprofit organization Alphabet Soup

## Report on Alphabet Soup Charity Neural Network Model
### Objective:
The purpose of this analysis was to create a Neural Network Model, binary classifier in order to predict whether a venture seeking funds from Alphabet Soup would be successful or not successful.

### Results:
In my analysis I created four models:
1. The first model consisted of all input features from the dataframe with two hidden layers. The first containing 43 nodes and second 28 nodes. Each layer had an activation function of "RELU" or rectifier. The model was designed to run for 100 epochs.

![Screenshot 2023-03-05 at 12 47 24 PM](https://user-images.githubusercontent.com/113069752/222979744-333454d5-30c4-48ab-b07a-c4593a810e4f.png)

2. The second model was all the same as the first model but this time I added a third hidden layer with 28 nodes.

![Screenshot 2023-03-05 at 12 50 19 PM](https://user-images.githubusercontent.com/113069752/222979873-48c61e26-642c-4695-9c23-7d2f01a2d6e0.png)

3. The third model still consisted of all input features with three hidden layers, but this time the activation function was changed to "TANH"

![Screenshot 2023-03-05 at 12 52 26 PM](https://user-images.githubusercontent.com/113069752/222979992-7aab9fb1-7082-4b8f-8249-1deb926d84a1.png)

4. In my final model I decided to look at the input features again. I found the potential outliers of the application type which turned out to be the highest number. So I binned differently, which gave me a shape of 51 which is then reflected in the number of nodes in the first hidden layer. The results were consistent with my other models.

![Screenshot 2023-03-05 at 1 37 34 PM](https://user-images.githubusercontent.com/113069752/222981872-4b36edba-cd81-4446-9147-3852b6e59602.png)

### Data Preprocessing
The target variable for the model was the "is_successful" column
The features include all other columns from the table. Except the Name and EIN columns were dropped in the intial cleaning of the data.
The Name and EIN columns were chosen to be left out because they have no impact on whether or not a venture would be successful or not.

I chose 43 nodes for my input layer because that was the amount of features being used and 28 nodes for the 2nd hidden layer because it is roughly 2/3s of the input neurons layer.

Unfortunately I was never able to achieve the desired 75% accuracy. Each model was tweaked either by adding additional layers or activation functions. But all models came back with just under 75%.

### Summary
All models came in with an accuracy of under 75%. My recommendation would be to adjust the number of feature inputs and possbily running an automated Deep Learning Neural Network in order to get the most accurate number of inputs as well as the most accurate activation function.
