# Exploratory Data Analysis (EDA) on Titanic Dataset

## 🎯 Objective
To understand the Titanic dataset using statistical analysis and data visualizations, identifying patterns, trends, and anomalies that provide insights into passenger survival factors.

## 📊 Dataset Information
- **Dataset**: Titanic Dataset
- **Source**: Classic machine learning dataset containing passenger information from the RMS Titanic
- **Size**: 891 passengers with 12 features
- **Target Variable**: Survived (0 = No, 1 = Yes)

## 🛠️ Tools & Libraries Used
- **Python 3.x**
- **Pandas** - Data manipulation and analysis
- **Matplotlib** - Basic plotting and visualization
- **Seaborn** - Statistical data visualization
- **NumPy** - Numerical computations


## 🔍 Analysis Performed

### 1. **Data Overview**
- Dataset shape and basic information
- Data types identification
- Missing values assessment
- Summary statistics generation

### 2. **Statistical Analysis**
- **Descriptive Statistics**: Mean, median, standard deviation, quartiles
- **Missing Data Analysis**: Identified missing values in Age (177), Cabin (687), and Embarked (2)
- **Distribution Analysis**: Examined skewness in numerical features

### 3. **Data Visualization**
- **Histograms**: Distribution of numerical features (Age, Fare, etc.)
- **Box Plots**: 
  - Age distribution and outlier detection
  - Fare distribution by passenger class
- **Correlation Matrix**: Relationships between numerical features
- **Pair Plots**: Feature relationships with survival outcomes
- **Count Plots**: 
  - Overall survival distribution
  - Survival by gender

## 📈 Key Findings & Insights

### Survival Patterns
- **Overall Survival Rate**: ~38% of passengers survived
- **Gender Impact**: Females had significantly higher survival rates than males
- **Class Influence**: First-class passengers had better survival chances compared to lower classes

### Data Distribution Insights
- **Age**: Shows right skewness with outliers, missing for ~20% of passengers
- **Fare**: Highly right-skewed with extreme outliers, indicating varied ticket prices
- **Class Distribution**: Third class had the most passengers, first class the least

### Feature Relationships
- **Positive Correlation**: Fare and survival show weak positive correlation
- **Class-Fare Relationship**: Higher classes generally paid higher fares
- **Age-Survival**: No strong linear relationship observed

### Data Quality Observations
- **Missing Data**: Significant missing values in Cabin (77%), Age (20%)
- **Outliers**: Present in both Age and Fare columns
- **Data Skewness**: Both Age and Fare show positive skew

## 🎯 Business Insights
1. **"Women and Children First"**: The data strongly supports the maritime evacuation protocol
2. **Socioeconomic Factors**: Higher class passengers had better access to lifeboats
3. **Fare Disparity**: Significant variation in ticket prices even within same class

## 🔧 Technical Implementation

### Code Structure
```python
# Data Loading & Basic Info
- pd.read_csv() for data import
- df.info(), df.describe() for overview
- df.isnull().sum() for missing value analysis

# Visualizations
- plt.hist() for distribution analysis
- sns.boxplot() for outlier detection
- sns.heatmap() for correlation analysis
- sns.pairplot() for feature relationships
- sns.countplot() for categorical analysis
```
## SnapShots 
![image](https://github.com/user-attachments/assets/905b88be-8044-43ba-af57-bd8dbdbcc797)
![image](https://github.com/user-attachments/assets/96bd965c-8600-4233-9154-b9b58fbc23ff)
![image](https://github.com/user-attachments/assets/1b1045d7-6f96-4983-8489-cf4910a5aa7c)
![image](https://github.com/user-attachments/assets/dd201978-0292-413a-8a6a-a1f97b1e9908)
![image](https://github.com/user-attachments/assets/a125613e-f61c-4ab9-adb5-5f837bc0bfa5)
![image](https://github.com/user-attachments/assets/d3ee589d-0384-41e3-8a12-6f95152856a6)
![image](https://github.com/user-attachments/assets/827f3a86-25fb-4ff4-a6c1-462ca60ec6cc)


## 📚 What I Learned
- **Data Visualization Techniques**: Creating meaningful plots to understand data patterns
- **Descriptive Statistics**: Calculating and interpreting summary statistics
- **Pattern Recognition**: Identifying trends and anomalies in real-world data
- **Feature Relationships**: Understanding correlations and associations between variables
- **Data Quality Assessment**: Detecting missing values, outliers, and distribution issues

## 🚀 Potential Next Steps
1. **Data Preprocessing**: Handle missing values and outliers
2. **Feature Engineering**: Create new features from existing ones
3. **Advanced Visualizations**: Interactive plots using Plotly
4. **Statistical Testing**: Hypothesis testing for survival factors
5. **Predictive Modeling**: Build machine learning models for survival prediction

## 📋 EDA Interview Questions Preparation

### Questions Covered in This Analysis:
1. **Purpose of EDA**: Understanding data structure, quality, and patterns before modeling
2. **Boxplots Usage**: Identifying outliers, quartiles, and distribution shape
3. **Correlation Analysis**: Measuring linear relationships between numerical features
4. **Skewness Detection**: Using histograms and statistical measures
5. **Visualization Role in ML**: Pattern discovery and feature understanding

## 🔗 How to Run
1. Clone this repository
2. Install required libraries: `pip install pandas matplotlib seaborn`
3. Run the script: `python titanic_eda.py`
4. View generated visualizations

## 📊 Dataset Features
- **PassengerId**: Unique identifier for each passenger
- **Survived**: Survival status (0 = No, 1 = Yes)
- **Pclass**: Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd)
- **Name**: Passenger name
- **Sex**: Gender
- **Age**: Age in years
- **SibSp**: Number of siblings/spouses aboard
- **Parch**: Number of parents/children aboard
- **Ticket**: Ticket number
- **Fare**: Passenger fare
- **Cabin**: Cabin number
- **Embarked**: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

---

**Task Completed**: AI & ML Internship - Task 2: Exploratory Data Analysis  
**Submission Date**: [Current Date]  
**Tools Used**: Python, Pandas, Matplotlib, Seaborn
