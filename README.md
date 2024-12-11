# SolarRadiation 
# KIAM 3 week 0 assessment 
# Exploratory Data Analysis (EDA) on Weather Dataset

This project involves performing an in-depth **Exploratory Data Analysis (EDA)** on a weather dataset, focusing on various aspects such as statistical analysis, data quality checks, time series trends, correlation analysis, wind and temperature analyses, and data cleaning. The goal is to uncover patterns and relationships within the data and prepare it for further analysis or modeling.

## Key Steps in the Analysis

### 1. **Summary Statistics**
- Calculated essential statistical measures for each numeric column, including:
  - **Mean**
  - **Median**
  - **Standard Deviation**
  - Other statistical measures to understand the distribution of the data.

### 2. **Data Quality Check**
- Inspected the dataset for missing values, incorrect entries (e.g., negative values where only positives should exist), and outliers, especially in columns like **GHI (Global Horizontal Irradiance)**, **DNI (Direct Normal Irradiance)**, and **DHI (Diffuse Horizontal Irradiance)**.
- Checked for anomalies and outliers in **sensor readings (ModA, ModB)** and **wind speed data (WS, WSgust)**.

### 3. **Time Series Analysis**
- Plotted bar charts and line charts for **GHI**, **DNI**, **DHI**, and **Tamb (Ambient Temperature)** to observe:
  - Monthly patterns
  - Daily trends
  - Anomalies, such as peaks in solar irradiance or temperature fluctuations.
- Evaluated the impact of the **'Cleaning'** column on sensor readings (**ModA**, **ModB**) over time.

### 4. **Correlation Analysis**
- Used **correlation matrices** and **pair plots** to visualize the relationships between:
  - Solar radiation components (**GHI**, **DNI**, **DHI**) and temperature measures (**TModA**, **TModB**).
- Investigated the correlation between **wind conditions (WS, WSgust, WD)** and **solar irradiance** using **scatter matrices**.

### 5. **Wind Analysis**
- Created **radial bar plots** or **wind roses** to analyze wind trends and identify significant wind events, including:
  - Distribution of **wind speed (WS)**
  - **Wind direction (WD)**
  - Variability of wind direction over time.

### 6. **Temperature Analysis**
- Examined how **Relative Humidity (RH)** might influence temperature readings and solar radiation, identifying any significant patterns or correlations.

### 7. **Histograms**
- Generated histograms for key variables like **GHI**, **DNI**, **DHI**, **WS**, and **temperatures** to visualize the frequency distribution and understand data spread.

### 8. **Z-Score Analysis**
- Calculated **Z-scores** to flag data points that significantly deviate from the mean, helping identify outliers or anomalous data points.

### 9. **Bubble Charts**
- Created **bubble charts** to explore complex relationships between variables, such as:
  - **GHI** vs **Tamb** vs **WS**, with bubble size representing an additional variable like **RH** or **Barometric Pressure (BP)**.

### 10. **Data Cleaning**
- Performed data cleaning based on initial findings, addressing:
  - Missing values
  - Anomalies in columns like **Comments** (which were found to be entirely null).
  - Correcting issues such as negative values in columns where only positive values should exist.

## Tools and Libraries Used
- **Python**
- **Pandas**: For data manipulation and cleaning.
- **Matplotlib & Seaborn**: For visualization (histograms, scatter plots, correlation matrices, etc.).
- **Numpy**: For statistical calculations (mean, median, standard deviation, Z-scores).
- **Scikit-learn**: For calculating Z-scores and performing additional data analyses.

## Conclusion
This EDA provides a comprehensive overview of the weather dataset, uncovering key patterns, trends, and relationships among solar radiation, wind, temperature, and other environmental factors. The insights gained will serve as a foundation for further analysis, modeling, and decision-making.


