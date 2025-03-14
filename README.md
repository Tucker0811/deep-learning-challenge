# deep-learning-challenge

Report on the Neural Network Model

Overview of the analysis:

The charitable organization Alphabet Soup aims to develop an algorithm that can forecast the likelihood of funding applicants achieving success. Utilizing expertise in machine learning and neural networks, we need to analyze the features in the given dataset to build a binary classifier that can determine whether applicants will thrive if granted funding by Alphabet Soup.

Results:

To start the data processing, we eliminated any unnecessary information. After removing the EIN and NAME columns, the remaining data was designated as features for the model. However, the NAME column was reintroduced in the second test for binning purposes. The dataset was then divided into training and testing sets. The target variable, labeled "IS_SUCCESSFUL," was assigned a value of 1 for success and 0 for failure. The APPLICATION data was examined, and the "CLASSIFICATION" values were used for binning. Several data points were set as thresholds to group rare variables under a new category labeled "Other." Finally, categorical variables were encoded using the get_dummies() function after verifying the effectiveness of the binning process.

Compiling, Training, and Evaluating the Model:

Each model consisted of three layers after implementing Neural Networks. The number of hidden nodes was determined by the total features. A three-layer training model generated 477 parameters. The initial attempt achieved an accuracy of just over 73%, falling slightly short of the desired 75% but remaining relatively close.

