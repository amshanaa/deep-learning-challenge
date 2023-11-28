# deep-learning-challenge
Module 21-Challenge


                                          OVERVIEW

The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. i utilized my knowledge of machine learning and neural networks to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.  Alphabet Soup’s business team, provided a CSV file of more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within the dataset were a number of columns that capture metadata about each organization, such as:

    EIN and NAME—Identification Columns
    APPLICATION_TYPE—Alphabet Soup application type
    AFFILIATION— Sector of Industry
    CLASSIFICATION—Government Organization Classification
    USE_CASE—Use case for funding
    ORGANIZATION—Organization type
    STATUS—Active status
    INCOME_AMT—Income classification
    SPECIAL_CONSIDERATIONS—Special considerations for application
    ASK_AMT—Funding amount requested
    IS_SUCCESSFUL—Was the money used effectively



DATA PREPROCESSNG:


The first step in building the neural model for the dataset was to convert it into a dataframe and then applied the pandas function "getdummies" in the code below:


![getdummies](https://github.com/amshanaa/deep-learning-challenge/assets/136298119/c2238f5d-5c77-4efe-9448-c231fd25d892)

What variable(s) should be removed from the input data because they are neither targets nor features?
Both EIN and Name were not needed and thus were removed from the dataset.

![drop](https://github.com/amshanaa/deep-learning-challenge/assets/136298119/827ddd32-0efd-42ce-9a3d-b9b3ae2b8526)


In order to satisfy the ask of Alphabet Soup Organization, the feature that was utilized was whether the campaign was successful or not (IS_SUCCESSFUL).  The target we wanted to emphasize were the Successfule campaigns which were denoted with the number 1.

![Success](https://github.com/amshanaa/deep-learning-challenge/assets/136298119/a91079b9-a1ef-4105-97d6-b17317073944)


    Compiling, Training, and Evaluating the Model
        
Neural networks need at least 3 hidden layers.  The first set was 80 neurons on layer 1, then 30 neurons on layer 2 and on the output layer it was 1. 

![hidden1](https://github.com/amshanaa/deep-learning-challenge/assets/136298119/95a74a06-f29a-48e7-8706-202cf05b2be1)


![hidden2](https://github.com/amshanaa/deep-learning-challenge/assets/136298119/25274740-5d15-43f3-a757-f550268b2da8)

![output1](https://github.com/amshanaa/deep-learning-challenge/assets/136298119/133c577b-9347-48f7-bff6-49ea8a0e86b8)

        
The model had an accuracy rate of 73.14%, unfortunately it did not reach the 75% threshold.

![sol1](https://github.com/amshanaa/deep-learning-challenge/assets/136298119/67b95159-f604-419a-8d14-f0a4e89c854e)


  
        What steps did you take in your attempts to increase model performance?

The model was optimized by changing the neurons in the layers and by manipulating the epoch as well.  I ran the model an additional 3 times and was not able to achieve the 75% threshold in all 3 attempts.  It was a fun exercise though.

This is the result after the first run

![chgmdl1](https://github.com/amshanaa/deep-learning-challenge/assets/136298119/f4f211a0-7694-4498-b7a9-2e821494a262)

![result1](https://github.com/amshanaa/deep-learning-challenge/assets/136298119/01615b9d-ef5c-42d8-bb0e-8121af676ad0)


This is the result after the second run

![chgmdl2](https://github.com/amshanaa/deep-learning-challenge/assets/136298119/876ed99f-d876-4734-b9a1-d05983d37682)

![result2](https://github.com/amshanaa/deep-learning-challenge/assets/136298119/ebc6f137-5467-475e-b391-53e43a487f26)


This is the result after the third run

![chgmdl3](https://github.com/amshanaa/deep-learning-challenge/assets/136298119/e5858add-239e-49b3-8cf9-a237daa7a6eb)

![result3](https://github.com/amshanaa/deep-learning-challenge/assets/136298119/971c5d6d-1c7e-4d3f-8ea5-8df77ac04673)

In conclusion, I manipulated the epoch in all 3 models and I did not see a difference in the output.  I am glad, I was able to get to this point in the model.






