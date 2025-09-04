# 📊 Data Science Salaries — Full Analysis (2020–2023)

This summary presents detailed insights and chart-level commentary based on the analysis of the **Kaggle Data Science Job Salaries** dataset.

---

## 📈 Salary Distribution (USD)

* **Shape:** Right-skewed distribution with a long tail of high-paying jobs.
* **Typical range:** Most salaries fall between **60k–160k USD**.
* **Central tendency:** Median is more robust than the mean due to extreme outliers.

---

## 💼 Salary by Employment Type

| Type      | Insights                                                           |
| --------- | ------------------------------------------------------------------ |
| Full-time | Highest median and widest range; many outliers; dominant category. |
| Freelance | Lower but consistent pay; less volatile.                           |
| Contract  | Falls between full-time and part-time; relatively stable.          |
| Part-time | Lowest salaries; very compact distribution.                        |

---

## 🧠 Salary by Experience Level

| Level       | Insights                                                   |
| ----------- | ---------------------------------------------------------- |
| Entry-Level | Lower range, minimal spread.                               |
| Mid-Level   | Modest uplift; broader distribution.                       |
| Senior      | Substantial increase; notable variance with high outliers. |
| Executive   | Highest and most stable salaries; minimal variability.     |

---

## 🏢 Salary by Company Size

* **Medium-sized companies** offer the **highest median** salaries.
* **Large companies** have wider ranges and more outliers.
* **Small companies** provide lower but stable pay.

---

## 🕒 Salary Over Time (2020–2023)

* **2020–2021:** Salaries remained flat.
* **2022:** Notable jump in average salaries.
* **2023:** Continued growth; average reached \~150k USD.

---

## 👨‍💻 Salary by Job Titles

* **Most Common Roles:** Data Engineer, Data Scientist, Data Analyst.
* **Highest Paying Roles:** ML Engineer, Research Scientist, Applied Scientist.
* **Job Title Diversity:** Long tail of niche roles with varying pay.

---

## 🌍 Geographic Insights

* **Employee Residence (Choropleth):** US leads, followed by India, UK, and Germany.
* **Company Location:** Mirrors employee residence.
* **Average Salary by Country:**

  * Higher in Western Europe, US, and Australia.
  * Lower in Asia, Africa, and Latin America.

---

## 🏠 Remote Work (Remote Ratio)

* **Fully Remote:** Tends to pay higher on average.
* **Fully On-Site:** Also shows high salaries in some regions.
* **Partially Remote:** Slightly lower pay, more variability.

---

## 📌 Summary Takeaways

* Salary growth accelerated post-2021.
* Executive roles command the highest and most stable compensation.
* Full-time roles are more variable but offer higher ceilings.
* Data Engineer and Data Scientist dominate the market.
* Geography and remote work policies impact salaries significantly.

---

## 📊 Top Visuals Included

* Histogram of Salary Distribution
* Boxplots by Employment Type, Experience, Company Size, Remote Ratio
* Line Plot of Salary Growth Over Time
* Choropleth Maps (Residence, Company Location, Salary by Country)
* Bar/Boxplots for Job Title Frequency and Salary

---

## 🔁 Notes on Data Handling

* **Outliers:** Retained to preserve real-world variance.
* **`work_year`:** Cast to string to avoid decimal ticks.
* **Geo-coding:** Used `pycountry` to convert ISO-2 to ISO-3 codes.
* **Filtering:** Used Top-N filtering for readability (e.g., top 10 countries).

---

## 🔮 Next Steps (Advanced Exploration)

* Adjust salaries by **cost of living / PPP**.
* Train a **salary prediction model** with SHAP explainability.
* Segment by **industry** and **remote policy** for deeper insights.
* Build a public-facing dashboard using Streamlit or Power BI.

---

## 📚 Dataset Source

Kaggle: [Data Science Job Salaries 2023](https://www.kaggle.com/datasets/arnabchaki/data-science-salaries-2023)

---

## 🤝 Contributions Welcome

If you have suggestions, ideas, or improved visualizations, feel free to open a PR!
