# Food-Delivery-Time-Prediction-Using-ML

# Food Delivery Time Prediction Using ML

## Project Overview
In the fast-growing food delivery industry, accurately predicting delivery times is essential for improving **customer satisfaction** and **operational efficiency**. Companies like **Zomato** and **Swiggy** use machine learning algorithms to estimate delivery times, considering various factors such as traffic, weather conditions, and restaurant efficiency.

This project focuses on developing a **Machine Learning (ML) model** to predict food delivery times using **Python**. The dataset includes historical delivery records, and we apply different ML techniques like **Random Forest** and **LSTM** to determine the most effective model for prediction.

## Dataset Details
The dataset used in this project is sourced from **Kaggle** and contains various features related to food delivery orders. Below are the key dataset columns:

### **Features**
- **ID**: Unique identifier for each order.
- **Delivery_person_ID**: Unique ID assigned to each delivery partner.
- **Delivery_person_Age**: Age of the delivery person, which may impact delivery efficiency.
- **Delivery_person_Ratings**: Customer ratings given to the delivery partner, potentially indicating performance.
- **Restaurant_Latitude & Restaurant_Longitude**: Geographical location of the restaurant.
- **Delivery_Location_Latitude & Delivery_Location_Longitude**: Coordinates of the delivery location.
- **Type_of_order**: Category of food ordered (e.g., fast food, beverages, desserts).
- **Type_of_vehicle**: The vehicle used for delivery (e.g., bike, scooter, car).
- **Time_taken(min)**: **Target variable**—actual delivery time in minutes.

## Process Flow
### **1. Data Preprocessing**
- Load dataset and check for missing/null values.
- Handle missing data through imputation or removal.
- Normalize or scale numeric features where necessary.

### **2. Feature Engineering**
- Calculate **distance** between restaurant and delivery location using the **Haversine formula**.
- Convert categorical variables (e.g., vehicle type, food type) into numerical representations.

### **3. Exploratory Data Analysis (EDA)**
- Analyze relationships between key variables using **scatter plots, histograms, and correlation heatmaps**.
- Identify trends, such as the impact of distance, age, and ratings on delivery time.

### **4. Model Building Using ML**
- Split the dataset into **training (80%)** and **testing (20%)** sets.
- Train and compare multiple models:
  - **Random Forest**: A strong baseline model for regression.
  - **LSTM (Long Short-Term Memory)**: A deep learning approach to capture sequential patterns in data.
- Evaluate models using performance metrics such as **Mean Absolute Error (MAE)** and **R-squared**.

### **5. Model Evaluation & Performance Testing**
- Use test data to validate model predictions.
- Compare actual vs. predicted delivery times.
- Identify potential improvements such as adding traffic/weather data for better accuracy.

## Key Findings
- **Distance** is the most critical factor affecting delivery time.
- **Younger delivery partners** tend to complete deliveries faster.
- **Higher-rated delivery partners** show more efficient delivery times.
- **Food type and vehicle type** have minimal impact on delivery duration.

## Future Improvements
- **Incorporate real-time traffic data** to enhance accuracy.
- **Use ensemble models** to improve prediction stability.
- **Optimize feature selection** by integrating external factors like weather conditions.

## Conclusion
This project demonstrates how **machine learning** can be leveraged to optimize food delivery services by predicting delivery times accurately. The insights gained from the analysis help improve **logistics planning**, **resource allocation**, and **customer satisfaction**. Further refinements can make the model even more effective for real-world applications.

---

### **Contributors**
- **Project Team:** Monu Yadav(Independent)
- **Dataset:** Kaggle  
- **Technologies Used:** Python, Scikit-learn, Pandas, NumPy, Matplotlib, Seaborn  
- **ML Models:** Random Forest, XGBoost

