
# **Sales Data Forecasting**  

## **Overview**  
This project aims to forecast weekly sales quantities for different product categories and sales channels using time series forecasting techniques. The goal is to generate accurate sales predictions for the next three months (September, October, and November) to aid in business planning and decision-making.  

## **Dataset Description**  
The dataset contains historical sales data with the following key attributes:  

- **weekend_date**: The date marking the end of each week (weekly time index).  
- **channel**: Sales channel identifier.  
- **brand**: Product brand identifier.  
- **category & sub_category**: Product classification details.  
- **SerialNum**: Unique product identifier.  
- **quantity**: Weekly quantity sold (target variable for forecasting).  

## **Objective**  
- Develop a robust time series forecasting model.  
- Predict weekly sales for the upcoming three months (September, October, November).  
- Present a clear DataFrame containing week-ending dates and predicted quantities.  

## **Approach**  
1. **Data Preprocessing**  
   - Convert `weekend_date` to a DateTime format.  
   - Aggregate data at the weekly level.  
   - Handle missing values and outliers.  

2. **Exploratory Data Analysis (EDA)**  
   - Analyze sales trends, seasonality, and patterns.  
   - Visualize historical sales data.  

3. **Model Selection & Forecasting**  
   - Time series models considered:  
     - **ARIMA** (AutoRegressive Integrated Moving Average)  
     - **Exponential Smoothing (ETS)**  
     - **Facebook Prophet** (used in this project)  
   - Train the model on historical data.  
   - Forecast sales for the next 13 weeks.  

4. **Results**  
   - Output a table containing predicted sales for each week.  
   - Visualize the forecasted trends.  

## **Installation & Setup**  
To run the forecasting model, follow these steps:  

### **1. Clone the Repository**  
```bash
git clone https://github.com/vidhirana10/Sales_data_forecasting.git
cd Sales_data_forecasting
```

### **2. Install Dependencies**  
Ensure you have Python installed, then install the required libraries:  
```bash
pip install pandas numpy matplotlib prophet
```

### **3. Run the Forecasting Script**  
```bash
python sales_forecasting.py
```

## **Example Output**  
| weekend_date | predicted_quantity |
|-------------|--------------------|
| 2024-09-07  | 1234               |
| 2024-09-14  | 1302               |
| 2024-09-21  | 1198               |
| ...         | ...                |
| 2024-11-30  | 1456               |

## **Contributors**  
- **Vinayak Rana**  

## **License**  
This project is open-source and available under the [MIT License](LICENSE).  

---

