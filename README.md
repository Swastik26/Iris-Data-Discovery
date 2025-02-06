# Exploratory Data Analysis on Iris Dataset

## Overview
This repository focuses on performing Exploratory Data Analysis (EDA) on the Iris dataset. The goal is to uncover meaningful insights, visualize patterns, and understand relationships between features using statistical analysis and visualizations. The dataset includes 150 samples of iris flowers from three species: Setosa, Versicolor, and Virginica, with 4 features: sepal length, sepal width, petal length, and petal width.

## Dataset
The Iris dataset contains:
- 150 rows (observations)
- 5 columns (4 features + target species)

### Features:
- **Sepal Length**: Length of the sepal (cm)
- **Sepal Width**: Width of the sepal (cm)
- **Petal Length**: Length of the petal (cm)
- **Petal Width**: Width of the petal (cm)
- **Species**: The species of the iris flower (Setosa, Versicolor, Virginica)

## Key Insights
- **Species Separation**: Setosa species is clearly distinguishable from Versicolor and Virginica, especially based on petal length and petal width. Versicolor and Virginica show some overlap.
- **Correlation**: Petal length and petal width have a very high correlation (0.96), indicating they vary similarly.
- **Distributions**: The features follow normal distributions with slight skewness in petal length and petal width, which are positively skewed.
- **Significant Differences**: Statistical analysis (ANOVA) shows significant differences in petal length and petal width between species.
- **PCA**: Principal Component Analysis (PCA) reveals that the first two components capture over 95% of the variance, suggesting the dataset can be reduced to 2D without losing important information.

## Descriptive Statistics

| Feature        | Mean   | Std. Dev | Min   | 25th percentile | Median (50th percentile) | 75th percentile | Max   |
|----------------|--------|----------|-------|-----------------|--------------------------|-----------------|-------|
| Sepal Length   | 5.843  | 0.828    | 4.3   | 5.1             | 5.8                      | 6.4             | 7.9   |
| Sepal Width    | 3.057  | 0.436    | 2.0   | 2.8             | 3.0                      | 3.3             | 4.4   |
| Petal Length   | 3.758  | 1.765    | 1.0   | 1.6             | 4.35                     | 5.1             | 6.9   |
| Petal Width    | 1.199  | 0.762    | 0.1   | 0.3             | 1.3                      | 1.8             | 2.5   |

## Visualizations
- **Pairwise Scatter Plot Matrix**: Visualizes relationships between features and highlights distinct clusters for different species.
- **Histograms**: Displays distributions of features, revealing key differences in petal length and width for Setosa vs. Versicolor and Virginica.
- **Boxplots**: Helps detect outliers and visualize distribution, with clear separation in petal length and width across species.
- **Correlation Heatmap**: Shows that petal length and petal width are strongly correlated (0.96).

## Statistical Analysis
- **Skewness**: Petal length and petal width have moderate positive skewness. Sepal length and width show nearly normal distributions.
- **Kurtosis**: The dataset shows near-zero kurtosis, indicating normal distribution shapes.
- **ANOVA**: p-values for petal length and petal width are significantly low (p < 0.05), indicating differences across species.
- **Principal Component Analysis (PCA)**: The first two principal components capture over 95% of the variance, allowing for dimensionality reduction while retaining important information.

## Outlier Detection
Using the Interquartile Range (IQR) method, minimal outliers were detected. The Setosa species shows some outliers in petal length and width, but these do not significantly affect the overall analysis.

## Conclusion
The Iris dataset is an excellent example of a simple, clean dataset for EDA. Through statistical analysis, visualizations, and feature exploration, we uncover clear distinctions between species, especially in terms of petal length and width. These insights can guide further analysis or be used for machine learning model building.

The EDA process highlights important relationships in the data, such as the high correlation between petal length and petal width, the separation of Setosa, and the normal distribution of sepal length and width. The dataset is ready for advanced modeling and classification tasks.

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy

## Installation

To run the analysis on your local machine, clone this repository and install the required dependencies:

```bash
git clone https://github.com/yourusername/iris-eda.git
cd iris-eda
pip install -r requirements.txt

