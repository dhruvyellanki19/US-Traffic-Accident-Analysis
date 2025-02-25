# **Optimizing Public Safety and Traffic Management Through US Accident Data (2016-2023)**

## **Data Source**: 
https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents/data


## **Overview**  
Traffic accidents in the U.S. contribute to significant fatalities, injuries, economic losses, and congestion-related delays. Understanding the causes, patterns, and risk factors behind accident severity is crucial for improving public safety, optimizing emergency responses, and enhancing traffic management systems. 

This project analyzes 7.7 million accident records (2016-2023) to identify trends and influencing factors in accident severity. By leveraging machine learning models, the study aims to predict accident severity levels based on weather conditions, road infrastructure, and temporal patterns. The findings provide actionable insights for policymakers, traffic engineers, and law enforcement agencies to implement effective safety interventions, reduce accident severity, and develop smarter traffic control strategies.

<p align="center">
  <img src="https://github.com/dhruvyellanki19/project_images/blob/8af7f7ee281f80a72dbd6e0934eb5a46212fd51e/Accident_analysis_image.png" width="500"/>
</p>

### **Problem Statement**  

Traffic accidents on highways such as US-1, I-95, and State Hwy 42 pose serious risks to public safety, leading to severe injuries, fatalities, congestion, economic losses, and environmental impacts. Accidents disrupt mobility, increase emergency response times, and result in significant financial burdens due to medical expenses, vehicle damage, and shipment delays. Additionally, prolonged traffic congestion caused by accidents leads to increased fuel consumption and emissions.  

Despite advancements in traffic management, predicting accident severity remains a challenge** due to the complex interplay of factors such as weather conditions, road infrastructure, traffic density, and temporal variations. Existing systems primarily focus on reactive measures rather than predictive analytics, limiting the ability of authorities to take proactive steps to mitigate accident severity.  

This project aims to develop a machine learning-based accident severity prediction model using 7.7 million accident records (2016-2023) By analyzing key influencing factors—such as temperature, humidity, wind speed, visibility, time of day, and road conditions**—this model will help predict accident severity levels in real-time. The insights generated from this analysis will enable traffic authorities, emergency responders, and policymakers to implement preventive measures, optimize resource allocation, and enhance traffic management strategies ultimately reducing accident severity and improving road safety.


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

- **Handling Missing Values**: Missing data is imputed using appropriate statistical techniques to maintain dataset integrity.  
- **Feature Engineering**: Additional features related to **weather conditions, traffic patterns, and accident hotspots** are created to enhance predictive power.  
- **Standardization and Encoding**: Categorical variables such as **wind direction and weather conditions** are standardized and encoded for better model compatibility.  
- **Geospatial Data Integration**: Accident locations are mapped to identify high-risk zones and incorporate spatial context into the analysis.  
- **Seasonal and Temporal Analysis**: Patterns related to accident frequency across different **times of the day, days of the week, and seasonal variations** are examined to detect recurring trends.  
- **Outlier Detection and Handling**: Extreme values in numerical columns, such as accident duration and distance, are addressed to improve model performance and prevent skewed predictions.  

### **Exploratory Data Analysis (EDA)**  

Performed Exploratory Data Analysis to analyze accident severity trends across temporal, weather, and geographic dimensions to uncover key influencing factors. The analysis included:  
- **Accident Frequency Trends**: Examined accident occurrences over different years, months, and hours of the day to detect high-risk time periods.  
- **Impact of Weather Conditions**: Investigated how factors like temperature, humidity, wind speed, and visibility correlate with accident severity.  
- **Geospatial Analysis**: Mapped accident hotspots at state and city levels to identify high-risk locations using clustering techniques.  
- **Urban vs. Rural Comparisons**: Analyzed accident frequency and severity variations in urban vs. rural settings to highlight differences in road conditions and congestion levels.  
- **Severity Analysis by Highway Type**: Assessed accident severity trends based on different highway types (e.g., I-95, US-1, and State Hwy 42) and their respective traffic congestion levels.  
- **Outlier Detection**: Identified anomalies in accident duration and travel distance using boxplots and clustering methods to refine the dataset.  
- **Feature Correlation Analysis**: Created correlation heatmaps to identify relationships between numerical variables affecting accident severity.  
- **Visualization Techniques**: Used histograms, scatter plots, boxplots, and violin plots to summarize and visualize accident characteristics across multiple dimensions.  

## **3. Model Development & Evaluation**

### Hypothesis  
We hypothesize that environmental factors (e.g., temperature, humidity, wind speed, and visibility),temporal factors (e.g., time of day, day of the week), and *location-specific characteristics significantly impact accident severity. By analyzing these factors, we aim to build a predictive model that identifies high-risk conditions and time periods for targeted interventions.  

### Target Variable  
The target variable for this study is Severity, categorized as follows:  
1 - Minor severity (minimal impact).  
2 - Moderate severity (some disruptions and injuries).  
3 - Severe accidents (significant injuries and delays).  
4 - Very severe accidents (critical injuries or fatalities).  

