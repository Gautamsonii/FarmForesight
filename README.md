# FarmForesight

Overview
This project, named Algo-Traders, integrates machine learning models for plant disease classification, crop recommendation, and fertilizer suggestion. The system is deployed using Flask, allowing users to interact with the models via a web interface.

Project Structure
app.py: Flask application handling web requests and responses.
model.py: PyTorch-based neural network model (ResNet9) for plant disease classification.
disease.py: Dictionary (disease_dic) containing information about various plant diseases.
fertilizer.py: Dictionary (fertilizer_dic) providing recommendations based on soil nutrient levels.
config.py: Configuration file containing API keys and other constants.
requirements.txt: List of Python dependencies for easy environment setup.
Models and Data
Plant Disease Classification Model:
Implemented using PyTorch ResNet9 architecture.
Trained on a dataset with multiple classes of plant diseases.
Crop Recommendation Model:
Utilizes a scikit-learn RandomForest model.
Trained on a dataset correlating soil conditions with optimal crop choices.
Datasets
Crop Dataset:
Contains information about various crops and their optimal nutrient requirements.
Fertilizer Dataset:
Provides district-wise crop yield data, useful for insights into regional agricultural trends.
Usage
Setup:

Install dependencies using pip install -r requirements.txt.
Ensure all necessary API keys (e.g., weather API) are configured in config.py.
Running the Application:

Execute python app.py to start the Flask web server.
Access the application at http://localhost:8080 in your web browser.
Functionality:

Crop Recommendation: Predicts suitable crops based on user-input soil parameters.
Fertilizer Suggestion: Recommends appropriate fertilizers based on soil nutrient levels.
Disease Detection: Identifies plant diseases from uploaded images using the trained neural network.
