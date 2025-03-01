# 📌 Restaurant Data Analysis

## 📝 Project Overview
This project focuses on analyzing a dataset of restaurants, examining their distribution, ratings, and geospatial locations. The analysis is structured into two parts:

### **🔹 Part 1: Data Analysis**
- **Task 1**: Data Exploration & Preprocessing
- **Task 2**: Descriptive Analysis
- **Task 3**: Geospatial Analysis

### **🔹 Part 2: Advanced Insights**
- **Task 4**: Sentiment Analysis
- **Task 5**: Price vs Rating Correlation
- **Task 6**: Restaurant Rating Prediction

The dataset is stored in:
```
Dataset.csv
```

---

## 📂 Dataset Details
The dataset contains the following key columns:
- **Restaurant ID**: Unique identifier for each restaurant
- **Name**: Restaurant name
- **City**: The city where the restaurant is located
- **Country Code**: Country identifier
- **Cuisines**: Types of cuisine served
- **Aggregate Rating**: Overall restaurant rating
- **Latitude & Longitude**: Geospatial coordinates
- **Review Text** (for sentiment analysis)
- **Price Range** (for pricing insights)

---

## 🔍 Analysis Breakdown

### **🔹 Part 1: Data Analysis**

#### 🏷️ Task 1: Data Exploration & Preprocessing
📁 **File Location**: `Task1.ipynb`

- **Loading Data**: Reads `Dataset.csv` using Pandas.
- **Handling Missing Values**:
  - Identifies missing values in the "Cuisines" column.
  - Drops rows where "Cuisines" data is unavailable.
- **Statistical Overview**:
  - Uses `.head()`, `.info()`, `.describe()` for a summary.
  - Plots the distribution of "Aggregate Rating" using Matplotlib.

📷 **Visualization**:
- Histogram of Aggregate Ratings
  
![image](https://github.com/user-attachments/assets/051f1de3-6780-4bbf-b175-cadd36560216)



#### 📊 Task 2: Descriptive Analysis
📁 **File Location**: `Task2.ipynb`

- **Loading Preprocessed Data**: Reads cleaned data from `Dataset.csv`.
- **City & Country Analysis**:
  - Finds the most common restaurant locations.
  - Groups data by "City" and "Country Code".
- **Visualizing Trends**:
  - Bar plots of the top 10 countries and cities using Seaborn.

📷 **Visualizations**:
- Top 10 Countries by Restaurant Count

![image](https://github.com/user-attachments/assets/6b681317-241b-462f-8688-141b4de3c009)

- Top 10 Cities by Restaurant Count

![image](https://github.com/user-attachments/assets/b3049969-c49b-4c79-9b4b-0dcb765c1de7)

- Top 10 Cuisines

![image](https://github.com/user-attachments/assets/915152f4-1ddc-434a-8aa8-a4b72a60ed2b)


#### 🗺️ Task 3: Geospatial Analysis
📁 **File Location**: `Task3.ipynb`

- **Loading Data**: Reads `Dataset.csv`.
- **Mapping Restaurants**:
  - Extracts latitude and longitude data.
  - Creates an interactive map with restaurant locations using Folium.
- **Visualization**:
  - Displays restaurants as clusters on an interactive map.

📷 **Visualizations**:
- Restaurant Location Map

![image](https://github.com/user-attachments/assets/6132622e-a0bd-441a-b1ab-fb75fce19861)


---

### **🔹 Part 2: Advanced Insights**

#### 💬 Task 4: Sentiment Analysis
📁 **File Location**: `Task4.ipynb`

- **Objective**: Analyze customer reviews to determine restaurant sentiment.
- **Approach**:
  - Cleans text data (removes stopwords, punctuation, etc.).
  - Applies sentiment analysis using NLP libraries (e.g., VADER, TextBlob).
  - Categorizes reviews into Positive, Neutral, and Negative.
- **Visualization**:
  - Pie charts and bar graphs to show sentiment distribution.

📷 **Visualizations**:
- Aggregate Rating Of Restaurants With Table Booking And Those Without.

![image](https://github.com/user-attachments/assets/34e441b3-0995-4baf-b626-46feb1112afa)

- Availability of Online Delivery Among Restaurants With Different Price Ranges.

![image](https://github.com/user-attachments/assets/589807c8-b9ed-47a6-bf0b-a84a9d46d720)


#### 💰 Task 5: Price vs Rating Correlation
📁 **File Location**: `Task5.ipynb`

- **Objective**: Examine how price affects restaurant ratings.
- **Approach**:
  - Compares price range with average aggregate rating.
  - Uses scatter plots and correlation heatmaps.
- **Findings**:
  - Identifies whether higher-priced restaurants have better ratings.

📷 **Visualizations**:
- Price vs Rating Scatter Plot

![image](https://github.com/user-attachments/assets/142c55b5-031e-4881-b775-405ad05f4475)

- Correlation Heatmap

![image](https://github.com/user-attachments/assets/1539b88f-1e46-4e7d-b337-63f8c1501cb7)


#### 📈 Task 6: Restaurant Rating Prediction
📁 **File Location**: `Task6.ipynb`

- **Objective**: Convert categorical data into numerical format for further analysis.
- **Approach**:
  - Encodes categorical variables using techniques like One-Hot Encoding or Label Encoding.
  - Ensures the dataset is in a structured numerical format.
  - Exports the processed data as CSV or Excel for machine learning models.
  
- **Visualization**:
  -Displays summary statistics of transformed data.

---

## ⚙️ Setup & Installation
To run this project, install the required libraries:
```bash
pip install numpy pandas matplotlib seaborn folium nltk textblob scikit-learn
```
Run the Jupyter notebooks in sequence:
1. `Task1.ipynb`
2. `Task2.ipynb`
3. `Task3.ipynb`
4. `Task4.ipynb`
5. `Task5.ipynb`
6. `Task6.ipynb`

---

## 🤝 Contributing
Feel free to fork this repository and open pull requests with improvements!

---

## 📜 License
This project is open-source under the MIT License.

