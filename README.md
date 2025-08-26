# Crop Recommender System

A web-based application that leverages a machine learning model to recommend the most suitable crop to grow based on soil and environmental factors. This tool is designed to help farmers make informed decisions and improve their agricultural productivity.  
---

## 📋 Table of Contents  
- [Features](#-features)  
- [How It Works](#%EF%B8%8F-how-it-works)  
- [Technologies Used](#-technologies-used)  
- [Setup and Installation](#-setup-and-installation)  
- [Usage](#-usage)  
- [File Structure](#-file-structure)  
- [Screenshots](#-screenshots)  

---


## ✨ Features  
- **Intelligent Crop Recommendation:** Utilizes a trained machine learning model to predict the optimal crop.  
- **User-Friendly Interface:** A simple web form for users to input environmental and soil parameters.  
- **Comprehensive Inputs:** Takes into account seven key factors for prediction:  
  - Nitrogen (N) content in the soil  
  - Phosphorus (P) content in the soil  
  - Potassium (K) content in the soil  
  - Temperature (°C)  
  - Relative Humidity (%)  
  - Soil pH  
  - Rainfall (mm)  
- **Visual Feedback:** Displays the name and an image of the recommended crop.  

# Problem Statement
Selecting the right crop for specific soil and climate conditions is crucial for agricultural success. This project aims to automatically predict the most suitable crop based on soil nutrients and environmental parameters using machine learning techniques.

# Technologies Used:

Python
Flask (Web Framework- Backend)
scikit-learn (Machine Learning)
Pickle (Model Serialization)
HTML/CSS (Frontend)
NumPy (Data Processing)

# Project Structure
Crop_Recommendation/
│
├── app.py              # Main Flask application file
├── model.pkl           # Trained machine learning model
├── minmaxscaler.pkl    # Saved MinMaxScaler object
├── standscaler.pkl     # Saved StandardScaler object
├── requirements.txt    # Project dependencies 
│
├── templates/
│   ├── index.html      # Main page with the form and results
│   └── welcome.html    # Welcome page
│
├── static/
│   └── (images of crops like rice.jpg, maize.webp, etc.)
│
└── README.md


---
## ⚙️ How It Works  
The application operates through a straightforward workflow:  

1. **User Input:** The user enters the soil and environmental data into a form on the web interface.  
2. **Data Processing:** The Flask backend receives the form data.  
3. **Data Scaling:** The input features are scaled using pre-fitted MinMaxScaler and StandardScaler to match the format used for training the model.  
4. **Prediction:** The pre-processed data is fed into the trained machine learning model (`model.pkl`) which predicts the most suitable crop.  
5. **Display Result:** The application displays the name and an image of the predicted crop on the webpage.  

---

# Setup Instructions
Follow these steps to set up the project locally:  

### 1. Clone the Repository  
```bash
git clone https://github.com/your-username/Crop_Recommendation.git
cd Crop_Recommendation

# Install dependencies:
Install all required packages using:
```bash
pip install -r requirements.txt

# Run the application:
python app.py

Access the web interface at http://127.0.0.1:5000
Enter the required parameters and click "Get Recommendation"
![image alt](https://github.com/komal-sharma19/Crop-Prediction/blob/main/crop%20prediction.png?raw=true)
# Usage:
Launch the application.

You will see a Welcome Page – click the link to go to the form.

Enter values for all seven environmental and soil input fields:

Nitrogen (N)

Phosphorus (P)

Potassium (K)

Temperature (°C)

Relative Humidity (%)

Soil pH

Rainfall (mm)

Click Predict.

📸 Screenshots
🌱 Welcome Page

🌾 Prediction Form & Result

