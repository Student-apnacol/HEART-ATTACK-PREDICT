# Heart Disease Data Analysis - README

## 1. Correlation Analysis

### Key Findings:
- **thalachh (Max Heart Rate Achieved) vs. Age**: Strong negative correlation (-0.39), suggesting younger individuals generally have higher max heart rates.
- **cp (Chest Pain Type) vs. output (Heart Disease Presence)**: Positive correlation (0.43), indicating that certain chest pain types are linked to a higher likelihood of heart disease.
- **oldpeak (ST Depression Induced by Exercise) vs. exng (Exercise-Induced Angina)**: Strong positive correlation (0.58), meaning patients with angina tend to exhibit higher ST depression values.

## 2. Scatter Plot Analysis

- **thalachh vs. Age**: Displays a clear downward trend, reinforcing the correlation seen in the heatmap.
- **oldpeak vs. exng**: Clustering effect observed, indicating that individuals with angina have distinct ST depression patterns.
- **chol (Cholesterol) vs. Age**: No strong trend, meaning cholesterol levels do not vary significantly with age.

## 3. Boxplot Analysis (Outliers & Distributions)

- **chol (Cholesterol levels)**: Several extreme outliers above 400 mg/dL, requiring further investigation.
- **oldpeak**: Highly right-skewed distribution, with a few extreme values that may impact model performance.
- **ca (Number of Major Vessels Colored by Fluoroscopy)**: Class imbalance observed, as most patients have 0 or 1 vessels affected.

## 4. Histogram Analysis (Feature Distributions)

- **thalachh**: Near-normal distribution with a slight left skew, indicating most patients have a high max heart rate.
- **oldpeak**: Strongly right-skewed, suggesting most individuals have low ST depression, but some have extreme values.
- **age**: Bimodal distribution, implying the dataset contains two primary age groups.

## 5. Feature Importance Analysis (Based on Model Interpretation)

### Most Predictive Features:
- **cp (Chest Pain Type)**: Strongest predictor of heart disease.
- **thalachh (Max Heart Rate Achieved)**: Significant impact, reinforcing earlier findings.
- **oldpeak**: High predictive power, suggesting that ST depression is a key diagnostic factor.

## 6. Additional Insights from Figures 6-12

- **Figure 6: Age Distribution Histogram**
  - The age distribution is bimodal, with peaks around 40-50 years and 60-70 years, suggesting two dominant patient groups.
- **Figure 7: Boxplot of Cholesterol Levels**
  - Cholesterol (chol) has several high-value outliers, particularly above 400 mg/dL, which may indicate extreme medical cases or data inconsistencies.
- **Figure 8: Relationship Between ST Depression (oldpeak) and Heart Disease (output)**
  - Higher oldpeak values (above 2.5) correlate with a higher likelihood of heart disease, confirming its diagnostic importance.
- **Figure 9: Gender-Based Heart Disease Distribution**
  - Males appear to have a higher incidence of heart disease than females, aligning with known medical trends.
- **Figure 10: Scatter Plot of Max Heart Rate (thalachh) vs. Age**
  - A clear declining trend is observed, reinforcing the correlation between younger individuals and higher heart rates.
- **Figure 11: Violin Plot of Chest Pain Type (cp) by Heart Disease (output)**
  - Certain chest pain types (cp=2 and cp=3) are strongly linked to heart disease, while cp=0 is more common in non-disease cases.
- **Figure 12: Pairplot of Key Features**
  - Clustering patterns in thalachh, oldpeak, and cp support earlier findings about their importance in heart disease prediction.
