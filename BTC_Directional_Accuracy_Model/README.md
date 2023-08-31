# Data Preparation/EDA/Preprocessing

- Current Features: BTC close, BTC volume, returns
- Scaling: Min Max Normalization into 0 to 1
- Reshape dataframes to 3D for LSTM Neural Network
- Time Ordered Train/Validation/Test sets:  (45%, 45%, 10%)


# Modeling

- LSTM Layer with 256 neurons, time step window of 10, learning rate 0.01, activation function tanh.
- Dropout Layer 10%
- Dense Layer
- Loss function: MSE
- Optimizer: adam
- 50 epochs, 50 batch size
- Target: Returns
- Error/Loss/Accuracy: Pearson correlation between prediction and target. RMSE for Directional Accuracy.


# Results

52.3% directional accuracy on test set predicting for direction of the returns.

