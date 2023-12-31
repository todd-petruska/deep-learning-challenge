# deep-learning-challenge

Overview of the analysis: The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. This project uses machine learning and neural networks for features in the dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.  The dataset is comprised of more than 34,000 organizations that received funding from Alphabet Soup over the years.

## Data Preprocessing Results:
* The model uses “IS_SUCCESSFUL for the target variable
* The feature variables for the model are the following: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL CONSIDERATIONS, and ASK-AMT.
* The EIN and NAME columns were removed from the data, since they are neither targets nor features 

The first model uses 100 neurons and 50 neurons as hidden layers with two activated as rectified linear unit (ReLU) and the output layer as ‘sigmoid’. The number of neurons for this model were doubled and epoch of 100 is used in order to test and hopefully understand how the neural net size impacts the accuracy rate. 


![model_1](https://github.com/todd-petruska/deep-learning-challenge/assets/128247739/6a71442f-ca11-499c-b300-e69fb848bc3e)





The second model uses 64 neurons, 16 neurons, and 4 neurons as hidden layers with three activated as (ReLU) and the output layer as is ‘sigmoid’. The number of neurons for this model were multiplied by four and epoch of 100 used to test/improve the accuracy rate.


![model_2](https://github.com/todd-petruska/deep-learning-challenge/assets/128247739/27616b6d-dcdf-4e6a-ac30-7be051b71798)


The third model uses 22 neurons, 16 neurons, 10 neurons, and 4 neurons as hidden layers with four activated as (ReLU) and the output layer is ‘sigmoid’. The number of neurons for this model uses increments of six and epoch of 100 to test how the neural net size impacts the accuracy rate.


![model_3](https://github.com/todd-petruska/deep-learning-challenge/assets/128247739/6849c6f5-aeb2-4f9b-8338-b3651cd0dbac)

All three of the deep neural net models did not achieve a 75% accuracy rate and the increase of neurons and hidden layers only saw slight improvements and in the 2nd case the additional hidden layers resulted in declined accuracy.  

## Summary: 

The first deep neural net model using the least number of hidden layers resulted in accuracy rates within close proximity to neural net models with numerous hidden layers.  Although, the second model uses an additional hidden layer its performance declined from the first model’s accuracy rate of 72.87463% to 72.7113% accuracy rate.  The third deep neural network utilizes four hidden layers and performed best; however, the improvement of 73.1311 accuracy rate vs. the first model’s 72.87463% accuracy rate is negligible. 

The use of an automated neural network using keras sequential model to search for the best hyperparameters could possibly improve the accuracy results for the dataset.  Additionally, running a model with data from the ‘NAME’ column would provide additional inputs to the model and could possibly result in improved accuracy.

Resources used for this project includes course materials, Stack Overflow, playground tensorflow.org, tensorflow documentation, and github. 
