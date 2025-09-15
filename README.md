# Federated-learning-

# Federated Learning with Flower (FLwr)

# Overview
## Framework: Flower (FLwr)  
## Dataset: MNIST  
## Setup: 3 Clients (Non-IID)  
## Algorithm: Federated Averaging (FedAvg)  
## Comparison: Federated vs Centralized  

# Project Structure
client_fn → Creates Clients  
MnistClient → Local Training and Evaluation  
## strategy → FedAvg with Metrics Aggregation  
## simulation → Runs Federated Rounds  
## central_model → Centralized Baseline  

# Experiment Setup
## Clients
### Client 1 → Digits 0–3  
### Client 2 → Digits 4–6  
### Client 3 → Digits 7–9  

## Model
### Type: MLP  
### Hidden Layer: 128 Units  
### Activation: ReLU → Softmax  

## Training
### Federated Rounds: 3  
### Centralized Epochs: 3  


# Key Insights
## FL works with Non-IID Splits  
## Accuracy Lower with Few Rounds  
## Centralized Model Highest Accuracy  
## More Rounds + Local Epochs Improve FL  
## FL Preserves Privacy, Centralized Does Not  

# How to Run
## Kaggle
### !pip install flwr tensorflow  
### Run Simulation Cells  
### Compare Federated vs Centralized  

## Local
### pip install flwr tensorflow  
### python server.py  
### python client.py  

# References
## Flower Documentation → https://flower.dev/docs  
## McMahan et al. (2017) → Communication-Efficient Learning of Deep Networks from Decentralized Data  
