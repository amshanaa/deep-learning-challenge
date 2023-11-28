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

In order to satisfy the ask of Alphabet Soup Organization, the feature that was utilized was whether the campaign was successful or not (IS_SUCCESSFUL).  The target we wanted to emphasize were the Successfule campaigns which were denoted with the number 1.

The first step in building the neural model for the dataset was to convert it into a dataframe and then applied the pandas function "getdummies" in the code below:


	STATUS 	ASK_AMT 	IS_SUCCESSFUL 	APPLICATION_TYPE_T10 	APPLICATION_TYPE_T12 	APPLICATION_TYPE_T13 	APPLICATION_TYPE_T14 	APPLICATION_TYPE_T15 	APPLICATION_TYPE_T17 	APPLICATION_TYPE_T19 	... 	INCOME_AMT_1-9999 	INCOME_AMT_10000-24999 	INCOME_AMT_100000-499999 	INCOME_AMT_10M-50M 	INCOME_AMT_1M-5M 	INCOME_AMT_25000-99999 	INCOME_AMT_50M+ 	INCOME_AMT_5M-10M 	SPECIAL_CONSIDERATIONS_N 	SPECIAL_CONSIDERATIONS_Y
0 	1 	5000 	1 	1 	0 	0 	0 	0 	0 	0 	... 	0 	0 	0 	0 	0 	0 	0 	0 	1 	0
1 	1 	108590 	1 	0 	0 	0 	0 	0 	0 	0 	... 	1 	0 	0 	0 	0 	0 	0 	0 	1 	0
2 	1 	5000 	0 	0 	0 	0 	0 	0 	0 	0 	... 	0 	0 	0 	0 	0 	0 	0 	0 	1 	0
3 	1 	6692 	1 	0 	0 	0 	0 	0 	0 	0 	... 	0 	1 	0 	0 	0 	0 	0 	0 	1 	0
4 	1 	142590 	1 	0 	0 	0 	0 	0 	0 	0 	... 	0 	0 	1 	0 	0 	0 	0 	0 	1 	0

5 rows × 117 columns


	


        What variable(s) are the target(s) for your model?
        What variable(s) are the features for your model?
        What variable(s) should be removed from the input data because they are neither targets nor features?

    Compiling, Training, and Evaluating the Model
        How many neurons, layers, and activation functions did you select for your neural network model, and why?
        Were you able to achieve the target model performance?
        What steps did you take in your attempts to increase model performance?
