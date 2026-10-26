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

## Member 3 — Saimi Manasiya


Through this midterm project, I gained a better understanding of how Exploratory Data Analysis (EDA) helps us understand a dataset before applying machine learning algorithms. I learned that examining data through graphs, charts, and statistical information makes it easier to identify patterns, distributions, and possible data quality issues. In our diabetes dataset, we explored important features such as age, BMI, smoking history, and diabetes status. Reviewing these features helped me understand how data visualization can provide useful information about the dataset and help us make better decisions during the preprocessing stage.

One of the most important things I learned was how class imbalance can affect a machine learning project. In our training dataset, approximately 91.5% of the records belonged to people without diabetes, while only 8.5% belonged to people with diabetes. This showed me that the dataset did not have an equal distribution between the two classes. I also learned that the BMI values were concentrated around 27.32, with 8,961 records having this value. Another important observation was that many records had missing smoking-history information represented as “No Info.” I understood that these records should be treated as unknown rather than assuming those people had never smoked. These findings helped me recognize why it is important to examine the data carefully before building a model.

Finally, I learned how preprocessing techniques can improve the preparation of data for machine learning. By comparing the class distributions before and after applying SMOTENC, I understood how this technique helps balance the training data by increasing the number of minority-class examples. After balancing, both diabetes classes contained 32,025 records. I also learned the importance of applying this technique only to the training data so that the testing data remains separate for evaluating the model. Overall, this project improved my understanding of data analysis, visualization, class imbalance, and preprocessing techniques. It also helped me appreciate the importance of teamwork and clear communication when working on a machine learning project. I believe the knowledge I gained from this assignment will help me in future projects involving real-world datasets and predictive modeling.


---

## Member 4 — Anavictoria Cavazos

  After working with my group on this midterm, with the chosen dataset to work with being diabetes prediction, I would say that I have 
learned a little more now about how to actually apply what has been learned in the past assignments. This midterm just allowed me to a
ctually do each part without a task guide. I feel that with the dataset that was chosen, it was easier to follow and analyze the steps 
that had to be taken, such as splitting the data and using categorical encoding. 

  One aspect of this assignment that I would point out would be how putting into practice the learning that I have been acquiring in the 
lectures has helped me have a better understanding of certain terms or coding features and how they are used. For instance, although I 
knew that when there are categorical features they have to be turned into numerical forms, when I actually used it in the diabetes 
dataset, I was able to see basically a real-life example (aside from the previous Titanic dataset) of seeing how the gender and the 
smoking history were categories that had to be converted. 

   In addition, I also finally understood the concept of understanding the way synthetic records and real records work together. Based on 
my understanding, the use or reason for synthetic records is to bridge the gap between the minority group and the majority. See what I 
understand now that happens is that when the data has too much of one class, like, for instance, a positive result with very few that 
have an actual condition referring to medical data, then the part that actually has the condition, since it is small in comparison, is 
the minority class that gets overlooked. That is where SMOTENC and other similar algorithms come into play with this process by adding 
those synthetic records previously mentioned. So then this still left me with a small doubt of why and if it would not affect the data 
negatively, but after looking deeper into how synthetic records work, I realized it does the exact opposite. By allowing a balance in the 
data of the records, it helps have a better prediction of people who would have that condition by being able to detect patterns when that 
condition is presented. I was also able to analyze how some were duplicates in the data, but it made me also see and remember how 
sometimes it can be a real-life case where two different patients share similar health aspects. Going forward, I see how this would be a 
limitation in data, and I will keep an eye open on how that issue can be fixed and better controlled.  

   Overall, I appreciate that as each assignment is accomplished, my understanding of machine learning and using data or actually working
 with it is growing as well. I hope to use every part of this learning in future work fields as well as with other future assignments. 



---

## Member 5 — [Enter Full Name]

### Personal Reflection

