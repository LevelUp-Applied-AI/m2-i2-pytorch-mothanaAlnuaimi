# Integration 2 — PyTorch Housing Price Prediction

## What the model predicts
This model predicts apartment price in Jordanian Dinars (`price_jod`) using five input features:
- `area_sqm`
- `bedrooms`
- `floor`
- `age_years`
- `distance_to_center_km`

## Training configuration
- Model: Linear(5, 32) → ReLU → Linear(32, 1)
- Loss function: MSELoss
- Optimizer: Adam
- Learning rate: 0.01
- Epochs: 100

## Training outcome
The training loss decreased during training:
- Epoch 0: 1950619776.0000
- Epoch 50: 1949262464.0000
- Epoch 100: 1943238144.0000

The model completed training successfully and saved predictions to `predictions.csv`.

## Behavioral observation
The loss decreased steadily but slowly over the 100 epochs, which suggests the model was learning, but the improvement was gradual rather than rapid.