# Estimation-of-Obesity-Levels-using-Unsupervised-Machine-Learning-Approach

# Obesity Clustering Analysis Using Unsupervised Learning

This repository contains a comprehensive analysis of obesity-related factors using unsupervised machine learning techniques. The project aims to identify natural patterns in lifestyle, dietary habits, and physical characteristics that contribute to different obesity levels.

## Project Overview

Obesity represents a significant public health challenge globally. This project employs unsupervised learning to analyze a dataset containing various physical, behavioral, and lifestyle attributes to identify natural groupings of individuals with similar characteristics and evaluate how these clusters align with known obesity levels.

### Dataset

The dataset contains information on 17 attributes for each individual:

- **Demographic Information**: Gender, Age
- **Physical Measurements**: Height, Weight
- **Family Context**: Family history with overweight
- **Eating Habits**: Frequency of high-caloric food consumption, vegetable consumption, daily meals, etc.
- **Lifestyle Factors**: Smoking status, physical activity frequency, technology usage time, transportation mode
- **Target Variable**: Obesity level (from Insufficient Weight to Obesity Type III)

## Project Goals

1. **Clustering Individuals**: Segment individuals into distinct groups based on similarities in dietary and lifestyle behaviors
2. **Understanding Cluster Characteristics**: Interpret the clusters to identify key patterns that distinguish different groups
3. **Association with Obesity Levels**: Evaluate how well the identified clusters align with known obesity levels

## Code Structure

The main script (`obesity_clustering.py`) includes:

1. **Data Loading and Preparation**
   - Loading the dataset
   - Basic data inspection

2. **Exploratory Data Analysis**
   - Distribution of obesity levels
   - Analysis of physical measurements
   - Analysis of lifestyle factors
   - Correlation analysis

3. **Data Preprocessing**
   - Feature engineering (BMI calculation, interaction terms)
   - Handling of categorical variables
   - Standardization of numerical features
   - Dimensionality reduction using PCA

4. **Clustering Individuals**
   - Determination of optimal number of clusters
   - Implementation of multiple clustering algorithms (K-Means, DBSCAN, GMM)
   - Evaluation of clustering quality using internal metrics
   - Visualization of clusters in reduced feature space

5. **Understanding Cluster Characteristics**
   - Profiling of numerical features by cluster
   - Analysis of categorical feature distributions within clusters
   - Visualization of key features across clusters
   - Detailed cluster profiles and summaries

6. **Association with Obesity Levels**
   - Calculation of external validation metrics (ARI, NMI)
   - Creation and analysis of confusion matrices
   - Comparison of mean BMI and dominant obesity level by cluster

7. **Summary and Conclusion**
   - Key findings
   - Implications for intervention strategies

## Requirements

- Python 3.7+
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

## Running the Analysis

1. Ensure you have all required packages installed:
   ```
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```

2. Place your dataset in the same directory (or update the file path in the script)


## Output

The script generates several visualization files:

- `obesity_distribution.png`: Distribution of obesity levels in the dataset
- `physical_measurements.png`: Analysis of physical measurements
- `lifestyle_factors.png`: Analysis of lifestyle factors across BMI values
- `correlation_matrix.png`: Correlation matrix of numerical features
- `optimal_clusters.png`: Determination of optimal cluster number
- `cluster_visualization.png`: Visualization of clusters in PCA space
- `cluster_characteristics.png`: Key features by cluster
- `cluster_obesity_alignment.png`: Alignment between clusters and obesity levels
- `bmi_obesity_by_cluster.png`: Comparison of mean BMI and obesity levels by cluster

## Key Findings

The analysis identifies distinct clusters of individuals with similar lifestyle and dietary patterns. Key factors differentiating these clusters include:

1. Physical activity frequency
2. Technology usage time
3. Transportation modes
4. Dietary habits (vegetable consumption, water intake)

The identified clusters show strong alignment with clinical obesity classifications, demonstrating the effectiveness of unsupervised learning for this application.

## Future Work

- Application of more advanced clustering techniques
- Incorporation of additional lifestyle factors (sleep patterns, stress levels)
- Development of targeted intervention strategies for each cluster
