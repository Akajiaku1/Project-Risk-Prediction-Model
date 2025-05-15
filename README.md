# 🛡️ Project Risk Prediction Model

This project uses machine learning to predict the **risk level** (Low, Medium, High) of a project based on its characteristics. It's suitable for PMOs, project analysts, and decision-makers seeking to proactively manage project uncertainties.

---

## 📊 Features

- Synthetic dataset generation
- Random Forest classifier for risk prediction
- Label encoding and feature scaling
- Model serialization with `joblib`
- Interactive Streamlit dashboard

---

## 📁 Project Structure

Project-Risk-Prediction-Model/
├── data/ # Project data (auto-generated)
│ └── project_data.csv
├── model/ # Saved model files
│ ├── risk_model.pkl
│ ├── scaler.pkl
│ └── label_encoders.pkl
├── generate_data.py # Creates synthetic data
├── risk_model.py # Trains and saves model
├── app.py # Streamlit app for predictions
├── requirements.txt # Python dependencies
└── README.md # Project documentation


---

## ⚙️ Setup Instructions

### 🔽 1. Clone the Repository

```bash
git clone https://github.com/yourusername/Project-Risk-Prediction-Model.git
cd Project-Risk-Prediction-Model

📦 2. Install Requirements

We recommend using a virtual environment:

pip install -r requirements.txt

📊 3. Generate Synthetic Data

python generate_data.py

🤖 4. Train the Model

python risk_model.py

🌐 5. Launch Streamlit App (Optional)

streamlit run app.py

🧠 Model Details

    Algorithm: Random Forest Classifier

    Preprocessing:

        Categorical encoding using LabelEncoder

        Feature scaling using StandardScaler

    Target: risk_level (classified as Low, Medium, High)

🧪 Sample Features Used
Feature	Description
budget	Estimated project cost (USD)
duration	Duration in months
team_size	Number of people on the team
complexity	Categorical: Low, Medium, High
stakeholder_engagement	Categorical: Poor, Average, Good
past_risk_incidents	Historical incidents (0–5 scale)
📈 Example Prediction

    Input: budget=150000, duration=6, team_size=10, complexity=High, engagement=Poor, past_risk_incidents=3
    Output: Predicted Risk Level: High

📌 Requirements

    Python 3.7+

    pandas, numpy

    scikit-learn

    joblib

    streamlit

Install all dependencies with:

pip install -r requirements.txt

🙌 Credits

Developed by Akajiaku
For inquiries or collaborations: LinkedIn
GitHub: @Akajiaku1
