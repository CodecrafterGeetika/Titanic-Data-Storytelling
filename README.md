# Titanic Survival Analysis: A Data-Driven Story

This project moves beyond a simple prediction of survival on the Titanic. It focuses on telling a data story by engineering insightful features to answer the question: **"Beyond 'women and children first,' how did socioeconomic status and family structure create a hidden hierarchy of survival?"**



---

### ## Key Findings & Insights

-   **Social Status is Key:** The most powerful predictor of survival was not age or class, but a passenger's **social title** (Mr., Mrs., Master), which we engineered from their names. This proved to be a stronger signal than `Pclass` alone.
-   **The Family Paradox:** Passengers traveling in small families (2-4 members) had a higher survival rate than those traveling alone. However, large families (5+ members) had a very low chance of survival, likely due to the difficulty of keeping the group together.
-   **Robust Modeling:** Our final `RandomForestClassifier` model, optimized with `GridSearchCV`, achieved a reliable, cross-validated accuracy of **~83%**. This score is a trustworthy measure of its predictive power.

---

### ## Project Workflow

1.  **Data Cleaning:** Handled missing `Age` values by filling them with the median age corresponding to the passenger's social title.
2.  **Feature Engineering:** Created new, insightful features like `Title`, `FamilySize`, and `IsAlone` to add depth to the analysis.
3.  **Data Visualization:** Used `seaborn` and `matplotlib` to create plots that tell the story of how different factors influenced survival.
4.  **Modeling & Tuning:** Trained a simple model and then optimized a `RandomForestClassifier` using `GridSearchCV` to find the best settings and ensure a robust, reliable performance.

---

### ## How to Run This Project

1.  Clone this repository.
2.  The main analysis is in the `Titanic_Survival_Analysis.ipynb` notebook.
3.  The dataset used is `train.csv`.
4.  Required libraries: `pandas`, `numpy`, `seaborn`, `matplotlib`, `scikit-learn`.
