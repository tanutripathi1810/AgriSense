# 🌾 Smart Agriculture Yield Prediction with Random Forest

This project uses a **Random Forest Regressor** to predict agricultural yield (in kg/ha) based on various environmental and soil features, with optional integration of IoT sensor simulation via Tinkercad.

---

## 🚀 Live Tinkercad Simulation

You can view and simulate the sensor circuit for data collection here:

  ![Tinkercad Circuit Screenshot](images/tinkercad_circuit.png)

🔗 [Tinkercad Circuit Simulation](https://www.tinkercad.com/things/2MGq35x2HQD-agrisense/editel?returnTo=https%3A%2F%2Fwww.tinkercad.com%2Fdashboard%2Fdesigns%2Fcircuits)


## 📊 Project Overview

We use environmental features such as:
- Nitrogen, Phosphorus, Potassium (NPK)
- pH level
- Organic Carbon (%)
- Rainfall (mm)
- Temperature (°C)
- Humidity (%)
- Crop type (One-hot encoded)

The goal is to **predict crop yield** using these features with a Random Forest model.


## 🧠 Machine Learning Model

- **Model**: RandomForestRegressor
- **Hyperparameters**:
  - `n_estimators=300`
  - `max_depth=25`
  - `max_features='sqrt'`
- **Target Variable**: `Yield (kg/ha)`
- **Features Scaled**: Yes (MinMaxScaler)
- **Target Scaled**: No



## 📈 Model Performance

Using a cleaned synthetic dataset, the model achieved:

| Metric | Value |
|--------|-------|
| MAE (Mean Absolute Error) | ~8 kg/ha |
| RMSE (Root Mean Squared Error) | ~10–12 kg/ha |
| R² Score | ~0.95 |

---

## 📂 Files Included

- `cleaned_agriculture_dataset.csv` – Cleaned input dataset
- `random_forest_model.py` – Full code to train and evaluate the model
- `README.md` – Project documentation
- `circuit_diagram.png` – Screenshot of Tinkercad circuit

---

## 🛠️ How to Run

1. Clone the repository:
   ```
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
   ```
Install required libraries:

```

pip install pandas scikit-learn numpy matplotlib
```
Run the model:
```
python random_forest_model.py
```

To open or fork the circuit simulation, use the Tinkercad link.

## 🧪 Optional Enhancements
Integrate real-time sensor data using Arduino + ESP and Firebase

Deploy model to a Flask web app for real-time yield prediction

Use XGBoost or ensemble models for better accuracy

Collect real sensor values from Tinkercad via serial and log into a .CSV file

## 📬 Contact
For questions, reach out via GitHub issues or email: [tripathitanu02@gmail.com]




