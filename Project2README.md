# statistics-for-artificial-intelligence-and-data-science

## **Project II**

## **Aim of Coursework II.**
The following analysis was carried out as part of an investigation on part of the Texas Department of Transportation (TDoT) regarding 
the conditions of the bridges of Texas state. The aim of this investigation is to check on the state of bridges so that necessary repairs
can be carried out. If this is not done, a bridge can fail. 

The following three variables are normally given with description about the state of the bridges - condition about the bridges' *deck, superstructure, 
substructure (foundations)*. However, *six new variables* are given by TDoT to be investigated, as to investigate how well the following new variables
could predict the condition of bridges and which of these proposed variables have more influence on the current condition - the bridges' *age, average use,
percent of traffic made up of 'trucks', material, design, and whether the bridges are historic or not.*

This analysis aims to give answers to the above posed questions by both visually inspecting 'what the data says' but also 'how it has been processed'. 
That is, any conclusions (preliminary or final) and their underlying assumptions are also reasoned and discussed.

## **Libraries and Nature of Operations**
* Pandas is used for dataframe creation and manipulations
* Matplotlib and Seaborn are used for visualisations
* Numpy is used for operations conducted on dataframes

 - Throughout the project - both in the data preparation and exploratory analysis stages - special care was given to the used variables as they included ordinal, 
continious, and categorical variables too, requiring constant conversions into variable formats that allowed meaningful operations to be carried out. 
- During the exploratory analysis stage, the main focus of the paper was to reduce the number of variables, that is, to find the most meaningful ones
that could later be used for the regression analysis (to find out which of these variables have more influence on the bridges' current condition). 

## **Content**

 1. **Section 1: Preparing the data**
      1. Creating a dataframe with relevant variables
      1. Deriving variable 'Age' for each bridge
      1. Excluding very old bridges based on two points (their age and how they are 'historically' classified)
      1. Reducing the number of categories of 'Material' and 'Design' (and the reasons behind it)
      1. Deriving a single integer Current Condition variable for each bridge based on selected ordinal categorical variables
      
 2. **Section 2: Exploratory Analysis**
      1. _Relationship between five predictor variables and target variable_
          * Predictor continuous variables and continuous target variable
          * Predictor categorical variables and continuous target variable
      1. _Relationship between predictor variables_
          * Continuous predictor variables
          * Categorical predictor variables and continuous predictor variables
          * Categorical predictor variables and categorical predictor variables
      1. _Summary of the findings and preliminary conclusions_
      
 3. **Section 3: Regression Modelling**
      1. Transforming categorical variables into dummy variables
      1. Checking for collinearity between variables used in regression analysis
      1. Dropping missing values from relevant columns of dataset
      1. Fitting the regression line - R2 coefficient, variables' coefficient results (comparing the coefficients), interpreting categorical coefficient outputs
      1. Prediction and the error distribution
      1. Plotting the regression line
