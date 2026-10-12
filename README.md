# Graduate Admission Prediction Using PyTorch

## About the Project
This is my first Artificial Neural Network (ANN) project, built using PyTorch to predict the chance of admission to a graduate program based on student-related features.

The project covers data preprocessing, feature scaling, ANN model development, model training, and evaluation.

## Technologies Used
- Python
- PyTorch
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Google Colab

## Dataset
The dataset contains student-related features used to predict `Chance of Admit`.

The features commonly include:
- GRE Score
- TOEFL Score
- University Rating
- Statement of Purpose (SOP)
- Letter of Recommendation (LOR)
- CGPA
- Research Experience

**Target variable:** Chance of Admit

*Note: Update this section to match the exact columns in your dataset and include the original dataset source.*

## Data Preprocessing
- Split the data into training and testing sets.
- Used an 80:20 train-test split.
- Applied MinMax Scaling to the input features.
- Fitted the scaler on training data and used it to transform the test data.

## ANN Architecture
The model was implemented using PyTorch.

- Input layer: Depends on the number of input features
- Hidden layers: 1
- Hidden neurons: 7
- Hidden activation function: ReLU
- Output layer: 1 neuron with a linear output
- Loss function: Mean Squared Error (MSE)
- Optimizer: Adam
- Learning rate: 0.001
- Training epochs: 200

## Model Evaluation
The model was evaluated on the test dataset.

- **R² Score: 0.78**

This score indicates that the model explains approximately 78% of the variation in admission chances in the test dataset. It does not mean that 78% of individual predictions are correct.

Additional evaluation metrics, such as MAE and RMSE, can be included after calculation.

## How to Run the Project
1. Open the notebook in Google Colab.
2. Load the dataset.
3. Run the preprocessing cells.
4. Convert the scaled data into PyTorch tensors.
5. Build and train the ANN.
6. Evaluate the model and visualize the predictions.

## Future Improvements
- Compare the ANN with Linear Regression.
- Experiment with different numbers of hidden neurons.
- Plot training and validation loss.
- Evaluate MAE and RMSE.
- Improve generalization using validation data.

## Disclaimer
This model provides estimated admission chances based on the available dataset. Its predictions are not guarantees of admission decisions.

## Author
Created as my first ANN project while learning deep learning and PyTorch.
