#How the missing data should be handled and the potential impact of the class distribution on tree splitting:
1. Missing Value Analysis: Initial analysis shows zero null/missing values in the dataset. However, a frequency check revealed "noisy" data in the target variable.

2. Data Consistency Issue: The income column contains duplicate labels due to trailing periods. These should be merged so that we do not have similar data and to ensure the model correctly identifies the two primary classes.

3. Class Distribution: After accounting for the noise, we find out that the dataset is imbalanced. Approximately 74.7% of the data belongs to the <=50K class, while only 25.3% belongs to the >50K class.

4. Impact on Tree Splitting: This distribution, which is roughly of 3:1 ratio, can lead to bias in Decision Trees making it imbalanced. The tree might over-optimize for the majority class to minimize Gini Impurity, potentially leading to poor precision for the >50K group.

#Analysis Methodology
I used pandas to read dataset.csv file.
To check for missing values I used df.isnull().sum()
And to check income column balance I ran value_counts which helped me notice that the data was dirty and unbalanced.
