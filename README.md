# Horse-Racing-Prediction-with-Custom-MLP-Classifier

This section details the process of predicting horse racing outcomes using a custom Multi-Layer Perceptron (MLP) classifier implemented from scratch. The dataset includes various features related to horse racing events, and the goal is to predict whether a horse finishes first in a race.

### Steps Involved

1. **Load and Clean Data**:
    - Load the horse racing data from a CSV file.
    - Drop rows with missing values to ensure a clean dataset.
    - Remove duplicate rows to avoid redundant information.

2. **Feature Engineering**:
    - Convert the `calc_position` column to binary values (1 if the horse finished first, 0 otherwise).
    - Drop the `price` column as it is not required for the prediction.

3. **Data Visualization**:
    - Generate a pie chart to visualize the count of each statistic category in the dataset.

4. **Train-Test Split**:
    - Split the data into training and testing sets to evaluate the model's performance.
    - Use 80% of the data for training and 20% for testing.

5. **Feature Scaling**:
    - Standardize the feature values using a scaler to ensure all features contribute equally to the model training.

6. **One-Hot Encoding**:
    - Encode the target variable (`calc_position`) using one-hot encoding to convert it into a format suitable for training the MLP classifier.

7. **Initialize and Train the MLP Classifier**:
    - Define the architecture of the MLP with one hidden layer containing 32 neurons.
    - Initialize the weights and biases for the layers.
    - Train the MLP using forward and backward propagation over 1000 epochs with a learning rate of 0.01.

8. **Model Evaluation**:
    - Perform a forward pass on the test data to obtain predictions.
    - Compute the confusion matrix and classification report to evaluate the model's performance.
    - Generate the Receiver Operating Characteristic (ROC) curve to visualize the model's ability to distinguish between classes.

### Key Points

- **Data Preparation**: Cleaning the dataset by handling missing values and removing duplicates ensures high-quality input for the model.
- **Feature Engineering and Scaling**: Transforming categorical variables and standardizing features are crucial steps for effective model training.
- **Custom MLP Implementation**: Implementing an MLP from scratch involves defining the network architecture, initializing parameters, and performing forward and backward propagation to update weights.
- **Model Evaluation**: Evaluating the model using metrics like confusion matrix, classification report, and ROC curve provides insights into its performance and ability to generalize to new data.

![Screenshot 2024-06-23 190158](https://github.com/idrees200/Horse-Racing-Prediction-with-Custom-MLP-Classifier/assets/113856749/26dca294-a897-4984-953d-e17d25a58731)
![Screenshot 2024-06-23 190204](https://github.com/idrees200/Horse-Racing-Prediction-with-Custom-MLP-Classifier/assets/113856749/db3ed3ce-7bc0-4e4b-b05f-46f6aeecd11d)
![Screenshot 2024-06-23 190214](https://github.com/idrees200/Horse-Racing-Prediction-with-Custom-MLP-Classifier/assets/113856749/645e9e66-284c-4642-948b-3b43757303e5)
