# Comparing some boosting and bagging models for (1) Continous, (2) Binary and (3) Multicategory responses: using the students performance data
## Students performance data

This dataset contains the examination scores of 1,000 students in three subjects: mathematics, reading, and writing. In addition to the test scores, it includes several demographic and socioeconomic variables, such as gender, race/ethnicity, parental level of education, lunch type, and participation in a test preparation course. The primary aim of the dataset is to investigate how factors such as family background, parental education, and test preparation influence student academic performance.

In this lecture, we use the dataset to illustrate boosting and bagging methods for three different types of response variables:

1.  **Continuous response:** We define the response variable as the student's **average score**, computed as the mean of the
    mathematics, reading, and writing scores.

2.  **Binary response:** We create a pass/fail outcome based on the average score, where students with scores from 1–49 are classified as **Fail** and those with scores from 50–100 are classified as **Pass**.

3.  **Multicategory response:** We further categorise the average score into three performance levels:

    -   **Poor:** average score \< 55,
    -   **Good:** average score between 55 and 80,
    -   **Excellent:** average score \> 80.
    
**Remark:** Each of these transformations leads to a different statistical learning problem:

-  Continuous response $\rightarrow$ regression problem  
-  Binary response $\rightarrow$ classification with two classes  
-  Multiclass response $\rightarrow$ multinomial classification  

Although the response changes, we keep the same predictor set throughout to ensure comparability across models.

These three response variables allow us to demonstrate how ensemble learning techniques such as bagging and boosting can be adapted to regression, binary classification, and multiclass classification problems within a single, coherent case study.

The dataset was obtained from the Kaggle repository and is used here solely for educational and teaching purposes. For access to the data and further details, see <https://www.kaggle.com/spscientist/students-performance-in-exams>.

