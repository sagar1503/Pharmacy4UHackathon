# Pharmacy2U Data Hackathon 🚀
Welcome to our unified submission repository for the **Pharmacy2U Data & AI Hackathon**.

This master repository houses our complete end-to-end data pipelines, modeling notebooks, and interactive applications for the Hackathon's challenges. We utilize the 5.2 Million synthetic CMS `DE-SynPUF` dataset to build robust, predictable, and scalable healthcare AI engines.

## 📂 Repository Challenges

### [Challenge 1: Late Refill Risk Prediction](./Challenge_1/)
*   **Focus:** Predictive Modeling & Machine Learning
*   **Objective:** Identify and flag patient-drug pairs that are at a high risk of late refills, allowing Pharmacy2U to proactively intervene and improve medication adherence.
*   **Core Asset:** `Pharmacy2U_Project_A.ipynb` (End-to-End Analysis, Feature Engineering, and XGBoost Modeling workflow).

### [Challenge 2: Next-Best Recommendation Engine](./Challenge_2/)
*   **Focus:** Markov Chains, Sequence Mining & Interactive UI
*   **Objective:** Shift from reactive refills to proactive care by predicting the *next logical step* in a patient's clinical journey based on their chronic illness context (e.g. predicting a patient on Statins will need Neuropathy medication if they have Diabetes).
*   **Core Assets:** Full Python Pipeline (`02b`...`04b`), pre-trained probability graph (`markov_transitions.json`), and Live UI Simulator (`app.py`).

---

## 🛠️ How to Review our Work
To review the specifics of our implementations, please click into the specific `Challenge_1` or `Challenge_2` folders above. Each folder maintains its own detailed `README.md` with standalone setup instructions, model insights, and evaluation caveats.

**Data Requirements:** Both challenges rely on the 400MB CMS `DE-SynPUF` PDE and Beneficiary Summary synthetic datasets, which are explicitly non-versioned here to preserve repository stability.

*Built for the 2026 Pharmacy2U Data & AI Hackathon.*
