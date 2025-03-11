# 🏪 Cafe Data Analytics Project


## 🎯 Project Overview
This project analyzes six months of cafe operations data to gain insights into sales trends, customer sentiment, and to build basic forecasting models.  The analysis was performed using Python and several key libraries. The project showcases data cleaning, exploratory data analysis (EDA), time series forecasting, and natural language processing (NLP) techniques.

## 📊 Features
* **Data Cleaning & Preprocessing:**  Handles missing values, standardizes data formats, and prepares data for analysis.
* **Sales Trend Analysis:** Explores monthly and daily sales patterns, identifies peak seasons and slow periods.
* **Product Category Analysis:**  Analyzes sales trends for individual product categories (e.g., pastries, hot drinks).
* **Time Series Forecasting:** Uses the Prophet library to forecast future sales for each product category.
* **Customer Sentiment Analysis:** Analyzes customer reviews to gauge overall sentiment and identify areas for improvement.
* **Aspect-Based Sentiment Analysis:**  Uses a BERT model to analyze customer reviews and identify sentiment towards specific aspects of the cafe experience (customer service, wait times, etc.).
* **Competitor Analysis:**  Compares customer sentiment and sales to competitor data.
* **Data Visualization:** Presents findings through various charts and graphs using Matplotlib and Seaborn.

## ⚙️ Usage
The project is implemented as Jupyter Notebooks. Each notebook focuses on a specific aspect of the analysis. To reproduce the analysis:

1. Install the necessary dependencies (see Installation section).
2. Obtain the `Workbook.xlsx` file containing the cafe data.  Place it in the same directory as the notebooks.
3. Run the Jupyter Notebooks sequentially:
    * `Initial_Exploration_Order_Data.ipynb`:  Performs initial data exploration and time series analysis.
    * `Intro_Review_Sentiment_Analysis.ipynb`: Performs NLP analysis on customer reviews.

## 📦 Installation
1. Create a conda environment: `conda create -n cafe_analysis python=3.9`
2. Activate the environment: `conda activate cafe_analysis`
3. Install dependencies: `pip install -r requirements.txt` (You'll need to create a `requirements.txt` file listing all the necessary packages, based on the import statements in the notebooks)

## 🛠️ Technologies Used
* **Python:** The primary programming language for data analysis and model building.
* **Pandas:** Used for data manipulation and cleaning.
* **NumPy:** Used for numerical operations and array handling.
* **Matplotlib & Seaborn:** Used for creating visualizations of data.
* **Prophet:** A time series forecasting library used to predict future sales.
* **spaCy:** Used for natural language processing tasks, including entity recognition and text processing.
* **Transformers:**  A library containing pre-trained language models, specifically used here for sentiment analysis via a BERT model.

## 🧮 Statistical Analysis
* **Descriptive Statistics:** Calculated means, frequencies, and distributions of review scores and sentiment scores.
* **Time Series Decomposition:**  Implicitly used by Prophet for forecasting.
* **Z-score Outlier Detection:** Used to remove outliers from the daily sales data.
* **Interquartile Range (IQR) Outlier Detection:** Used to remove outliers from the daily sales data before further analysis.
* **MAPE (Mean Absolute Percentage Error):** Used for evaluating the accuracy of time series forecasts.

## 📈 Visualization
The project makes extensive use of Matplotlib and Seaborn to generate various types of visualizations, including:

* Histograms of review scores and sentiments.
* Line charts of sales trends over time.
* Bar charts comparing sentiment percentages across different aspects.
* Heatmaps to show the frequency of certain entities or phrases.
* Word clouds to visualize frequent topics in customer reviews.

*README.md was made with [Etchr](https://etchr.dev)*