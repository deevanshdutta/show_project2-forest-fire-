This project uses a Ridge regression model to predict the forest fire weather index based on meteorological parameters. The model was trained and saved as a pickle file along with a scaler for data normalization, allowing predictions directly through the web application.

Features
Predictive Modeling: Uses Ridge regression to estimate fire weather risk.
Interactive Web Interface: Built with Flask, allowing users to enter data for prediction.
Data Preprocessing: StandardScaler normalizes data inputs for improved prediction accuracy.
Installation
Prerequisites
Python 3.6 or later
Flask
Scikit-Learn
Numpy
Pandas
Steps
Clone this repository:

bash
Copy code
git clone https://github.com/deevanshdutta/show_project2-forest-fire-/tree/main/FWI-main.git
Navigate to the project directory:

bash
Copy code
cd FWI-main
Install required packages:

bash
Copy code
pip install -r requirements.txt
Ensure the ridge.pkl model and scaler.pkl files are in the models_pkl directory.

Start the Flask application:

bash
Copy code
python app.py
Open your browser and go to http://127.0.0.1:5000.

Usage
Go to the home page.
Enter the following parameters for prediction:
Temperature: Current temperature (°C).
Relative Humidity (RH): Humidity level (%).
Wind Speed (Ws): Wind speed (km/h).
Rain: Rainfall (mm).
FFMC, DMC, ISI, Classes, Region: Forest fire-specific parameters.
Submit the form to receive a prediction.
Model Training
The model was trained using Jupyter notebooks, which handle:

Data Cleaning: Managing missing values and preparing the dataset.
Scaling: StandardScaler normalizes the data.
Model Training: Trains a Ridge regression model on processed data.
File Structure
app.py: Main application file for running the Flask server.
models_pkl/: Directory for serialized model (ridge.pkl) and scaler (scaler.pkl) files.
templates/: HTML templates for the web interface.
notebooks/: Jupyter notebooks for data preprocessing and model training.
Contributing
Contributions are welcome! Please feel free to fork the repository, submit issues, or create pull requests for any enhancements or bug fixes.
