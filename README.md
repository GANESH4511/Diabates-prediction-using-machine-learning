

-----

# Diabetes Prediction Web App 🩺

This project is a web application that predicts whether a person has diabetes based on several medical diagnostic measures. The prediction is made using an XGBoost machine learning model trained on the PIMA Indians Diabetes Dataset, with a user-friendly interface built using Streamlit.

-----

## 🚀 Features

  * **Intuitive Interface:** A simple and clean web form for easy data entry.
  * **Instant Predictions:** Get a real-time diabetes risk assessment immediately after submitting the data.
  * **ML-Powered Accuracy:** Utilizes a trained XGBoost classifier for reliable and accurate predictions.
  * **Easy to Deploy:** Built with Streamlit, making it straightforward to run locally or deploy on a server.

-----

## 🛠️ Tech Stack

  * **Language:** Python
  * **Machine Learning:** Scikit-learn, XGBoost, NumPy
  * **Web Framework:** Streamlit
  * **Data Processing:** Pandas
  * **Model Persistence:** Pickle

-----

## 📋 Dataset

The model was trained on the **PIMA Indians Diabetes Dataset**, sourced from the National Institute of Diabetes and Digestive and Kidney Diseases. The dataset consists of data from female patients of at least 21 years of age and of Pima Indian heritage.

The prediction is based on the following 8 features:

1.  **Pregnancies:** Number of times pregnant
2.  **Glucose:** Plasma glucose concentration (2 hours in an oral glucose tolerance test)
3.  **BloodPressure:** Diastolic blood pressure (mm Hg)
4.  **SkinThickness:** Triceps skin fold thickness (mm)
5.  **Insulin:** 2-Hour serum insulin (mu U/ml)
6.  **BMI:** Body mass index (weight in kg / (height in m)^2)
7.  **DiabetesPedigreeFunction:** A function scoring the likelihood of diabetes based on family history
8.  **Age:** Age in years

-----

## ⚙️ Setup and Installation

Follow these steps to get the application running on your local machine.

### Prerequisites

  * Python 3.7 or higher
  * pip (Python package installer)
  * Git

### 1\. Clone the Repository

Open your terminal and run the following command to clone the repository:

```bash
git clone https://github.com/GANESH4511/Diabates-prediction-using-machine-learning.git
cd Diabates-prediction-using-machine-learning
```

### 2\. Create and Activate a Virtual Environment

It is highly recommended to use a virtual environment to manage project dependencies.

```bash
# Create a virtual environment named 'venv'
python -m venv venv

# Activate the environment
# On Windows:
venv\Scripts\activate

# On macOS/Linux:
source venv/bin/activate
```

### 3\. Install Required Packages

Install all the necessary libraries from the `requirements.txt` file.

```bash
pip install -r requirements.txt
```

-----

## 🚀 Run the Streamlit App

You are now ready to launch the web application\!

```bash
streamlit run "diabetes prediction web app.py"
```

> **💡 Important Note:** The original code specifies the model path as `'content/trained_model.sav'`. If your `trained_model.sav` file is located in the main project directory (as is typical), make sure to update line 13 in your Python script to:
> `loaded_model = pickle.load(open('trained_model.sav', 'rb'))`

After running the command, a new tab should automatically open in your web browser with the application running.

-----

## 📖 How to Use

1.  Once the application is running, you will see a web page with input fields for each medical feature.
2.  Enter the values for all the required fields.
3.  Click the **"Diabetes Test Result"** button to submit the data.
4.  The prediction (`The person is diabetic` or `The person is not diabetic`) will be displayed instantly on the screen.
