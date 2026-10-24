# Group 4 — Midterm Project Individual Contribution Journal

**Course:** ITAI 1371 — Introduction to Machine Learning  
**Project:** Diabetes Prediction Dataset — Data Preparation and Preprocessing  
**Group:** 4

## Member 1 — Patrick Rostand Gandjouon Tchassem

### Individual Contribution

My contribution to this project focused on developing and verifying the data preprocessing workflow using Python in Google Colab. I worked on loading and examining the original Diabetes Prediction Dataset, which contained 100,000 records, and using stratified random sampling to reduce it to 50,000 records while maintaining the original diabetes class distribution.

I also worked on splitting the sampled dataset into 35,000 training records and 15,000 testing records. I performed exploratory data analysis to examine missing values, duplicate records, class imbalance, and important features such as age, BMI, and blood glucose levels. I created visualizations using Matplotlib to compare the data before and after preprocessing.

Additionally, I worked on categorical encoding, numerical scaling, and SMOTENC class balancing. I helped create and validate the `high_bmi` feature and checked the final processed training dataset to ensure that it contained 64,050 records with an equal number of diabetes-positive and diabetes-negative cases.

Finally, I verified the final preprocessing results and exported the original training, processed training, and untouched testing datasets as CSV files for our GitHub submission.

---

## Member 2 — Kenneth Kouokam

My contribution focuses on interpreting the final data-quality checks and reviewing how the submitted files support the project requirements. The review confirms that the original split contains 35,000 training records and 15,000 testing records. After preprocessing and class balancing, the training dataset contains 64,050 records, with 32,025 examples in each diabetes class and no missing values. My section explains these results and the importance of keeping the test set separate from the preprocessing workflow. It also discusses the consistency of the engineered high_bmi feature with the BMI values in the exported dataset.

Another part of my contribution is documenting points that need attention before submission and future model training. The processed training data still contains 565 duplicate rows, so the group should explain how repeated records are handled rather than assuming that balanced data is automatically free of quality issues. The review also identifies exact record matches between the training and testing files that deserve investigation. For the documentation, I recommend updating the notebook PDF to include the final verification and export steps and shortening the proposal to the required one-page limit.


---

## Member 3 — Saimi Manasiya

My contribution to the group project focused on reviewing and interpreting the exploratory data analysis and visualizations in the diabetes dataset. I examined the graphs representing diabetes class distribution, age, BMI, and smoking history to understand the patterns present in the training data. I reviewed the class imbalance, where the majority of records belonged to patients without diabetes, and noted the concentration of BMI values around 27.32. I also examined the smoking history categories and understood why records marked as “No Info” should be treated as unknown rather than as patients who have never smoked. Additionally, I reviewed the before-and-after class distribution graphs to understand the effect of SMOTENC on balancing the training data. This work helped me understand the dataset’s characteristics, identify potential data quality concerns, and explain why EDA is an important step before training machine learning models.


---

## Member 4 — [Enter Full Name]

### Individual Contribution


---

## Member 5 — [Enter Full Name]

### Individual Contribution

