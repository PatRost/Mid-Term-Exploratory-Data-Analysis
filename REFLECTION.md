# Group 4 — Midterm Project Reflection Journal

**Course:** ITAI 1371 — Introduction to Machine Learning  
**Project:** Diabetes Prediction Dataset — Data Preparation and Preprocessing  
**Group:** 4

## Member 1 — Patrick Rostand Gandjouon Tchassem

### Personal Reflection

Working on the Diabetes Prediction Dataset helped me understand how important data preparation is before training machine learning models. I learned how to use Python in Google Colab to explore a dataset, check for missing values and duplicate records, and create visualizations to understand patterns in the data. I also learned how stratified sampling works and why we divided our dataset into 70% training data and 30% testing data.

One of the most interesting parts of this project was learning how to handle imbalanced data. Our dataset had significantly more patients without diabetes than patients with diabetes. By using SMOTENC, we balanced the training dataset while keeping the testing dataset unchanged. I also gained experience with categorical encoding, numerical scaling, and feature engineering by creating a new `high_bmi` feature.

One challenge was making sure the preprocessing steps were performed correctly and that the final dataset contained no missing values or inconsistent features. This project helped me improve my Python skills, understand the importance of preventing data leakage, and feel more confident preparing datasets for future machine learning models.

---

## Member 2 — Kenneth Russel Kouokam Meli

This project shows me that preparing data for machine learning involves more than making a file load successfully or removing empty cells. A dataset can contain no missing values and still have issues that deserve attention. Looking at the final quality checks helps me connect the preprocessing steps to their purpose: making the data understandable, checking its consistency, and preparing for a fair evaluation later.

The separation between training and testing data is especially important. Our sampled dataset contains 50,000 records, divided into 35,000 training records and 15,000 testing records. The training data is used to explore patterns and determine preprocessing choices. Keeping the testing data separate protects its role as a later check on model performance. The exact record matches found across the two files raise a useful question about whether repeated information could affect that evaluation. Without patient identifiers, matching values alone cannot tell us whether the records describe the same person.

Class balancing also requires careful interpretation. The original training data contains far more records without diabetes than with diabetes. SMOTENC increases the minority class so that both classes contain 32,025 records. These additional examples are synthetic, rather than newly collected patient records. This distinction matters because a larger, balanced dataset does not automatically mean a model will perform better. That will need to be tested during the final project.

The high_bmi feature illustrates why creating a new column should be followed by validation. Its definition depends on whether BMI is at least 30 in the original units. Since BMI is standardized during preprocessing, checking that rule requires recovering its original scale. The notebook documents inconsistencies after synthetic sampling and corrects them through Python. This helps me understand that a feature can contain valid values such as zero and one while still being inconsistent with the information it represents.

My main takeaway is that final review is part of the technical work. The remaining duplicate rows need an explanation, and the documents should accurately show the completed workflow. An outdated PDF or an oversized proposal can make otherwise substantial work harder to assess. For future projects, I want to pay attention to both the data checks and the evidence presented in the submission. Good preparation means understanding what changed, why it changed, and what limitations still remain.


---

## Member 3 — [Enter Full Name]

### Personal Reflection


---

## Member 4 — [Enter Full Name]

### Personal Reflection


---

## Member 5 — [Enter Full Name]

### Personal Reflection

