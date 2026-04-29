# SafeMedRL: Constrained Reinforcement Learning for Personalized Medical Dosage

> **Status:** Research Paper Under Review. Full source code restricted to peer-reviewers and academic collaborators.

## 📌 Project Overview
SafeMedRL is a research initiative focused on the application of **Constrained Reinforcement Learning** to optimize medical treatment dosages, specifically targeting **Type 1 Diabetes management**. The system utilizes a safety-critical agent to maintain glycemic levels within strict clinical bounds while optimizing for personalized patient response.

## 🚀 Key Features
*   **Safe-PPO Agent:** An implementation of RL techniques with a custom **Lagrangian safety layer** to prevent hypoglycemic events.
*   **LSTM-based Forecasting:** Integrated networks to predict physiological trends based on historical sensor data.
*   **Explainable AI (XAI):** A visualization module that maps RL decision pathways to clinical guidelines for physician trust.
*   **Bio-Sim Integration:** Validated against the Simglucose environment and clinical datasets.

## 🏗 System Architecture
```mermaid
graph TD
    A[Patient Data Stream] --> B[Deep Learning Predictor]
    B --> C[Safe-RL Agent]
    C --> D{Safety Constraint Layer}
    D -- Pass --> E[Recommended Dosage]
    D -- Violation --> F[Safety Override/Adjustment]
    F --> E
```

## 📊 Visualizations & Results
<img width="1390" height="1083" alt="RL_agent_vs_fixed_bbaseline" src="https://github.com/user-attachments/assets/71094da5-be2a-42e7-93da-58e47d7febb6" />
<img width="1389" height="1279" alt="24_hour_glucose_control_SAfety_Layer" src="https://github.com/user-attachments/assets/ff8b0e6c-b5c4-4719-9225-a34cfd4b841d" />
<img width="1290" height="396" alt="multi_patient_dqn" src="https://github.com/user-attachments/assets/93e00814-9cf0-4417-848d-a1be4e579011" />
<img width="1589" height="1181" alt="full_model" src="https://github.com/user-attachments/assets/7a1c5916-956a-48dd-98ee-384f0d682f7d" />
*   **Safety Adherence:** Achieved a **98%+ safety threshold** across simulated cohorts.
*   **Accuracy:** Reduced Mean Absolute Error (MAE) in dosage prediction by **14%** compared to standard baseline controllers.

## 🛠 Tech Stack
*   **Language:** Python 3.10+
*   **Core Libraries:** PyTorch, Gymnasium, NumPy, Pandas
*   **Visualization:** Three.js, GSAP 
*   **Research Tools:** OSF, LaTeX

## 🔒 Access Policy
Due to the ongoing journal submission and the sensitive nature of clinical control logic, the core training scripts and unique safety constraints are currently in a **private repository**.

**For Professors and Admissions Committees:**
I am happy to provide temporary collaborator access or a live technical walkthrough. Please contact me at **sharmaishita1097@gmail.com** to request a deep-dive.
---
