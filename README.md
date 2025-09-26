<h1 align="center">Indonesia's Red Chili Pepper Retail Price Forecasting with MIMO LSTM Model Optimized with TPE</h1>

<p align="center">
  <a href="https://www.python.org" target="_blank"> <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"></a>
  <a href="https://pandas.pydata.org/" target="_blank"> <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"></a>
  <a href="https://numpy.org/" target="_blank"> <img src="https://img.shields.io/badge/Numpy-013243?style=for-the-badge&logo=numpy&logoColor=white"></a>
  <a href="https://matplotlib.org/" target="_blank"> <img src="https://img.shields.io/badge/Matplotlib-000000?style=for-the-badge&logo=matplotlib&logoColor=white"></a>
  <a href="https://seaborn.pydata.org/" target="_blank"> <img src="https://img.shields.io/badge/Seaborn-80b6ff?style=for-the-badge&logo=seaborn&logoColor=white"></a>
  <a href="https://scikit-learn.org/" target="_blank"> <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white"></a>
  <a href="https://www.tensorflow.org/" target="_blank"> <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white"></a>
  <a href="https://optuna.org/" target="_blank"> <img src="https://img.shields.io/badge/Optuna-00468B?style=for-the-badge&logo=optuna&logoColor=white"></a>
  <a href="https://joblib.readthedocs.io/en/latest/" target="_blank"> <img src="https://img.shields.io/badge/Joblib-00468B?style=for-the-badge&logo=joblib&logoColor=white"></a>
</p>

---

## 📌 Project Overview
Red chili pepper (*Cabai Rawit Merah*) is one of the most essential spices in Indonesian cuisine. Known for its fiery taste, it is widely used in various traditional dishes and is almost inseparable from Indonesian dining culture. Its presence is especially significant during special celebrations, communal gatherings, and in countless street food vendors, making it a staple ingredient that strongly represents Indonesian food identity.

With such high demand, red chili pepper has become more than just a cooking ingredient, it is now considered a strategic commodity in Indonesia. Price fluctuations of this commodity can directly impact household spending and food vendors. Therefore, analyzing its retail price over time is crucial to better understand supply-demand dynamics and potential market volatility.

This analysis covers multiple regions across Indonesia, with provinces selected to represent major islands of the archipelago. Specifically, Bali represents the island of Bali, Gorontalo for Sulawesi, Central Java for Java, South Kalimantan for Kalimantan, Papua for Papua, and North Sumatra for Sumatra. By including provinces from different islands, this study aims to capture a comprehensive and strategic overview of chili price behavior across the nation.

The ultimate expectation of this analysis is to provide valuable insights for multiple stakeholders. For farmers, it may serve as a reference to plan cultivation and harvest cycles. For consumers, it can help anticipate price fluctuations and manage household expenses. For the government, these findings can support policy-making and future strategies to stabilize food prices and ensure sustainable food security in Indonesia.

The Indonesian Retail Commodity Price Dataset used in this analysis was obtained from the [National Food Agency Price Panel](https://panelharga.badanpangan.go.id). The dataset covers the provinces of **Bali**, **Gorontalo**, **Central Java**, **South Kalimantan**, **Papua**, and **North Sumatra**. The data includes various commodities, but for this analysis, the focus will be on the commodity **Red Chili Pepper**, a natural ingredient commonly used in Indonesian cuisine.

This dataset is structured as a **time series** in **daily units**, spanning from **March 2021 to December 2023**. The dataset contains commodity price data recorded in **Indonesian Rupiah (IDR)** and expressed per **kilogram** (IDR/kg).

---

## ⚙️ Methodology

### 1. Exploratory Data Analysis (EDA)
- Identifying and analyzing missing values to understand data completeness and decide on proper handling strategies.
- Detecting duplicate records that may introduce bias and ensuring data integrity.
- Examining data distribution patterns and identifying potential outliers that may distort statistical analysis or modeling. *(Using boxplots)*
- Measuring skewness and kurtosis to evaluate whether the data approximates a normal distribution or shows deviations. *(Using histograms, skewness, and kurtosis calculations for each variable)*
- Visualizing time series data with line charts to observe trends, seasonality, and fluctuations over time.
- Assessing correlations among variables at the current time to uncover potential relationships relevant for MIMO modeling. *(Using Pearson correlation)*
- Analyzing autocorrelations across different lags to understand dependencies in time series data, which is critical for determining forecasting model window size/look-back period. *(Using ACF plots)*

### 2. Data Cleaning and Pre-processing
- Handling missing values and duplicate records.
- Splitting the dataset into **90% training**, **5% validation**, and **5% testing**.
- Applying **Min-Max normalization** to standardize the data range across all provinces and avoid bias during the training of the MIMO LSTM model.

### 3. Modeling & Evaluation
- Build a **Multi-Input Multi-Output (MIMO) LSTM** architecture tailored for multivariate time series forecasting.
- Optimize hyperparameters using **Tree-Structured Parzen Estimator (TPE)** to improve forecasting performance.
- Train the model on the processed dataset, using validation data to prevent overfitting.
- Evaluate the model using the **test set** with metrics such as **MAE (Mean Absolute Error)**, **MSE (Mean Squared Error)**, and **MAPE (Mean Absolute Percentage Error)**.
- Compare forecasting results across provinces to analyze regional differences in chili price dynamics.

---

## 📊 Results & Insights
- (Later)
- (Later)
- (Later)
- ...

---

## 💡Future Work
- (Later)
- (Later)
- (Later)
- ...
