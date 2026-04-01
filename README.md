🧠 Marketing Campaign Decision Engine + LLM Analysis Pipeline

This project is an end-to-end data science + decisioning pipeline that combines large-scale SQL data extraction, feature engineering, and machine learning evaluation with LLM-powered analysis to improve marketing campaign performance.

🚀 What This Project Does
Extracts 1M+ customer-level records from SQL Server using complex campaign, quote, and behavioral joins
Builds a feature-rich dataset (100+ attributes) capturing:
Demographics
Membership & renewal behavior
Transaction/spend signals
Campaign history & engagement
Calculates marketing KPIs:
Quote rates
Direct quote performance
Mail volume trends
Runs parallelized data processing for scalability
Uses LLMs (OpenAI) to:
Audit model performance
Identify feature gaps
Generate actionable optimization strategies
📊 Key Insights & Capabilities
Handles high-volume direct mail campaigns (~40K per drop)
Tracks conversion degradation over time (declining quote rates despite stable volume)
Highlights precision vs recall tradeoffs in marketing targeting
Detects:
Overfitting (train vs test gap)
High false positive rates
Potential audience saturation
🤖 LLM-Powered Decision Layer

This project goes beyond modeling by integrating a Human-in-the-Loop (HITL) AI system:

Step 1: Model Audit
Evaluates performance metrics (AUC, recall, confusion matrix)
Diagnoses drift, targeting inefficiencies
Step 2: Feature Gap Analysis
Identifies unused predictive signals (recency, spend, engagement)
Step 3: Strategy Generation
Recommends:
Feature engineering improvements
Segmentation strategies
Campaign optimization tactics
⚙️ Tech Stack
Python (pandas, pyodbc, multiprocessing)
SQL Server (complex multi-join campaign dataset)
OpenAI API (LLM-driven analytics & reasoning)
Parallel Processing (ThreadPoolExecutor)
📈 Example Output
Monthly campaign performance:
~40K mailed records per drop
~0.28%–0.50% quote rate
Model performance:
AUC ~0.67
Recall ~76%
Precision extremely low (~0.5%) → key optimization target
🎯 Why This Matters

Traditional marketing models stop at prediction.
This system bridges the gap between:

👉 Model outputs → Business decisions → Campaign ROI

By combining:

Data engineering
Predictive modeling
LLM reasoning

…it creates a decision engine, not just a model.

🔮 Future Enhancements
Integrate real-time scoring APIs
Add causal lift / incrementality modeling
Deploy interactive dashboard (Streamlit)
Expand to multi-channel (email + digital + DM) optimization
