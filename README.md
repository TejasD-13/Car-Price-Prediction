🚗 Car Price Prediction Web App

A machine learning–powered web application that predicts the selling price of used cars based on user inputs such as company, model, year, fuel type, and kilometers driven.
The app is built using Flask and a Linear Regression model, trained on a cleaned Kaggle dataset.

---
✨ Features:

📊 Predicts car prices using machine learning

🧠 Linear Regression model trained on real-world data

🌐 Web interface built with Flask

🔄 Dynamic dropdowns for company, model, year, and fuel type

⚡ Fast predictions with pre-trained model

---
🛠️ Tech Stack

Python
Flask
Flask-CORS
Pandas
NumPy
Scikit-learn
HTML / CSS

```bash
📂 Project Structure
├── app.py                     # Flask application
├── LinearRegressionModel.pkl  # Trained ML model
├── Cleaned Car.csv            # Dataset (Kaggle)
├── templates/
│   └── index.html             # Frontend UI
├── static/                    # CSS / JS
```

---
🧠 Machine Learning Model

Algorithm: Linear Regression

Target Variable: Car price

Input Features:
Car name,
Company,
Year of manufacture,
Kilometers driven,
Fuel type

The model is saved using pickle and loaded at runtime for predictions.

---
📊 Dataset

Source: Kaggle.

File: Cleaned Car.csv

The dataset contains information about used cars such as:
Brand,
Model,
Year,
Fuel type,
Kilometers driven,
Selling price.

---
⚙️ How It Works

User selects car details from the web interface.
The data is sent to the Flask backend via POST request.
Input values are converted into a DataFrame.
The trained Linear Regression model predicts the price.
The predicted price is returned and displayed to the user.

🚀 Installation & Setup
1️⃣ Clone the repository
```bash
git clone https://github.com/your-username/car-price-prediction.git
cd car-price-prediction
```

2️⃣ Install required dependencies
```bash
pip install flask flask-cors pandas numpy scikit-learn
```

3️⃣ Run the application
```bash
python app.py
```
4️⃣ Open in browser
```bash
http://127.0.0.1:5000/
```


🔮 Prediction Endpoint

POST /predict

Input Fields: 
company
car_models
year
fuel_type
kilo_driven

Output:
Predicted car price (rounded to 2 decimal places)