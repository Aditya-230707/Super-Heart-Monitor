Project Architecture

                       Streamlit UI (app/)
                       ├── Interference agent
                             │
                             ├── Data Agent ──── Clinical Dataset(kaggle)
                             ├── Training Agent ──── ML models (XGBoost)
                             └── monitor Agent ──── Drift/Quality Logs
                     

Repository Structure

                       [Super-Heart-Monitor/]
                       │
                       ├── app/
                       │   └── streamlit_app.py
                       │
                       ├── src/
                       │   ├── agent_runner.py
                       │   ├── data_agent.py
                       │   ├── training_agent.py
                       │   ├── inference_agent.py
                       │   └── utils.py
                       │
                       ├── architecture.png
                       │
                       ├── requirements.txt
                       │
                       └── README.md

Model Training Layer

Model training uses:

  XGBoostClassifier — selected for:
  
	•	Handling imbalance
	•	High accuracy
	•	Gradient boosting
	•	Industry-tested reliability

  Preprocessing:
  
	•	StandardScaler
	•	OneHotEncoder
	•	FeatureUnion / ColumnTransformer

Tools & Technologies

🔹 Python

🔹 Streamlit (for front-end UI)

🔹 XGBoost / Scikit-learn (ML models)

🔹 Pandas, NumPy (data processing)

🔹 Agentic pipeline (custom python agents)

🔹 Google AI Tools Used

 • Google Colab
 • Google Gemini API

🔹Chat GPT

SetUp instruction

1. Clone the Repo
   
   git clone https://github.com/<Aditya-2030707>/Super-Heart-Monitor.git cd Super-Heart-Monitor

2. Install dependencies
   
   pip install -r requirements.txt

3. run the app
   
   steamlit run/steamlit_app.py

LICENSE

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
