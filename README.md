# **Optimizing Public Safety and Traffic Management Through US Accident Data (2016-2023)**

## **Overview**  
Traffic accidents in the U.S. contribute to significant **fatalities, injuries, economic losses, and congestion-related delays**. Understanding the **causes, patterns, and risk factors** behind accident severity is crucial for **improving public safety, optimizing emergency responses, and enhancing traffic management systems**. 

This project analyzes **7.7 million accident records (2016-2023)** to identify trends and influencing factors in accident severity. By leveraging **machine learning models**, the study aims to predict accident severity levels based on **weather conditions, road infrastructure, and temporal patterns**. The findings provide **actionable insights for policymakers, traffic engineers, and law enforcement agencies** to implement **effective safety interventions, reduce accident severity, and develop smarter traffic control strategies**.

<p align="center">
  <img src="https://github.com/dhruvyellanki19/project_images/blob/8af7f7ee281f80a72dbd6e0934eb5a46212fd51e/Accident_analysis_image.png" width="500"/>
</p>


## **Problem Statement**
Traffic accidents result in **injuries, fatalities, economic losses, and transportation disruptions**. Understanding the factors influencing accident severity is essential for **data-driven traffic management and road safety improvements**. This project aims to:
- Analyze accident severity trends across the US using **historical accident data (2016-2023).**
- Identify **high-risk locations** and **critical factors** influencing accident severity.
- Develop **machine learning models** to predict accident severity, enabling preventive measures.
- Assist in designing **intelligent traffic systems** that reduce the impact of severe accidents.
- Provide **data-driven insights for policymakers** to enhance roadway safety.

## **Motivation**
With **7.7 million recorded accidents across 49 states**, understanding accident patterns can help improve public safety and optimize traffic management. This study aims to:
- Identify locations, weather conditions, and timeframes leading to severe accidents.
- Predict accident severity using advanced ML models for better risk management.
- Assist **traffic agencies, city planners, and policymakers** in taking proactive steps to reduce accidents.
- Enhance **real-time decision-making** for emergency response teams.
- Develop **preventive strategies** to mitigate accident severity in high-risk areas.

## **Dataset & Features**
- **Source**: US Accident Data (2016-2023)
- **Size**: 7.7 million records
- **Coverage**: 49 states, with a focus on major highways like **I-95, US-1, and State Hwy 42**
- **Key Features**:
  - **Weather conditions** (temperature, humidity, wind speed, precipitation)
  - **Time-based attributes** (hour of day, weekday, peak hours, seasonal variations)
  - **Road conditions** (visibility, number of lanes, traffic signals, speed limits, road surface type)
  - **Accident severity levels** (1 to 4, representing minor to fatal accidents)
  - **Traffic density and congestion levels**

## **Methodology**
### **1. Data Preprocessing**
- **Handled missing values** via imputation strategies.
- **Feature engineering** for weather impact, traffic patterns, and accident hotspots.
- **Standardization and encoding** of categorical variables.
- **Implemented geospatial data integration** to account for accident hotspots.
- **Analyzed seasonal and temporal trends** to detect recurring accident patterns.

### **2. Exploratory Data Analysis (EDA)**
- **Accident frequency trends** across years, months, and hours.
- **Impact of weather conditions on severity.**
- **Geospatial analysis** to map high-risk accident locations.
- **Comparative study of urban vs. rural accident trends.**
- **Analysis of accident severity by highway type and congestion level.**

### **3. Machine Learning Models**
We implemented and evaluated multiple ML models:

| Model                  | Accuracy | ROC-AUC |
|------------------------|----------|---------|
| **Random Forest**      | **91.45%** | **0.81** |
| **Gradient Boosting**  | 90.67%  | 0.73 |
| **Logistic Regression** | 90.65%  | 0.67 |

- **Best Model**: Random Forest (**91.45% accuracy**, **0.81 ROC-AUC**)
- **Key Features Identified**:
  - **Temperature & Humidity** strongly influence accident severity.
  - **Peak hours (4-7 PM)** contribute to higher accident counts.
  - **Road type and visibility** affect severity levels.
  - **Traffic congestion levels** play a significant role in determining accident outcomes.
  - **Seasonal weather conditions** have a noticeable impact on accident trends.

## **Conclusion**
From this project, we can conclude that machine learning models can effectively predict accident severity based on environmental and temporal factors such as temperature, humidity, wind speed, and time of day. Random Forest emerged as the most reliable model with an accuracy of 90.95% and a ROC-AUC score of 0.79, demonstrating its ability to handle imbalanced data and capture complex patterns. Gradient Boosting and Logistic Regression performed moderately, but their limitations in handling minority classes and non-linear relationships highlighted the advantages of Random Forest.

Feature importance analysis showed that factors like temperature and humidity significantly influence accident severity, while conditions like rain and snow had minimal impact. These findings emphasize the importance of environmental and temporal variables in understanding accident dynamics. By identifying high-risk conditions and time periods, this project provides actionable insights for implementing targeted safety interventions, improving road safety, and potentially reducing the severity of accidents.

This project demonstrated the potential of machine learning to provide actionable insights. By identifying high-risk scenarios, such as certain weather conditions or peak traffic times, we can guide targeted interventions like deploying traffic management measures, optimizing traffic signal timing, increasing law enforcement presence, or issuing real-time safety alerts.

Additionally, preventive strategies such as improving roadway infrastructure, installing adaptive traffic control systems, integrating predictive analytics into transportation planning, and incorporating AI-powered early warning systems can significantly help in mitigating accident severity. Enhancing emergency response efficiency by allocating resources based on predicted accident hotspots will further improve public safety.

These findings reinforce the role of data-driven approaches in improving road safety, reducing accident severity, and enabling smarter, more adaptive traffic management systems.
The machine learning model successfully predicts accident severity based on weather, time, road conditions, and traffic data. While Random Forest performed the best, improvements in handling class imbalance and integrating real-time data sources can further enhance prediction accuracy. These findings can be leveraged by policymakers and traffic authorities to make data-driven decisions for safer roadways.

By identifying high-risk scenarios, such as specific weather conditions, time periods, and congestion levels, authorities can implement targeted traffic management interventions and deploy early warning systems to minimize accident severity. This project reinforces the potential of AI-driven predictive models in traffic safety and intelligent transportation systems.



## **Future Enhancements**
- **Develop AI-powered early warning systems for high-risk areas.**
- **Integrate deep learning models for real-time accident detection using traffic camera feeds.**
- **Enhance geospatial accident mapping with real-time GPS tracking.**
- **Implement SMOTE or other techniques to handle class imbalance more effectively.**
- **Develop interactive dashboards for real-time accident monitoring and risk prediction.**
