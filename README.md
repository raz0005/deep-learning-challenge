# Neural Network Model for Alphabet Soup

## Analysis Report

### Purpose of the Analysis
We developed and optimized a neural network model to predict the success of charitable donations using data in 'Alphabet Soup.' The objective was to create a model that accurately classifies whether a charity application will be successful based on a variety of features. This model was initially developed in the `Starter_Code.ipynb` file and later optimized in the `AlphabetSoupCharity_Optimization.ipynb` file.

## Data Preprocessing

### Target Variable
- **`IS_SUCCESSFUL`:** Indicates whether or not a charity application was successful.

### Feature Variables
- **APPLICATION_TYPE:** Type of application submitted.
- **AFFILIATION:** Affiliation of the charity.
- **CLASSIFICATION:** Classification of the charity.
- **USE_CASE:** Use case for the donation.
- **ORGANIZATION:** Type of organization.
- **STATUS:** Status of the application.
- **INCOME_AMT:** Income amount of the charity.
- **SPECIAL_CONSIDERATIONS:** Any special considerations.
- **ASK_AMT:** Amount requested in the application.

### Data Cleaning
- **Removed Columns:** The `EIN` and `NAME` columns were removed as they are not relevant to the prediction task.

## Model Compilation, Training, and Evaluation

### Initial Model (`Starter_Code.ipynb`)
- **First Hidden Layer:** 80 neurons, ReLU activation function.
- **Second Hidden Layer:** 30 neurons, ReLU activation function.
- **Output Layer:** 1 neuron, sigmoid activation function.

**Model Performance:**
- Trained for 100 epochs, achieving a loss of 0.5581 and an accuracy of 72.79%.

### Optimization Attempts (`AlphabetSoupCharity_Optimization.ipynb`)

#### First Optimization: Adding a Third Hidden Layer
- **Modification:** Introduced a third hidden layer with 100 neurons and ReLU activation.
- **Performance:** 100 epochs, loss of 0.5619, accuracy of 72.87%.

#### Second Optimization: Increasing Epochs
- **Modification:** Increased the number of epochs to 200.
- **Performance:** Loss of 0.5941, accuracy of 72.66%.

#### Third Optimization: Adjusting Batch Size
- **Modification:** Changed the batch size to 50.
- **Performance:** Loss of 0.6112, accuracy of 72.73%.

## Summary of Results
The deep learning model developed in this analysis only achieved initial accuracy of 72.80%. Despite several optimization attempts, the model's accuracy only saw marginal improvements, with the highest accuracy being 72.87%.