The objective is to predict the severity of an accident based on environmental, temporal, and geographical features.  

### Approach  
The model was developed using a structured machine learning pipeline, including data cleaning, feature selection, and predictive modeling. Various machine learning algorithms were implemented and evaluated to identify the most effective model.  

- **Feature Preprocessing**: Numerical features were scaled, and categorical features were encoded for consistency.  
- **Multicollinearity Handling**: Variance Inflation Factors (VIF) were calculated to remove highly correlated features.  
- **Model Selection**: Logistic Regression, Random Forest, and Gradient Boosting were tested to determine the best-performing model.  
- **Performance Evaluation**: Accuracy and ROC-AUC scores were used to assess model reliability.  

### Model Performance  

| Model                  | Accuracy | ROC-AUC |
|------------------------|----------|---------|
| Random Forest         | 91.45%   | 0.81    |
| Gradient Boosting     | 90.67%   | 0.73    |
| Logistic Regression   | 90.65%   | 0.67    |

**Best Model**: The **Random Forest model** achieved the highest accuracy of **91.45%** and an **ROC-AUC score of 0.81**, making it the most effective classifier in distinguishing accident severity levels.  

### Feature Importance  
The most influential features affecting accident severity were:  
1. **Temperature** - 29.6%  
2. **Humidity** - 25.3%  
3. **Hour of the Day** - 15.4%  
4. **Wind Speed** - 14.6%  
5. **Weekday** - 8.1%  

### Key Findings  
- The model accurately predicts **low and mid-severity accidents**, offering reliable insights for these categories.  
- Predictions for **high-severity accidents** showed greater variation, suggesting additional influencing factors not accounted for in the dataset.  
- Residual distribution analysis indicated that **most predictions had minimal error**, but some cases exhibited significant deviations.  
- **Scatter plots** comparing actual and predicted severity levels revealed higher variance in severe accidents, highlighting the need for additional data points to improve model robustness.  

By implementing machine learning models and evaluating their effectiveness, we successfully developed a **predictive framework for accident severity classification**. The next steps involve refining the model by incorporating additional data sources and optimizing hyperparameters for improved accuracy.


## **Conclusion**

This project demonstrates that machine learning models can effectively predict accident severity based on environmental and temporal factors, such as temperature, humidity, wind speed, and time of day. Among the models tested, Random Forest emerged as the most reliable, achieving an accuracy of 91.45% and a ROC-AUC score of 0.81, demonstrating its ability to handle complex patterns in accident data. Gradient Boosting and Logistic Regression also performed well, but both faced challenges in handling class imbalances and non-linear relationships, further highlighting the advantages of Random Forest.

Feature importance analysis revealed that temperature and humidity significantly influence accident severity, followed by wind speed and time of day. Weather conditions like rain and snow had low but non-negligible impact. These findings emphasize the critical role of environmental and temporal variables in understanding accident dynamics. By identifying high-risk conditions and time periods, this project provides actionable insights that can enhance traffic safety measures, improve emergency response times, and reduce accident severity.

Machine learning offers a data-driven approach to road safety, enabling authorities to implement targeted interventions such as:
- Deploying traffic management measures in high-risk areas.
- Optimizing traffic signal timing to reduce congestion-related accidents.
- Increasing law enforcement presence in accident-prone locations.
- Issuing real-time safety alerts based on weather and traffic conditions.

Beyond predictive modeling, this study highlights the potential of preventive strategies like improving roadway infrastructure, installing adaptive traffic control systems, and integrating predictive analytics into transportation planning. Enhancing emergency response efficiency by allocating resources based on predicted accident hotspots can further reduce fatalities and improve public safety.

While Random Forest delivered the best performance, future improvements—such as better handling of class imbalances and integrating real-time traffic and weather data—can further enhance the model’s accuracy and reliability. By identifying high-risk scenarios—such as specific weather conditions, time periods, and congestion levels—authorities can proactively deploy targeted traffic management interventions to minimize accident severity. This project serves as a foundation for leveraging machine learning and data analytics to make data-driven decisions for safer roadways.

## **Future Enhancements**
- Develop AI-powered early warning systems for high-risk areas.
- Integrate deep learning models for real-time accident detection using traffic camera feeds.
- Enhance geospatial accident mapping with real-time GPS tracking.
- Implement SMOTE or other techniques to handle class imbalance more effectively.
- Develop interactive dashboards for real-time accident monitoring and risk prediction.


## **Technology Used**
-	Python – For data processing and model development.
-	Pandas & NumPy – For handling and transforming data.
-	Matplotlib & Seaborn – For visualization and insights.
-	Scikit-learn – For implementing machine learning models.
-	Jupyter Notebook – For interactive analysis and development.
-	Plotly – For creating interactive visualizations.
-	Dask – For handling large datasets.
-	Scipy – For statistical transformations.
-	Statsmodels – Used for statistical analysis.
-	KMeans (Scikit-Learn) – For clustering accident data.
-	Statsmodels (VIF Analysis) – For handling multicollinearity.
-	Scikit-learn – For model implementation.
