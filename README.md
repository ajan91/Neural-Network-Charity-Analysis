# Neural-Network-Charity-Analysis

**Overview**
Bek’s come a long way since her first day at that boot camp five years ago—and since earlier this week, when she started learning about neural networks! Now, she is finally ready to put her skills to work to help the foundation predict where to make investments.

With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, Beks received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:

    EIN and NAME—Identification columns
    APPLICATION_TYPE—Alphabet Soup application type
    AFFILIATION—Affiliated sector of industry
    CLASSIFICATION—Government organization classification
    USE_CASE—Use case for funding
    ORGANIZATION—Organization type
    STATUS—Active status
    INCOME_AMT—Income classification
    SPECIAL_CONSIDERATIONS—Special consideration for application
    ASK_AMT—Funding amount requested
    IS_SUCCESSFUL—Was the money used effectively


**Deliverable 1 Requirements**

The following preprocessing steps have been performed:

- The EIN and NAME columns have been dropped
 
- The columns with more than 10 unique values have been grouped together
 
- The categorical variables have been encoded using one-hot encoding
 
- The preprocessed data is split into features and target arrays
 
- The preprocessed data is split into training and testing datasets

- The numerical values have been standardized using the StandardScaler() module


**Deliverable 2 Requirements**

The neural network model using Tensorflow Keras contains working code that performs the following steps:

- The number of layers, the number of neurons per layer, and activation function are defined 

- An output layer with an activation function is created
        
- There is an output for the structure of the model

- There is an output of the model’s loss and accuracy

- The model's weights are saved every 5 epochs

- The results are saved to an HDF5 file



**Deliverable 3 Requirements**

The model is optimized, and the predictive accuracy is increased to over 75%, or there is working code that makes three attempts to increase model performance using the following steps:

- Noisy variables are removed from features

- Additional neurons are added to hidden layers

- Additional hidden layers are added

- The activation function of hidden layers or output layers is changed for optimization

- The model's weights are saved every 5 epochs

- The results are saved to an HDF5 file
        
**Results**        

For this analysis and model, the target is held in IS_SUCCESSFUL field.
The following variable(s) should be considered on features model

    ORGANIZATION
    STATUS
    INCOME_AMT
    SPECIAL_CONSIDERATIONS
    ASK_AMT
    APPLICATION_TYPE
    AFFILIATION
    CLASSIFICATION
    USE_CASE

The following variable(s) should be removed from input and data.

    NAME
    EIN

Compiling, Training, and Evaluating the Model

Model Configuration:

    hidden_nodes_layer1 = 80
    hidden_nodes_layer2 = 30
    number_input_features = 43

This model acheived 63.8% accuracy with several attempts to incraese the accuracy including:

    Increasing the number of hidden nodes in layer 1 (3 X number of input features)
    Increasing the number of hidden layers to include a 3rd
    Changing the activation functions: tried linear, tanh, sigmoid for a combination of hidden layers and output layer

SUMMARY

Therefore the results include a recommendation for how a different model could solve this classification and results.

