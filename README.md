# screentime_studyinghours
## **Project Goal**
In this DSA210 term project, I will analyze how my screen time impacts my education by influencing my studying hours. By using factors like total screen usage (both educational platforms and entertainment/social media platforms), academic stress levels, academic responsibilities, sleep duration, and time spent on social activities (including face-to-face interactions), I aim to track my daily screen time and examine its correlation with my studying hours. These factors can influence my screen time by increasing or decreasing it, which in turn may positively or negatively affect the time I plan to study.

---

## **Motivation**
Screen time plays a crucial role in education through its impact on studying habits. While digital tools and educational platforms can enhance learning, unstructured screen use—especially for entertainment and social media might negatively affect academic productivity. Understanding how my screen habits correlate with my studying hours can help me develop more effective time management strategies. I hope to:
- Identify patterns between screen usage and studying hours to determine whether increased screen time leads to reduced study efficiency or if structured digital engagement enhances learning.

- Analyze how external factors such as academic responsibilities, stress levels, sleep duration, and social interactions influence screen time, potentially affecting my study habits.

- Gain actionable insights into optimizing my screen habits to improve focus, productivity, and overall academic performance.

---

## **Data Collection & Analysis**
The dataset for this project consists of three months of daily records. 

#### **Data Sources**
- **Date**: The specific day, recorded manually in Google Sheets file in Drive. 
- **Screen time**: The screen time for both educational and non-educational platforms (hours), recorded from iOS Screen Time Data. 
- **Academic responsibilities**: Includes the number of homework assignments, exams, and projects, retrieved from academic calendar and recorded manually in Google Sheets file in Drive.
- **Sleep duration**: Total sleep duration (hours), recorded in Sleep Diary App.
- **Time spent on social activities**: Total time spent (hours), recorded manually in Google Sheets file in Drive.
- **Studying hours**: Total study hours (in hours), recorded in Toggle Track App.

I will track all data using Google Sheets and Applications that I mentioned to ensure accurate and consistent data collection. External factors such as illness, special circumstances, or unexpected routine changes will be noted and excluded from the analysis to maintain data reliability.

#### **Data Analysis** 

##### **1. Data Preprocessing**
The collected dataset undergoes preprocessing to ensure consistency and accuracy before analysis. This includes:

- Cleaning and structuring the data recorded in Google Sheets, iOS Screen Time, Toggl Track, and Sleep Diary App.

- Standardizing data formats across different sources for seamless integration.

##### **2. Exploratory Data Analysis (EDA)** 
- Analyzed distributions of screen time, studying hours, sleep duration, academic stress levels, and social activity time over the recorded period.

- Identified trends in how screen time fluctuates with external factors such as academic responsibilities, sleep patterns, and social interactions.

- Compared educational vs. entertainment screen time usage and its potential impact on studying hours.

##### **3. Correlation Analysis**
- Examined the relationship between total screen time and studying hours to determine if higher screen time negatively or positively correlates with study efficiency.

- Investigated how external factors (academic stress, responsibilities, sleep duration, and social activities) influence screen time, potentially affecting study productivity.
- Analyzed if specific types of screen usage (educational vs. non-educational) correlate differently with studying hours.

##### **4. Visualization**
- Used graphs, histograms, scatter plots, bar charts, and heatmaps to represent trends and correlations.

- Created comparative charts to analyze the impact of various external factors on screen time and studying hours.

---

## **Report**
This study aims to understand how daily screen time habits influence studying hours, considering external factors such as academic stress, academic load, sleep duration, and time spent on social activities. Recognizing patterns in personal habits will enable better planning and improved academic efficiency.

### **Hypothesis**
- Null Hypothesis(H0): There is no significant correlation between total screen time and studying hours.
- Alternative Hypothesis(H1): There is a significant negative correlation between total screen time and studying hours.
  
### **Machine Learning Models**
To further explore how various behavioral and contextual variables affect studying hours, we implemented supervised machine learning models.
Regression Models with Hyperparameter Tuning:
- Random Forest Regressor

