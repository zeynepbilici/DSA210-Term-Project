# _DSA210-Term Project_
I am Zeynep Bilici, a CS student at Sabancı University, and this is my DSA210 term project. The goal of this project is to analyze data from the Starbucks Mobile App to examine how my coffee consumption changes during the school period based on my course load and exam schedules. I will collect the data from the Starbucks Mobile App manually.

---

# _Contents_
- [Motivation](#motivation)
- [Project Goal](#project-goal)
- [Data and Data Analysis]((#data-and-data-analysis )
- [Files]((#files )
- [Google Collab Link]((#google-collab-link )
- [Findings and Visualization]((#findings-and-visualization )

---

# _Motivation_
Since I know that over caffeine consumption can be harmful to health, I wanted to analyze my coffee consumption during periods of school time. By analyzing the results, I aim to use this project in a way that benefits my well-being and health. Additionally, I want to analyze the patterns in my coffee consumption on days with a low or high course load, as well as on weeks when I have exams.

---

# _Project Goal_
The goal of this project is to analyze my coffee consumption data from the Starbucks Mobile App to identify the patterns based on my course load and exam periods. My purpose is to find the interaction between higher stress and busier school schedule with caffeine consumption. I aim to determine whether my coffee consumption habits align with healthy limits or not. 

---

# _Data and Data Analysis_
The dataset consists of manually collected records from the Starbucks Mobile App and SuCourse website.
Each record includes the following fields:
- **Date:** The date when the coffee was purchased
- **Coffee Type:** The type of coffee ordered
- **Coffee Number:** The number of coffees bought on that day
- **Caffeine Amount (mg):** The estimated total caffeine intake
- **Course Load (min):** The total number of minutes spent in classes that day
- **Exam Number (that week):** The number of exams during the corresponding week
The data was collected over the course of one academic semester to investigate the relationship between academic stress (course load, exams) and coffee consumption habits.
---

# _Files_
- `raw_data`: Manually collected data
- `code.ipynb`: Python code for data cleaning, exploratory data analysis (EDA), and hypothesis testing.

---

# _Google Collab Link_
https://colab.research.google.com/drive/1Lf23-suBLmbRgzYGmnocHuiQYjTNDKQB?usp=sharing

---

# _Findings and Visualization_
1. Time Series Plot: Daily Coffee Consumption
This plot shows the number of coffees consumed on each day throughout the semester.
The purpose is to observe general trends over time, such as whether coffee consumption spikes during specific periods like exam weeks or high workload days.
Fluctuations in the graph indicate varying levels of caffeine demand, possibly influenced by academic stress or workload intensity.

2. Bar Graph: Average Coffee Consumption – Exam Week vs. Normal Week
This bar graph compares the average number of coffees consumed during exam weeks versus normal (non-exam) weeks.
It provides a clear visual comparison to test the hypothesis that coffee consumption increases during exam periods.
If the bar representing exam weeks is significantly higher, it suggests that academic stress during exams leads to higher caffeine intake.

3. Boxplot: Coffee Consumption by Course Load Category
This boxplot illustrates the distribution of coffee consumption across different course load categories (Low, Medium, High).
It helps to understand whether days with heavier workloads are associated with higher coffee consumption.
The spread and median values allow us to visually assess if students tend to consume more caffeine as their academic demands increase.

4. Correlation Matrix Heatmap
The correlation matrix heatmap shows the relationships between key numeric variables:
Coffee Number
Caffeine Amount (mg)
Course Load (min)
Exam Number (that week)
Strong positive or negative correlations can be identified through color intensity.
For example, a positive correlation between course load and coffee number would indicate that as the workload increases, coffee consumption tends to rise.

5. Line Plot: Weekly Average Coffee Consumption
This line plot displays the average number of coffees consumed each week.
By aggregating the data weekly, we can observe broader patterns and seasonal trends across the semester.
Peaks in the graph could correspond to exam periods or weeks with particularly high academic workload.
