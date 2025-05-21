# _DSA210-Term Project_

I am Zeynep Bilici, a CS student at Sabancı University, and this is my DSA210 term project. The goal of this project is to analyze data from the Starbucks Mobile App to examine how my coffee consumption changes during the school period based on my course load and exam schedules. I collected the data manually.

---

# _Contents_
- [Motivation](#motivation)
- [Project Goal](#project-goal)
- [Data and Data Analysis](#data-and-data-analysis)
- [Files](#files)
- [Google Colab Link](#google-colab-link)
- [Methods and Analysis](#methods-and-analysis)
- [Interpretation of Results](#interpretation-of-results)
- [Machine Learning](#machine-learning)
- [Findings and Visualization](#findings-and-visualization)

---

# _Motivation_

Since I know that over caffeine consumption can be harmful to health, I wanted to analyze my coffee consumption during school periods. By analyzing the results, I aim to use this project to support my well-being and health. I also want to explore how my coffee habits change on days with varying course loads and during exam weeks.

---

# _Project Goal_

The goal of this project is to analyze my coffee consumption data from the Starbucks Mobile App to identify patterns based on my course load and exam periods. I aim to examine the relationship between academic stress and caffeine consumption, and evaluate whether my habits align with healthy intake limits.

---

# _Data and Data Analysis_

The dataset consists of manually collected records from the Starbucks Mobile App and SuCourse. Some weeks in the weekly graph have 0 coffee consumption, meaning no coffee was consumed during those weeks. This is a valid behavioral finding rather than a data collection issue.

Each record includes the following fields:
- **Date:** The date when the coffee was purchased
- **Coffee Type:** The type of coffee ordered
- **Coffee Number:** The number of coffees bought on that day
- **Caffeine Amount (mg):** The estimated total caffeine intake
- **Course Load (min):** The total number of minutes spent in classes that day
- **Exam Number (that week):** The number of exams during the corresponding week

---

# _Files_
- `raw_data`: Manually collected data
- `code.ipynb`: Python code for data cleaning, EDA, hypothesis testing, and machine learning

---

# _Google Colab Link_

[Google Colab Notebook](https://colab.research.google.com/drive/1A7vcgjbd5rBE3E2kaYBdlZm9FjZdaxjZ?usp=sharing)

---

# _Methods and Analysis_

### 1. Data Cleaning
- Converted date and numeric fields to correct formats
- Checked for missing values (very few found)

### 2. Exploratory Data Analysis (EDA)
- **Time Series Plot**: Daily coffee consumption over the semester
- **Bar Graph**: Average consumption in exam vs. non-exam weeks
- **Boxplot**: Coffee consumption based on course load category
- **Correlation Matrix Heatmap**: Relationship among variables
- **Weekly Consumption Plot**: Weekly average using resampled timeline

### 3. Hypothesis Testing

#### Hypothesis 1: Exam Weeks vs Normal Weeks
- **Test**: Independent Samples t-test
- **Result**: p = 0.012 → There is a statistically significant increase in coffee consumption during exam weeks.

#### Hypothesis 2: Coffee Consumption by Course Load
- **Test**: One-way ANOVA
- **Result**: p = 0.43 → There is no statistically significant difference in coffee consumption across different course load categories.

---

# _Interpretation of Results_

- **Exam Weeks**: The t-test result indicates that I tend to drink significantly more coffee during exam weeks, suggesting a link between academic pressure and caffeine intake.
- **Course Load**: The ANOVA analysis showed no statistically significant difference in coffee consumption among low, medium, and high course load days, which suggests that daily workload may not strongly influence my caffeine habits.

---

# _Machine Learning_

To complete the full data science pipeline, a **Linear Regression model** was trained to predict daily coffee consumption.

- **Goal**: Estimate the number of coffees consumed on a given day
- **Features Used**:
  - `Course Load (min)`
  - `Exam Number (that week)`
  - `Day of the Week`
- **Target Variable**: `Coffee Number`

### Results:
- **Mean Squared Error (MSE)**: 0.768
- **R² Score**: 0.611

A scatter plot was generated to visualize the actual vs. predicted coffee consumption values. The model provides insights into how academic variables impact caffeine intake and demonstrates how simple machine learning models can be applied to personal behavior data.

---

# _Findings and Visualization_

1. **Time Series Plot: Daily Coffee Consumption**
   - Reveals fluctuations in daily caffeine consumption.
   - Peaks align with exam periods or stressful academic weeks.

2. **Bar Graph: Average Coffee Consumption – Exam Week vs. Normal Week**
   - Shows a clear increase in average coffee consumption during exam weeks.
   - Visual support for Hypothesis 1.

3. **Boxplot: Coffee Consumption by Course Load Category**
   - Displays distribution across `Low`, `Medium`, and `High` course load.
   - Median values are relatively similar, consistent with ANOVA results.

4. **Correlation Matrix Heatmap**
   - Identifies relationships among key numeric variables.
   - Suggests mild positive correlation between course load and coffee intake.

5. **Line Plot: Weekly Average Coffee Consumption**
   - Shows trends and seasonality across the semester.
   - Highlights exam-related peaks and periods of no coffee consumption.
