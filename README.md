# ADS506 Project

## Team 2, ADS 506

### Metro Interstate Traffic Volume Forecasting

---

## The Dataset
The dataset used in this project is the **"Metro Interstate Traffic Volume"** dataset from the [UC Irvine Machine Learning Repository](https://archive.ics.uci.edu/dataset/492/metro+interstate+traffic+volume). It contains **48,204 observations** and **8 columns** covering the period from **2012 to 2018**.

### Key Dataset Details:
- **Time Range Used for Modeling**: Data from **June 11, 2015** to **September 30, 2018**.
- **Features**:
  - `date_time`: Timestamp of each traffic count.
  - `traffic_volume`: Hourly vehicle counts.
  - `temp`: Hourly temperature in Fahrenheit.
  - `rain_1h`: Rain volume in the last hour.
  - `snow_1h`: Snow volume in the last hour.
  - `clouds_all`: Cloud coverage percentage.
  - `holiday`: Indicator of whether the day is a holiday.
  - `weather_main`: General weather condition (e.g., clear, fog, etc.).
  - `weather_description`: Detailed weather conditions (e.g., light rain, heavy snow, etc.).

---

## Objective
The primary objectives of this project are to:
1. **Perform Exploratory Data Analysis (EDA)**:
   - Study trends in traffic volume across time, weather conditions, and holidays.
   - Identify seasonal and temporal patterns in traffic.
2. **Complete Time Series Analysis**:
   - Build predictive models to forecast traffic volume.
   - Evaluate models using metrics like MAE, RMSE, and R².

---

## Data Information

### Purpose
To create an advanced traffic forecasting tool for commuters and urban planners by leveraging historical traffic data, meteorological conditions, and time-specific factors.

### Background
Urban congestion is a critical problem affecting productivity and quality of life. By accurately predicting traffic volumes, this project aims to:
- Help commuters plan their travel times effectively.
- Assist traffic authorities in developing long-term strategies for traffic management.

### Libraries Used
This project extensively uses the following Python libraries:
- **Data Processing**: `pandas`, `numpy`
- **Visualization**: `matplotlib`, `seaborn`
- **Machine Learning**: `scikit-learn`, `keras`, `statsmodels`
- **Time Series Analysis**: `statsmodels.tsa`, `ARIMA`, `LSTM`

---

## Notable Findings from EDA
- **Hourly Trends**:
  - Peak traffic during morning (6-9 AM) and evening (4-6 PM) rush hours.
  - Lowest traffic volume observed between 2-4 AM.
- **Day of the Week**:
  - Higher traffic volumes on weekdays, with peaks on Thursdays and Fridays.
  - Lower traffic volumes on weekends, especially Sundays.
- **Weather Effects**:
  - Adverse weather conditions (e.g., thunderstorms, squalls) correlate with lower traffic volumes.
  - Clear weather conditions result in higher traffic counts.
- **Holiday Impact**:
  - Significant drop in traffic on holidays like Christmas, Thanksgiving, and State Fair days.
  - Holidays like Independence Day and Memorial Day see relatively higher traffic due to recreational travel.
- **Seasonal Variations**:
  - Traffic volume peaks in spring and summer (May to October), with June as the highest month.
  - Winter months like January and December see the lowest volumes.

---
## Exploratory Data Analysis (EDA)

Key insights from the initial EDA include:
1. **Traffic Volume Trends**:
   - Peaks during morning (6-9 AM) and evening (4-6 PM) rush hours.
   - Lowest volumes observed between 2-4 AM.
2. **Day of the Week**:
   - Higher volumes on weekdays, particularly on Thursdays and Fridays.
   - Lower volumes on Sundays and holidays.
3. **Seasonal Trends**:
   - Traffic volume peaks during spring and summer (May to October), with a maximum in June.
   - Declines during winter months (December to February).
4. **Weather Impacts**:
   - Clear and cloudy conditions are associated with higher traffic.
   - Adverse weather, such as thunderstorms and snow, correlates with lower traffic.

## Modeling
### Models Implemented:
1. **Linear Regression**:
   - Baseline model for traffic forecasting.
2. **Gradient Boosting**:
   - Ensemble method for improved performance.
3. **ARIMA**:
   - Classical time-series forecasting technique.
4. **LSTM**:
   - Deep learning-based model for capturing temporal dependencies.
5. **Hybrid ARIMA-LSTM**:
   - Combines ARIMA's trend forecasting with LSTM's nonlinear feature capture for enhanced accuracy.

### Results Summary:
| Model                  | MAE       | RMSE      | R²       |
|------------------------|-----------|-----------|----------|
| Linear Regression      | 384.18    | 493.01    | 0.945    |
| Gradient Boosting      | 245.79    | 313.80    | 0.978    |
| ARIMA                  | 319.97    | 380.02    | 0.967    |
| LSTM                   | 155.24    | 187.54    | 0.992    |
| Hybrid ARIMA-LSTM      | **123.86**| **153.26**| **0.995** |

---

## Conclusion
The **Hybrid ARIMA-LSTM** model demonstrated the best performance, achieving the lowest error metrics and the highest R² score. This forecasting system can:
- Empower commuters to make better travel decisions.
- Support urban planners in designing data-driven strategies for efficient traffic management.

---

## Contributors

- **Archana Suresh Patil** 
- **Jason Tong**
- **Madeline Chang**
