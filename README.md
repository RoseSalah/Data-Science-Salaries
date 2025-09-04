# 📊 Data Science Salaries Analysis (2020–2023)

This repository analyzes the **Data Science Job Salaries** dataset from Kaggle to understand how pay varies by **experience level, job title, employment type, company size, remote ratio, and geography**.  
The project is designed to be **clear, reproducible, and easy to review**.

---

## 📦 Dataset

- **Source:** Kaggle — *Data Science Job Salaries*  
  [🔗 Kaggle Dataset](https://www.kaggle.com/datasets/arnabchaki/data-science-salaries-2023)
- **Coverage:** 2020 → 2023  
- **Key columns:**  
  `work_year`, `experience_level`, `employment_type`, `job_title`, `salary_in_usd`,  
  `employee_residence`, `remote_ratio`, `company_location`, `company_size`.

> **Attribution:** The dataset belongs to the Kaggle author. This repo uses it for analysis & educational purposes.

---

## 🗂️ Repository Structure

DATA-SCIENCE-SALARIES/
│
├── data/ # Raw & cleaned datasets
│ ├── ds_salaries.csv
│ └── ds_salaries2.csv
│
├── notebooks/ # Jupyter notebooks
│ ├── data.ipynb # Cleaning, preprocessing
│ └── visuals.ipynb # Exploratory plots (Plotly)
│
├── outputs/ # Exported visuals
│ ├── Average Salary by Year - LinePlot.png
│ ├── Average Salary Distribution by Employee Residence Country - Choropleth.png
│ ├── Distribution of Company Size - BarPlot.png
│ ├── Distribution of Employment Type - BarPlot.png
│ ├── Distribution of Experience Level - BarPlot.png
│ ├── Distribution of Salaries (USD) - Histogram.png
│ ├── Employees Distribution by Company Location - Choropleth.png
│ ├── Employees Distribution by Employee Residence Country - Choropleth.png
│ ├── Job Titles Distribution by Country (Top 10 Countries) - Histogram.png
│ ├── Job Titles Word Count.png
│ ├── Salary by Experience Level and Employment Type - BoxPlot.png
│ ├── Salary Distribution by Company Size - BoxPlot.png
│ ├── Salary Distribution by Employment Type - BoxPlot.png
│ ├── Salary Distribution by Experience Level - BoxPlot.png
│ ├── Salary Distribution by Remote Ratio - BoxPlot.png
│ ├── Salary Distribution for Top 15 Job Titles - BoxPlot.png
│ └── Top 15 Most Common Job Titles - BarPlot.png
│
├── summary.md # concise findings
├── requirements.txt # dependencies
└── README.md # this file


---

## ⚙️ Environment & Requirements

```bash
python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt

## 🚀 How to Run

Open in **VS Code** (recommended) with the **Jupyter extension**.

Run step by step:

- `notebooks/data.ipynb` → cleaning & preprocessing.  
- `notebooks/visuals.ipynb` → generate visuals & insights.  

---
## 🔎 Sample Visuals

| 📊 Distribution of Salaries (USD) | 🌍 Average Salary by Country |
|----------------------------------|------------------------------|
| ![Salary Histogram](outputs/Distribution%20of%20Salaries%20(USD)%20-%20Histogram.png) | ![Average Salary by Country](outputs/Average%20Salary%20Distribution%20by%20Employee%20Residence%20Country%20-%20Choropleth.png) |

| 💼 Salary by Experience Level | 👨‍💻 Salary by Job Title |
|------------------------------|--------------------------|
| ![Salary by Experience](outputs/Salary%20Distribution%20by%20Experience%20Level%20-%20BoxPlot.png) | ![Salary by Job Title](outputs/Salary%20Distribution%20for%20Top%2015%20Job%20Titles%20-%20BoxPlot.png) |

➡️ See [`summary.md`](summary.md) for full insights and chart commentary.

---

## 📌 Key Highlights

- 📈 **Salary growth** accelerated post-2021, peaking in 2023 (~150k USD average).
- 🧠 **Experience** plays a major role — Executives earn the most, with stable salaries.
- 💼 **Full-time roles** show higher potential but also wider variability.
- 🌎 **The US leads** in both employee and company counts.
- 🌐 **Fully remote and fully on-site** jobs pay more than partially remote ones.

---

## 🛠️ Reproducibility Notes

- Convert `work_year` to **string** before plotting (avoids decimal ticks like `2020.5`).
- Use `pycountry` to convert **ISO-2 to ISO-3** codes for choropleth maps.
- Apply **Top-N filtering** to avoid clutter in visualizations (e.g., top 10 countries).
- **Outliers** are retained to reflect real distributions — use **medians** for fair comparisons.

---

## 🧭 Suggested Next Steps

- Adjust salaries for **cost of living / PPP** to improve cross-country comparison.
- Train a **salary prediction model** (e.g., Linear Regression or GBM with SHAP).
- Segment by **industry** and **remote policy** for deeper insights.
- Publish an **interactive dashboard** (Streamlit / GitHub Pages / Power BI, etc.).

---

## 🛡️ License & Attribution

- **Code:** MIT License (or your preferred open-source license).
- **Data:** Courtesy of the [original Kaggle dataset author](https://www.kaggle.com/datasets/arnabchaki/data-science-salaries-2023) — please follow their terms for reuse.

---

## 🤝 Contact

Have questions or suggestions?

- Open an **issue** on this repository.
- **Pull Requests** improving code, visuals, or documentation are highly welcome! 🚀
