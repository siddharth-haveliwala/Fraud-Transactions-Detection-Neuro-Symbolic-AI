# 🛡️ Financial Fraud Detection using Neuro-Symbolic AI Approach

## Project Overview

This project presents an advanced solution for high-stakes **financial fraud detection** by pioneering a **Neuro-Symbolic Artificial Intelligence (AI)** architecture. Unlike traditional deep learning models that often act as black boxes, this hybrid approach combines the **pattern-recognition power of a Neural Network (NN)** with the **transparent, logical reasoning of symbolic rules**.

The result is a robust, highly accurate, and most importantly, **fully explainable** fraud detection system—a critical requirement in regulatory environments.

### 🧠 What is Neuro-Symbolic AI?

Neuro-Symbolic AI is a paradigm that synergistically integrates deep learning (neural networks) with symbolic reasoning (logic, rules, knowledge graphs). This approach is designed to:

* **Enhance Explainability:** Provide logical justification alongside statistical predictions.
* **Improve Reasoning:** Integrate explicit business knowledge and expert rules directly into the decision-making pipeline.
* **Achieve Robustness:** Overcome the statistical biases inherent in pure data-driven models.

## ⚙️ Technical Highlights

* **Dataset Reference**: E. A. Lopez-Rojas , A. Elmir, and S. Axelsson. "PaySim: A financial mobile money simulator for fraud detection". In: The 28th European Modeling and Simulation Symposium-EMSS, Larnaca, Cyprus. 2016

| Component | Technology | Purpose |
| :--- | :--- | :--- |
| **Neural Network (NN)** | `MLPClassifier` | The **pattern-recognition core** that identifies subtle, non-linear relationships in transactional data. |
| **Symbolic Reasoning** | Custom Logic Rules (Python) | Encodes specific **business logic**, such as the `illegal_transfer_threshold` ($200,000.0) and balance consistency checks. |
| **Feature Engineering** | Delta Features, Risk Ratios | Creation of domain-specific features like `abs_delta_orig` and `amount_over_orig` to capture suspicious activity. |
| **Model Combiner** | Logistic Regression | A final, simple model that **learns to weigh** the probability from the NN against the score from the Symbolic Rules. |

## 📂 Project Structure

```bash
.
├── src/
│   └── neuro_symbolic_fraud_detector.py  # All core code and pipeline
├── data/
│   └── synthetic_financial_dataset.csv  # Synthetic dataset (or sample)
├── notebooks/
│   └── exploratory_data_analysis.ipynb  # Visualization and key insights
├── README.md                          # Comprehensive project documentation (You are here)
├── requirements.txt                   # List of dependencies
└── LICENSE                            # MIT or other chosen license
```

### Project is in progress
