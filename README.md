# ADS506 Project  
**Team 2, ADS 506**  

## Metro Interstate Traffic Volume Forecasting  

### The Dataset  
The dataset used in this project is the "Metro Interstate Traffic Volume" dataset from the UC Irvine Machine Learning Repository. It contains 48,204 observations and 8 columns, covering the period from **2012 to 2018**.  

- **Source**: [Metro Interstate Traffic Volume Dataset](https://archive.ics.uci.edu/dataset/492/metro+interstate+traffic+volume)
- **Features**:
  - **Date/Time**: Hourly timestamp for traffic volume counts.
  - **Traffic Volume**: Count of vehicles passing a section of Interstate 94.
  - **Weather Attributes**: Includes temperature, precipitation, cloud cover.
  - **Holiday Indicators**: Binary flag for holidays.
  - **Seasonal/Temporal Data**: Hour, day, and month of observation.

---

### Objective  
This project aims to:
1. Perform exploratory data analysis (EDA) to study trends in traffic volume.
2. Analyze the impact of weather and temporal factors on traffic.
3. Develop advanced time series models for accurate traffic forecasting.

---

### Project Details  

#### **Motivation**  
Urban mobility challenges demand accurate traffic prediction systems to:
- Reduce commute stress and congestion.
- Enable efficient travel planning.
- Support urban planning decisions for sustainable city infrastructure.

#### **Libraries Used**  
The project leverages the following Python libraries:  
- **Data Analysis**: `pandas`, `numpy`, `seaborn`, `matplotlib`
- **Machine Learning**: `scikit-learn`, `statsmodels`
- **Deep Learning**: `keras`, `tensorflow`
- **Time Series**: `ARIMA`, `LSTM`

#### **Project Workflow**  
1. **Exploratory Data Analysis**:
   - Analyzed traffic patterns across hours, days, months, and weather conditions.
   - Key Insights:
     - Peak traffic occurs during morning (6-9 AM) and evening (4-6 PM) rush hours.
     - Traffic is lower during adverse weather and holidays.
     - Seasonal variations show higher traffic in spring/summer (May-October).
2. **Model Development**:
   - Baseline Models: Linear Regression, Gradient Boosting.
   - Time-Series Models: ARIMA, LSTM, and Hybrid ARIMA-LSTM.
   - Evaluation Metrics: MAE, RMSE, R².
3. **Visualization**:
   - Time series plots of actual vs. predicted traffic volumes.
   - Comparative analysis of model performance.

---

### Results  

| Model                  | MAE       | RMSE      | R²       |
|------------------------|-----------|-----------|----------|
| Linear Regression      | 384.18    | 493.01    | 0.945    |
| Gradient Boosting      | 245.79    | 313.80    | 0.978    |
| ARIMA                  | 319.97    | 380.02    | 0.967    |
| LSTM                   | 155.24    | 187.54    | 0.992    |
| Hybrid ARIMA-LSTM      | **123.86**| **153.26**| **0.995**|

---

### Conclusion  

This project demonstrates the use of machine learning and time-series analysis to forecast traffic volumes with high accuracy. The insights and models developed here can be extended to real-time traffic prediction systems, assisting commuters and city planners alike.

---

### Future Scope  

- Integration with real-time traffic APIs for dynamic forecasting.
- Extending the analysis with additional features such as construction updates.
- Exploring alternative hybrid modeling approaches.

---

### Project Contributors  
- Archana Suresh Patil 
- Jason Tong  
- Madeline Chang  

---


