# **Optimizing Public Safety and Traffic Management Through US Accident Data (2016-2023)**  

## **Overview**  
Traffic accidents are a major concern in the U.S., leading to injuries, fatalities, congestion, and economic losses. Effective accident analysis and prediction can help mitigate risks, improve public safety, and enhance traffic management.  

This project leverages **7.7 million accident records (2016-2023)** to analyze patterns, trends, and risk factors influencing accident severity. Using machine learning models, we predict accident severity based on weather conditions, road features, and time-based factors. These insights can be used by policymakers, traffic authorities, and emergency response teams to prevent severe accidents and optimize traffic control strategies.  

---

## **Problem Statement**  
Highway accidents remain a critical public safety issue, affecting millions of people every year. Determining accident severity in advance can:  
- Reduce fatalities and injuries by identifying high-risk situations.  
- Optimize emergency response time by prioritizing severe accident-prone areas.  
- Improve traffic flow management by deploying proactive safety measures.  

However, traditional accident prediction methods fail to account for dynamic factors like weather conditions, congestion levels, and road design features. This project addresses these gaps by building a data-driven machine learning model that accurately predicts accident severity and helps decision-makers implement safety interventions.  


---

## **Motivation**  
With over **7.7 million recorded accidents** across **49 states**, understanding patterns, trends, and risk factors is essential for data-driven decision-making in traffic safety. This study aims to:  
- Identify high-risk locations and conditions leading to severe accidents.  
- Predict accident severity based on weather, road conditions, and time-based factors.  
- Provide actionable insights for reducing accident risks and improving emergency response.  
- Assist transportation authorities in traffic control planning and infrastructure improvements.  

---

## **Objectives**  
1. Analyze accident trends to determine the key factors influencing severity.  
2. Develop predictive models for accident severity classification.  
3. Identify high-risk zones and timeframes for targeted interventions.  
4. Provide actionable insights for transportation authorities and policymakers.  
5. Support emergency response teams in prioritizing accident-prone areas.  

---

## **Dataset & Features**  
### **Dataset Overview**  
- Source: U.S. Accident Data (2016-2023)  
- Size: 7.7 million accident reports  
- Coverage: 49 states (focus on I-95, US-1, and other highways)  

### **Key Features**  
- Weather conditions – Temperature, humidity, wind speed, precipitation  
- Time-based attributes – Day/night, rush hours, weekday/weekend trends  
- Road conditions – Visibility, number of lanes, speed limits, traffic signals  
- Accident severity levels – Minor, moderate, and severe (target variable)  

---

## **Data Processing Steps**  
To improve model accuracy, the dataset underwent extensive preprocessing:  
- Data Cleaning – Handled missing values, duplicate entries, and inconsistencies.  
- Outlier Removal – Eliminated extreme cases to reduce bias in severity prediction.  
- Feature Engineering – Created new attributes from existing data (e.g., temperature impact, peak traffic hours).  
- Normalization & Encoding – Scaled numerical variables and converted categorical features for model training.  

---

## **Methodology**  
### **1. Exploratory Data Analysis (EDA)**  
EDA was conducted to identify trends and key insights:  
- Accident severity distribution across different conditions.  
- Impact of weather factors (rain, snow, fog) on accident severity.  
- High-risk accident locations & traffic congestion analysis.  

### **2. Feature Selection & Model Interpretability**  
- Correlation analysis to determine the most influential factors.  
- Feature importance ranking for predictive performance improvement.  

### **3. Machine Learning Models**  
We implemented and evaluated multiple models:  

| Model                  | Accuracy | ROC-AUC |
|------------------------|----------|---------|
| Random Forest         | 90.95%   | 0.79    |
| Gradient Boosting     | 89.67%   | 0.73    |
| Logistic Regression   | 88.65%   | 0.67    |

- Best Model: Random Forest, achieving 90.95% accuracy and 0.79 ROC-AUC.  
- Key Findings from Feature Importance Analysis:  
  - Temperature and humidity strongly influence accident severity.  
  - Night-time accidents are more severe compared to daytime accidents.  
  - High-speed highways report more severe accidents than urban roads.  

---

## **Key Findings**  
- Peak accident hours: Most accidents occur between **4-7 PM** due to high traffic density.  
- Weather impact: **Temperature and humidity are stronger predictors** of accident severity than rain or fog.  
- High-risk locations: **I-95 and US-1** report the most severe accidents.  
- Machine learning models effectively **predict accident severity**, enabling **preventive traffic management**.  

---

## **Challenges & Limitations**  
- Class imbalance: Severe accidents are less frequent, requiring oversampling techniques.  
- Data inconsistencies: Some records lacked critical weather details, leading to data imputation.  
- Geographic variations: Different states have different traffic laws, affecting severity trends.  

---



## **Future Enhancements**  
- Integration with real-time accident data for live risk assessment.  
- Development of an interactive visualization dashboard.  
- Advanced deep learning models for traffic image analysis.  
- Collaboration with smart traffic management systems.  

---

## **Conclusion**  
From this project, we can conclude that machine learning models can effectively predict accident severity based on environmental and temporal factors such as temperature, humidity, wind speed, and time of day. Random Forest emerged as the most reliable model with an accuracy of 90.95% and a ROC-AUC score of 0.79, demonstrating its ability to handle imbalanced data and capture complex patterns. Gradient Boosting and Logistic Regression performed moderately, but their limitations in handling minority classes and non-linear relationships highlighted the advantages of Random Forest.

Feature importance analysis showed that factors like temperature and humidity significantly influence accident severity, while conditions like rain and snow had minimal impact. These findings emphasize the importance of environmental and temporal variables in understanding accident dynamics. By identifying high-risk conditions and time periods, this project provides actionable insights for implementing targeted safety interventions, improving road safety, and potentially reducing the severity of accidents.

This project demonstrated the potential of machine learning to provide actionable insights. By identifying high-risk scenarios, such as certain weather conditions or peak traffic times, we can guide targeted interventions like deploying traffic management measures or issuing real-time safety alerts. These findings reinforce the role of data-driven approaches in improving road safety and reducing the severity of accidents.