- Decision Tree Regressor

- K-Nearest Neighbors Regressor

Each model was evaluated using; R² Score – to measure explanatory power, Mean Squared Error (MSE) – to evaluate prediction accuracy, Visual analysis of actual vs. predicted studying hours.

### **Results of the Analysis**
##### **Univariate Analysis** 
- Studying Hours: A histogram of studying hours revealed a moderately right-skewed distribution. This suggests that while most days involved a typical amount of study, a few days showed exceptionally high dedication—likely during periods of intense academic responsibility.
  
- Screen Time: Screen time showed a broad distribution, with peaks around average daily screen exposure. Non-educational usage dominated the total screen time, particularly on weekends and low-stress days.
  
- Sleep Duration: Most values ranged between 5.5 and 8 hours. Days with longer sleep tended to align with increased studying hours, indicating a positive association between rest and academic productivity.
  
- Academic Responsibility: Days with a high number of academic tasks (homeworks or exams) generally correlated with reduced non-educational screen time and increased study commitment.
  
- Social Activity Time: Spikes in social time were common on weekends, and these days typically had lower study duration, confirming an inverse relationship.

##### **Bivariate Analysis** 
- Screen Time vs. Studying Hours: Scatter plots demonstrated a negative correlation between total screen time and study duration. As screen time increased, studying hours decreased significantly—especially when screen time was non-educational.
  
- Sleep vs. Studying Hours: A positive trend was observed: individuals who slept more (7–8+ hours) studied longer and more consistently compared to sleep-deprived days.
  
- Academic Responsibility vs. Screen Time: Bar charts revealed that as academic tasks increased, users naturally self-regulated by reducing screen exposure—especially from entertainment platforms.

##### **Multivariate Analysis** 
- Correlation Heatmap:
The strongest negative correlation was between screen time and studying hours, while sleep duration showed a weak positive correlation.
Notable correlations:
Screen Time vs. Studying Hours: −0.65
Academic Responsibilities vs. Studying Hours: +0.58
Sleep Duration vs. Studying Hours: +0.30

- Combined Influences:
Days with both high academic responsibility and sufficient sleep tended to result in significantly higher studying hours, even when screen time was above average—suggesting possible compensatory focus.

##### **Machine Learning Results** 
The performance of the three models is summarized below:
  |**Model**                |**Mean Squared Error(MSE)**   	 |**R^2**      |
  |-------------------------|--------------------------------|-------------|
  |Random Forest            | 0.36 				                   | 0.67        |
  |Decision Tree	          | 0.41 				                   | 0.63        |
  |K-Nearest Neighbors      | 0.44 				                   | 0.58        |

Among the tested models, the Random Forest Regressor achieved the best overall performance, with the highest R^2 score and lowest MSE. This suggests that ensemble methods are more effective in capturing the nonlinear and complex relationships between daily habits and studying hours.

### **Findings**
- Screen time (especially non-educational) showed a strong negative correlation with studying hours.
 
- High academic responsibility days led to increased studying hours and reduced unproductive screen time.

- Sleep duration had a positive effect on studying hours — better-rested days resulted in more focused study sessions.

- Social activity time, particularly on weekends, showed a moderate negative impact on studying time.

### **Limitations**
- The dataset is limited to one individual's daily observations over a 3-month period.
- Self-reported values such as social interaction hours may introduce subjective bias.
- The analysis does not include qualitative screen use details (e.g., content type).

### **Conclusion**
This project highlights the strong relationship between screen time habits and academic productivity. Unstructured screen use—especially for entertainment—reduces studying efficiency, while structured usage (such as educational platforms) may offer mild positive support.

The machine learning models confirmed these patterns, with Random Forest showing the highest predictive performance. Overall, the study emphasizes the importance of mindful screen usage and offers a data-driven approach to managing digital behavior for academic improvement.























