# Yulu---Hypothesis-Testing-Jul-2024-

# 🚲 Yulu: Hypothesis Testing  

## 📌 About Yulu  
Yulu is India’s leading micro-mobility service provider, offering innovative solutions for daily commutes. With a mission to reduce traffic congestion, Yulu provides shared, solo, and sustainable commuting options through its mobile app. Yulu zones are strategically located near metro stations, bus stands, office spaces, and residential areas to ensure seamless first- and last-mile connectivity.  

## 🎯 Business Problem  
Yulu has recently experienced a significant dip in revenue. To address this, they have partnered with a consulting firm to analyze the factors influencing the demand for shared electric cycles in the Indian market.  

### 🔍 Objectives  
- Identify significant variables that impact the demand for shared electric cycles.  
- Determine how well these variables explain the fluctuations in demand.  

## 📂 Dataset  
📌 **Dataset Name:** `yulu_data.csv`  

### 🏷️ Column Profiling  
| Column | Description |  
|--------|------------|  
| `datetime` | Timestamp of the record |  
| `season` | Season (1: Spring, 2: Summer, 3: Fall, 4: Winter) |  
| `holiday` | Whether the day is a holiday (Yes/No) |  
| `workingday` | Whether the day is a working day (1: Yes, 0: No) |  
| `weather` | Categorical variable describing weather conditions: <br>1: Clear/Partly Cloudy <br>2: Mist/Cloudy <br>3: Light Snow/Rain <br>4: Heavy Rain/Snow |  
| `temp` | Temperature (°C) |  
| `atemp` | Feels-like temperature (°C) |  
| `humidity` | Humidity percentage |  
| `windspeed` | Wind speed |  
| `casual` | Number of casual users |  
| `registered` | Number of registered users |  
| `count` | Total rental bike count (casual + registered) |  

## 🧪 Concepts Used  
- **Bivariate Analysis**  
- **Two-Sample T-Test** (Comparing means across two populations)  
- **ANOVA** (Analysis of Variance)  
- **Chi-Square Test** (Checking dependency between categorical variables)  

## 🚀 Approach & Methodology  
### 🔹 **Exploratory Data Analysis (EDA)**  
✔ Import dataset and examine structure & missing values.  
✔ Convert categorical attributes for better visualization.  
✔ Perform univariate analysis (distribution of numeric & categorical features).  
✔ Conduct bivariate analysis (relationships between key variables).  

### 🔹 **Hypothesis Testing Steps**  
1. Define the **Null Hypothesis (H₀)** and **Alternate Hypothesis (H₁)**.  
2. Choose the appropriate statistical test:  
   - **T-Test**: Impact of working days on bike rentals.  
   - **ANOVA**: Comparing rental demand across different seasons & weather conditions.  
   - **Chi-Square Test**: Checking dependency between weather and season.  
3. Validate test assumptions:  
   - **Normality** (Histogram, Q-Q plot, Shapiro-Wilk test)  
   - **Equal Variance** (Levene’s test)  
4. Compute **test statistics** & **p-value**.  
5. Decision-making: **Accept or Reject H₀**.  
6. Derive **business insights** from the results.  

## 📊 Evaluation Criteria (50 Points)  
### ✅ **1. Problem Definition & EDA (10 points)**  
✔ Clearly define the problem.  
✔ Perform univariate & bivariate analysis.  
✔ Generate insights from data distributions & relationships.  

### ✅ **2. Hypothesis Testing (30 points)**  
✔ **T-Test** for working day impact (10 points).  
✔ **ANOVA** for seasonal & weather variations (10 points).  
✔ **Chi-Square** for dependency between weather and season (10 points).  

### ✅ **3. Notebook Quality (10 points)**  
✔ Structured analysis with well-commented code.  
✔ Visualizations to support conclusions.  

## 📈 Insights & Key Findings  
✔ **No significant difference** in bike rentals between working and non-working days.  
✔ **Strong seasonal impact**: Demand varies significantly across different seasons.  
✔ **Weather plays a crucial role**: Clear/mist conditions see higher demand, while heavy rain reduces usage.  
✔ **Weather and season are statistically dependent**: Chi-square test confirms correlation.  

## 🔍 Business Recommendations  
### 📌 **Data-Driven Insights**  
- **Spring season** shows the highest demand; marketing campaigns should focus on this period.  
- **Lack of data in heavy rain conditions**: More data collection is needed to refine business strategies.  
- **Dynamic pricing**: Introduce surge pricing based on demand patterns.  
- **Loyalty program**: Reward registered users to improve retention.  
- **University partnerships**: Deploy more cycles in high-footfall areas like campuses.  

### 📌 **Strategic Improvements**  
- **Introduce rain-resistant bikes** with protective covers.  
- **Seasonal promotions** to boost demand during off-peak periods.  
- **Expand social media marketing** to reach a broader audience.  
- **Improve inventory management** based on demand patterns.  
- **Host cycling marathons/events** to increase brand visibility.  

## 🛠️ Tools & Technologies  
- **Python**: `Pandas`, `NumPy`, `Matplotlib`, `Seaborn`, `SciPy`  
- **Statistical Methods**: T-Test, ANOVA, Chi-Square Test  
- **Visualization**: Histograms, Boxplots, Heatmaps
