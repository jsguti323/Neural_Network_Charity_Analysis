# Neural Network Charity Analysis


## Overview
Alphabet Soup is a non-profit, philthropic foundation dedicated to helping organziations that protect the environment, improve people's well-being, and unify the world. To ensure the foundation's money is being used effectively, we will analyze the impact of each donation and vet potential recipients. Using a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years, we will create a binary classifier that is capable of predicting whether applicants will be successful if funded by the foundation.

## Results
### Data Preprocessing
* Target Variable: 'IS_SUCCESSFUL'
* Features: 'APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'STATUS', 'INCOME_AMT', 'SPECIAL_CONSIDERATIONS', 'ASK_AMT'
* Removed Features: 'EIN', 'NAME'

### Compiling, Training, and Evaluating the Model
* Our initial neural network model had 2 hidden layers with 80 and 30 neurons respectively that used a "relu" activation system, as well as 1 output layer with 1 neuron that used a "sigmoid" activation system.
* The initial model had an accuracy score of 72.65% so we modified the model to raise our score.
  * The amount of layers were increased from 2 to 4.
  * The amount of neurons in each layer also increased from 80 and 30 to 100, 75, 50, and 25.
  * The amount of epochs increased from 100 to 150.
  * Input data was preprocessed further.
    * Bucketing the "ASK_MNT" feature lowered unqiue values from 8747 to 7.
    * Bucketing the "INCOME_AMT" feature lowered unique values from 9 to 7.
* The new model had an accuracy score of 72.72%, which wasn't a significant increase from our initial model.
* We were not able to achieve target performance.