🚦 Traffic Volume Forecasting with Facebook Prophet
This project utilizes time series forecasting to predict vehicle traffic volume using the Facebook Prophet library. The goal is to understand traffic trends and generate accurate short-term predictions based on historical hourly traffic data.

📄 Dataset Overview
The dataset contains:

DateTime: Timestamps (hourly)

Vehicles: Number of vehicles recorded

Additional fields like ID and Count (later dropped during preprocessing)

🔧 Key Processes
🔍 Data Preprocessing
Converted DateTime column to proper datetime format

Removed unused columns (ID, Count)

Renamed columns to ds (datetime) and y (target) for Prophet compatibility

📊 Exploratory Visualization
Time series line plot of vehicles vs. time to visually analyze patterns

✂️ Input Splitting
Splits the dataset into training and testing sets with the last 60 hours reserved for testing

🤖 Model Training with Facebook Prophet
Trains Prophet with yearly seasonality and seasonality prior scale adjustment

Generates future dataframes for hourly prediction

Plots the seasonal components (daily/weekly/yearly effects)

📈 Forecasting & Evaluation
Plots actual test values vs predicted traffic volume

Visualizes how well the model aligns with real traffic counts

📦 Libraries Used
pandas, numpy, matplotlib, seaborn

fbprophet (now known as prophet)

✅ Outcomes
Predictive traffic trends using historical patterns

Useful for applications in smart city planning, event traffic control, or infrastructure development

