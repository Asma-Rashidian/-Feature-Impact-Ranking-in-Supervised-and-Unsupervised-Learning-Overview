## Feature Impact Ranking in Supervised and Unsupervised Learning

### Overview
This project is focused on evaluating the impact of various features on a labeled dataset to establish a ranking based on their influence on the output labels. The project utilizes both supervised and unsupervised learning techniques to analyze and rank features according to their importance and impact on classification results.

### Project Structure

#### 1. Data Input
- **Data Description**: The dataset contains 83 columns, including an Index column, 81 feature columns (Feature1 to Feature81), and a label column (Class Label).
- **Data Source**: [Provide the link or source of the data here]

#### 2. Data Preprocessing
- **Normalization**: All feature values will be normalized to ensure consistent scale across all features, which is crucial for accurate model performance.

#### 3. Feature Analysis
- **Correlation Analysis**: Calculate the correlation coefficient between each pair of features to identify interdependencies.
- **Visualization**: Utilize a Heat Map to visually represent the correlation coefficients between pairs of features, facilitating a clearer understanding of feature relationships.

#### 4. Unsupervised Learning
- **Feature Ranking**:
  - **K-means Clustering**: Features will be clustered and ranked according to their impact on labels, using a top-down approach based on their influence.
  - **Separate Tagging**: Perform feature ranking within each label category after segregating records based on labels.
  - **Chameleon Algorithm**: Apply this hierarchical clustering method to explore deeper structure and dependencies in the dataset.

#### 5. Supervised Learning
- **Data Balancing**: Check the balance of the dataset and apply necessary balancing techniques to prevent overfitting.
- **Model Training and Ranking**:
  - **Random Forest**: Train the model and use it to determine the importance of each feature.
  - **Feature Importance Evaluation**: Rank features based on their effectiveness as determined by the Random Forest algorithm.

#### 6. Evaluation
- **Metrics**: Evaluate models using a variety of metrics including Accuracy, F-score, Confusion Matrix, Silhouette Coefficient, AUC-ROC, Recall, and others such as RMSR, Davies-Bouldin Index, and Calinski-Harabasz Index.
- **Results Documentation**: Document all metrics in a structured table format and save them in an XLSX or CSV file named `metrics`.

#### 7. Conclusion
- **Feature Overlap**: Analyze whether there are common features that significantly influence both supervised and unsupervised learning models.
- **Rationality of Ratings**: Discuss the reasonableness of the ranking methodologies employed.
- **Method Evaluation**: If there are notable differences in the evaluation criteria results, provide an explanation.
