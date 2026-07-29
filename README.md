# 🚀 Automated Data Pipeline & EDA with AI Prompt Engineering

This project is a practical case study of **Data Analytics assisted by Artificial Intelligence**. 

As an aspiring data analyst, my goal in this repository was to design the logical architecture, define key business questions, and validate statistical outputs, using AI as an engine to generate the corresponding Python code (Pandas & Seaborn).

---

## 🎯 Project Objective
Build an interactive pipeline in Jupyter Notebook capable of processing and interpreting sales/transactional datasets **dynamically**, eliminating the need to rewrite code when column names or file structures change.

---

## 💡 Analytical & Business Logic (My Role)

Throughout development, I took full ownership of the data integrity and business logic decisions:

1. **Handling Missing Data Strategy:**
   * Identified a dataset with **52% missing values** in the quantity column (`quantity`).
   * **Decision:** Rather than blindly dropping rows (losing half of the financial insights) or imputing zeros globally (which distorts averages), I implemented a dual approach: using 100% of the records for financial metrics (`value`) and applying selective filtering/imputation for volume analysis.

2. **Automation & Adaptability (Dynamic Pipeline):**
   * Designed a **keyword-based column detector** instead of relying on static code. The notebook automatically maps columns representing `Category`, `Amount`, `Quantity`, and `Country`, preventing syntax errors (`KeyError`).

3. **Statistical Interpretation:**
   * Handled scientific notation for executive-level readability.
   * Evaluated data skewness and outliers by comparing means against percentiles (25%, 50%, 75%).

---

## 🤖 The Role of AI (Prompt Engineering)

100% of the Python code was generated iteratively using structured prompts. My workflow consisted of:
* Translating functional requirements into precise technical instructions (e.g., *"Create a function that scans column names for keywords and assigns them to variables"*).
* Interpreting execution errors (`Traceback`) and guiding the AI to resolve version or syntax conflicts.
* Validating that all visual outputs and mathematical summaries aligned with logical business sense.

---

## 🛠️ Tech Stack
* **Language:** Python 3.13
* **Environment:** Jupyter Notebook / VS Code
* **Core Libraries:** Pandas, Seaborn, Matplotlib
* **AI Partner:** Gemini (Iterative Prompting)

---

## 📂 How to Test This Project
1. Clone the repository.
2. Open `notebook.ipynb` in Jupyter Notebook.
3. Load any sales or transactional dataset (CSV or Excel) and run all cells. The column detector will automatically map the key fields.
