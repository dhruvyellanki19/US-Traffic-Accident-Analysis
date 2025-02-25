# **US-Traffic-Accident-Analysis**  
**Optimizing Public Safety and Traffic Management Through US Accident Data (2016-2023)**  

## **Problem Statement**  
Highway accidents pose significant risks to public safety, leading to injuries, fatalities, traffic congestion, and economic losses. Identifying the key factors contributing to accident severity is crucial for **enhancing traffic management, improving road safety, and minimizing accident-related disruptions**.  

This project focuses on **analyzing and predicting accident severity** using **historical US traffic accident data from 2016-2023**, with a specific focus on major highways such as **US-1 and I-95**. By leveraging machine learning models, we aim to develop predictive tools that assist in **real-time traffic management and accident prevention**.  

---

## **Motivation**  
With over **7.7 million recorded accidents** across **49 states**, understanding **patterns, trends, and risk factors** is essential for **data-driven decision-making in traffic safety**. This study aims to:  
- Identify **high-risk locations and conditions** leading to severe accidents.  
- Predict **accident severity** based on **weather, road conditions, and time-based factors**.  
- Provide **actionable insights** for **reducing accident risks and improving emergency response**.  
- Assist transportation authorities in **traffic control planning and infrastructure improvements**.  

---

## **Objectives**  
1. **Analyze accident patterns** to determine major contributing factors.  
2. **Predict accident severity** using machine learning models.  
3. **Provide insights** for traffic management and policymaking.  
4. **Develop a data-driven approach** for improving public safety on highways.  
5. **Support emergency response teams** in prioritizing accident-prone areas.  

---

## **Dataset**  
- **Source**: US Accident Data (2016-2023)  
- **Size**: 7.7 million accident records  
- **Coverage**: 49 states, focusing on highways like **US-1, I-95, and State Hwy 42**  
- **Key Features**:  
  - **Weather conditions** (temperature, humidity, wind speed, precipitation)  
  - **Time-based attributes** (day/night, rush hours, weekday/weekend trends)  
  - **Road conditions** (visibility, number of lanes, speed limits, traffic signals)  
  - **Accident severity levels** (classified into minor, moderate, and severe)  

---

## **Methodology**  
### **1. Data Preprocessing**  
- **Handling missing values and outliers** through imputation techniques.  
- **Feature engineering** for weather, time, and geographical attributes.  
- **Data normalization and encoding** for machine learning model compatibility.  

### **2. Exploratory Data Analysis (EDA)**  
- **Analysis of accident frequency by state, highway, and weather conditions.**  
- **Correlation between accident severity and contributing factors.**  
- **Heatmaps to visualize accident-prone areas and high-risk locations.**  

### **3. Machine Learning Models**  
The following models were implemented and evaluated:  

| Model                  | Accuracy | ROC-AUC |
|------------------------|----------|---------|
| **Random Forest**      | **90.95%** | **0.79** |
| **Gradient Boosting**  | 89.67%  | 0.73 |
| **Logistic Regression** | 88.65%  | 0.67 |

- **Best Model**: **Random Forest**, achieving **90.95% accuracy** and **0.79 ROC-AUC**.  
- **Feature Importance Analysis**:  
  - **Temperature and humidity** were **strong predictors** of accident severity.  
  - **Night-time accidents** had higher severity compared to daytime accidents.  
  - **High-speed highways reported more severe accidents** than urban streets.  

---

## **Conclusion**  
From this project, we can conclude that machine learning models can effectively predict accident severity based on environmental and temporal factors such as temperature, humidity, wind speed, and time of day. Random Forest emerged as the most reliable model with an accuracy of 90.95% and a ROC-AUC score of 0.79, demonstrating its ability to handle imbalanced data and capture complex patterns. Gradient Boosting and Logistic Regression performed moderately, but their limitations in handling minority classes and non-linear relationships highlighted the advantages of Random Forest.

Feature importance analysis showed that factors like temperature and humidity significantly influence accident severity, while conditions like rain and snow had minimal impact. These findings emphasize the importance of environmental and temporal variables in understanding accident dynamics. By identifying high-risk conditions and time periods, this project provides actionable insights for implementing targeted safety interventions, improving road safety, and potentially reducing the severity of accidents.

This project demonstrated the potential of machine learning to provide actionable insights. By identifying high-risk scenarios, such as certain weather conditions or peak traffic times, we can guide targeted interventions like deploying traffic management measures or issuing real-time safety alerts. These findings reinforce the role of data-driven approaches in improving road safety and reducing the severity of accidents.

---


## **Key Findings**  
- **Peak accident hours**: Most accidents occur between **4-7 PM** due to high traffic density.  
- **Weather impact**: While **rain and fog contribute to accidents, temperature and humidity have a stronger impact on severity**.  
- **High-risk locations**: **I-95 and US-1** experience frequent and severe accidents due to heavy traffic.  
- **Machine learning models** can effectively **predict accident severity**, enabling **preventive traffic management**.  

---

## **Future Enhancements**  
- **Integration with real-time accident data for live risk assessment**.  
- **Development of an interactive visualization dashboard**.  
- **Advanced deep learning models for traffic image analysis**.  
- **Collaboration with smart traffic management systems**.  

---
