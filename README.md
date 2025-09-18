# Bitcoin-Forecast-XGB-Compass.Ai-
🧭 Using AI to find the true north in Bitcoin's price direction. A quant research project with XGBoost &amp; SHAP
📈 Bitcoin Price Direction Prediction with XGBoost
Can machine learning cut through the noise of crypto markets? This project explores that question by building a model to predict the 30-day price direction of Bitcoin.

This repository is a deep dive into quantitative research, fusing on-chain metrics, social sentiment, and macroeconomic indicators to train a highly-tuned XGBoost model. The goal isn't just to predict, but to understand the why behind the market's movements using explainable AI.

✨ Key Features
🧠 Intelligent Modeling with XGBoost: Leverages the power of gradient boosting to capture complex, non-linear relationships between diverse features.

⚙️ Advanced Hyperparameter Tuning: Employs Optuna across 500 trials to rigorously optimize the model, ensuring peak performance.

📊 Demystifying the 'Why' with SHAP: Moves beyond a "black box" approach by using SHAP (SHapley Additive exPlanations) to visualize and understand which factors are driving the model's predictions.

⏳ Robust Time-Series Validation: Uses a 5-fold TimeSeriesSplit cross-validation to train the model, strictly preventing look-ahead bias and ensuring the results are realistic.

📂 What's Inside?
This repository provides everything you need to understand and replicate the core of this research:

btc_insight.py: The main Python script containing the entire workflow—data preprocessing, model training, Optuna optimization, and SHAP analysis.

sample.csv: A sample of the dataset (the last 10 rows) to illustrate the required data structure for the model.

optuna_output_log.txt: A detailed log from the 500-trial hyperparameter tuning session, showcasing the optimization process and best-performing parameters.

📊 The Dataset
The model was trained on a comprehensive dataset spanning from August 2022 to September 2025. This timeframe was chosen to incorporate crucial on-chain data like exchange reserves, which became available in late 2022.

Features include:

On-Chain Metrics: NUPL, SOPR, Miner Flows, Exchange Reserves

Macroeconomic Indicators: DXY, CPI, Federal Reserve Interest Rates

Social Data: Social media sentiment scores

Note: Due to privacy and licensing constraints, the full dataset cannot be published. The provided sample.csv is intended to demonstrate the data schema.

🚀 Getting Started
You can run a demonstration of the model on the sample data.

Clone the repository:

Bash

git clone https://github.com/imaroraanmol/Bitcoin-Forecast-XGB-Compass.AI.git
cd Bitcoin-Forecast-XGB.Compass.AI
Install the dependencies:

Bash

pip install -r requirements.txt
Run the script:

Bash

python btc_insight.py
(Note: Running with sample.csv is for demonstration only; the results will not be meaningful with such a small dataset.)

📈 Results & Key Insights
The final optimized model achieved 62.1% accuracy on the test set, with an impressive 91% recall for upward price movements, making it particularly effective at identifying potential bull runs.

Most interestingly, the SHAP analysis uncovered several counterintuitive relationships between Bitcoin's price and macro factors. The model learned non-linear patterns related to the USD Index (DXY) and CPI inflation surprises that challenge conventional wisdom.

For a full breakdown of the model's performance and a deep dive into these insights, please see the detailed write-up:

➡️ Read the Full Analysis on LinkedIn

⚠️ Disclaimer
This project is for educational and research purposes only. The information and results presented here are not financial advice. Trading cryptocurrencies involves significant risk of financial loss.

📫 Connect & Collaborate
Have questions, ideas, or want to collaborate on a project? Feel free to reach out to me on LinkedIn.
