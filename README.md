# \# Student-Employability-EDA

# An exploratory data analysis of soft skills and student academic performance as predictors of student employability. 

# \### Dataset

# Student Employability Dataset (Hamoutni, 2022) is composed of 2,982 mock interview records across Philippine universities. Eight factors are rated from 1 to 5 with a binary employability classification.

# \## Research Questions

# 1\. Which individual factor is most strongly associated with students being classified as Employable?

# 2\. Which factors demonstrate the strongest associations with Employability? 

# 3\. Is Student Performance Rating significantly associated with Employability?

# 4\. Do soft skill factors exhibit multicollinearity, and does combining them (via PCA or composite scoring) improve prediction?

# 5\. Do combinations of factors reveal effects on employability that aren't visible when looking at each factor individually?

# \## Key Findings

# 1\. `mental\_alertness` has the strongest association with employability: 77.15% of students rated 5 are employable, while a rating of 2 gives a 75.76% chance of being less employable.

# 2\. `mental\_alertness` and `manner of speaking` have the highest (but weak) correlations with employability (ρ < 0.20). No single soft skill factor is strongly predictive; employability likely depends on multiple factors or external variables.

# 3\. Academic performance ratings show little to no correlation with soft skills or employability, contradicting the belief that good grades predict career success.

# 4\. The soft skill factors are highly interrelated (severe multicollinearity). Combining them resolves this problem, but neither PCA nor composite scores outperform mental alertness alone in predicting employability.

# 5\. The pivot analysis of `mental\_alertness` and `manner\_of\_speaking` reveals non-linear effects: some rating combinations (e.g., (3,3)) yield better employability rates than higher scores (e.g., (4,4)), highlighting that specific combinations matter more than individual high scores.

# \## Tools Used

# \- Python, pandas, NumPy

# \- matplotlib, seaborn (visualization)

# \- statsmodels (VIF)

# \- scikit-learn (PCA, StandardScaler)

# \## Repository Structure

# ```

# .

# ├── data/

# │   └── Student-Employability-Datasets.xlsx

# ├── notebooks/

# │   └── EDA - Students Employability.ipynb

# ├── requirements.txt

# └── README.md

# ```

# \## Running Locally

# ```bash

# git clone https://github.com/amieltongco/Students-Employability-EDA

# cd https://github.com/amieltongco/Students-Employability-EDA

# pip install -r requirements.txt

# jupyter notebook notebooks/"EDA - Students Employability.ipynb"

# ```

# Ensure `Student-Employability-Datasets.xlsx` is in the `data/` directory, or update the file path in the corresponding cell to match your local setup.

# \## References

# \- Franke, G. R. (2010). Multicollinearity. \_Wiley International Encyclopedia of Marketing\_. \[https://doi.org/10.1002/9781444316568.wiem02066](https://doi.org/10.1002/9781444316568.wiem02066)

# \- Hamoutni, A. (2022). \_Students Employability Dataset\_, Version 1. \[https://www.kaggle.com/datasets/anashamoutni/students-employability-dataset/version/1](https://www.kaggle.com/datasets/anashamoutni/students-employability-dataset/version/1)

