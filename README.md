# 🏨EDA Hotel Analysis

##Project Overview

**Hotel Harmony – Data Insights for Optimized Operations** is a data analysis project focused on understanding hotel booking patterns, guest behavior, cancellations, pricing, and operational performance.

The project uses the **Hotel Bookings Dataset** and applies **Python-based Exploratory Data Analysis (EDA)** to identify meaningful patterns and generate data-driven insights.

The analysis covers booking behavior, hotel types, arrival trends, cancellations, Average Daily Rate (ADR), market segments, distribution channels, guest types, room preferences, and special requests.

---

## Project Objectives

The main objectives of this project are:

* Analyze hotel booking patterns.
* Understand booking distribution across hotel types.
* Analyze booking cancellations.
* Identify the most common arrival months.
* Study Average Daily Rate (ADR).
* Analyze booking behavior by country.
* Examine market segments and distribution channels.
* Study the relationship between lead time and cancellations.
* Analyze guest stay duration.
* Compare new and repeated guests.
* Identify the most popular reserved room types.
* Analyze special requests and their relationship with ADR.
* Identify important operational patterns and trends.

---

## Dataset

### Hotel Bookings Dataset

**Dataset:** `hotel_bookings.csv`

The dataset contains information related to hotel reservations and guest bookings.

Important attributes include:

| Column                          | Description                                |
| ------------------------------- | ------------------------------------------ |
| **hotel**                       | Type of hotel                              |
| **is_canceled**                 | Cancellation status                        |
| **lead_time**                   | Number of days between booking and arrival |
| **arrival_date_year**           | Arrival year                               |
| **arrival_date_month**          | Arrival month                              |
| **arrival_date_week_number**    | Arrival week                               |
| **arrival_date_day_of_month**   | Arrival day                                |
| **stays_in_weekend_nights**     | Weekend nights stayed                      |
| **stays_in_week_nights**        | Weekday nights stayed                      |
| **adults**                      | Number of adults                           |
| **children**                    | Number of children                         |
| **babies**                      | Number of babies                           |
| **country**                     | Guest country                              |
| **market_segment**              | Booking market segment                     |
| **distribution_channel**        | Booking distribution channel               |
| **reserved_room_type**          | Reserved room type                         |
| **previous_cancellations**      | Previous cancellations                     |
| **booking_changes**             | Number of booking changes                  |
| **adr**                         | Average Daily Rate                         |
| **required_car_parking_spaces** | Required parking spaces                    |
| **total_of_special_requests**   | Number of special requests                 |

---

## Technologies Used

| Technology                     | Purpose                   |
| ------------------------------ | ------------------------- |
| **Python**                     | Data analysis             |
| **Pandas**                     | Data manipulation         |
| **NumPy**                      | Numerical operations      |
| **Matplotlib**                 | Data visualization        |
| **Seaborn**                    | Statistical visualization |
| **Jupyter Notebook / VS Code** | Development environment   |

---

## Project Workflow

```text
Data Collection
      ↓
Data Loading
      ↓
Data Inspection
      ↓
Missing Value Analysis
      ↓
Data Cleaning
      ↓
Feature Engineering
      ↓
Descriptive Statistics
      ↓
Basic Analysis
      ↓
Medium-Level Analysis
      ↓
Data Visualization
      ↓
Key Insights
```

---

## Data Exploration

The project begins by loading the hotel booking dataset and examining:

* Dataset dimensions
* Column names
* First few records
* Random sample records
* Data types
* Missing values
* Duplicate records

This provides an initial understanding of the dataset before performing analysis.

---

## Data Cleaning

The following data-cleaning operations were performed:

* Created a copy of the original dataset.
* Replaced missing `agent` values with **Unknown**.
* Replaced missing `company` values with **Unknown**.
* Replaced missing `children` values with `0`.
* Replaced missing `country` values with **Unknown**.
* Converted `reservation_status_date` to datetime format.
* Identified duplicate rows.
* Removed duplicate records.
* Converted numerical columns to numeric data types.
* Replaced the negative ADR value with a missing value.
* Created a new `total_stay_nights` feature.
* Created a readable cancellation label.
* Ordered arrival months chronologically.

These steps prepare the dataset for reliable analysis and visualization.

---


# Analysis Performed

## 1. Basic-Level Analysis

The project answers several fundamental hotel operations questions.

### Booking Analysis

* Average booking lead time
* Booking distribution by hotel type
* Number of canceled bookings
* Most common arrival month
* Average number of special requests
* Country with the highest number of bookings

### Pricing Analysis

* Average ADR for each hotel type
* Average ADR by market segment
* ADR trend across years

### Guest & Stay Analysis

* Average weekday stay
* Average weekend stay
* Bookings made through travel agents
* New vs repeated guest stay duration
* Most popular reserved room type

The corresponding calculations are implemented in the analysis code.

---

# Visualizations

The project contains multiple visualizations to understand hotel operations.

### Basic-Level Visualizations

1. **Distribution of Bookings by Hotel Type**
2. **Bookings by Arrival Month**
3. **Booking Cancellation Distribution**
4. **Frequency of Special Requests**
5. **Average ADR by Hotel Type**
6. **Top 10 Countries by Number of Bookings**

These visualizations provide a graphical overview of booking and operational patterns.

---

# 📊Medium-Level Analysis

The project also performs more detailed analysis.

### Cancellation Analysis

* Cancellation rate by hotel type
* Relationship between lead time and cancellation
* Previous cancellations by hotel type

### Revenue & Pricing Analysis

* Average ADR by market segment
* ADR trend over the years
* Monthly ADR-based revenue proxy
* Relationship between special requests and ADR

### Guest Analysis

* Average stay duration of new and repeated guests
* Most popular reserved room types

### Booking Channel Analysis

* Distribution of bookings by distribution channel
* Identification of the distribution channel with the highest number of bookings

The medium-level calculations are implemented using grouping, correlation, and aggregation techniques.

---

# 📉 Medium-Level Visualizations

The project includes the following advanced visualizations:

1. **Cancellation Rate by Hotel Type**
2. **Average ADR by Market Segment**
3. **Lead Time vs Cancellation**
4. **Average ADR Trend Over the Years**
5. **Total ADR by Arrival Month**
6. **Special Requests vs ADR**
7. **Stay Duration: New vs Repeated Guests**
8. **Most Popular Reserved Room Types**

These visualizations help identify relationships between booking behavior, cancellations, pricing, guest characteristics, and hotel operations.

---

# 🔑 Key Questions Answered

This project helps answer questions such as:

* Which hotel type receives more bookings?
* What is the average booking lead time?
* Which month has the highest number of arrivals?
* How many bookings are canceled?
* Which country contributes the highest number of bookings?
* What is the average ADR for each hotel type?
* Which market segment has the highest ADR?
* Which distribution channel receives the most bookings?
* Is there a relationship between lead time and cancellation?
* How does ADR change over the years?
* Which month has the highest total ADR?
* Do special requests have a relationship with ADR?
* Do repeated guests have different stay durations?
* Which room type is reserved most frequently?

---

# 📁 Project Structure

```text
Hotel-Operations-Analysis/
│
├── data/
│   └── hotel_bookings.csv
│
├── notebooks/
│   └── Hotel_Operations_Analysis.ipynb
│
├── visualizations/
│   └── charts/
│
├── README.md
│
└── requirements.txt
```

---

# How to Run the Project

## Step 1: Clone the Repository

```bash
git clone <your-github-repository-url>
```

## Step 2: Navigate to the Project Folder

```bash
cd Hotel-Operations-Analysis
```

## Step 3: Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn
```

## Step 4: Open the Notebook

Using Jupyter Notebook:

```bash
jupyter notebook
```

Or open the project in **VS Code**.

## Step 5: Run the Analysis

Run the notebook cells in sequence:

```text
Data Loading
      ↓
Data Cleaning
      ↓
Feature Engineering
      ↓
Descriptive Statistics
      ↓
Basic Analysis
      ↓
Medium-Level Analysis
      ↓
Visualization
      ↓
Insights
```

---

# Conclusion

The **Hotel Harmony – Hotel Operations Analysis** project provides a structured analysis of hotel booking data using Python.

The project examines booking patterns, cancellations, guest behavior, room preferences, pricing, market segments, distribution channels, and operational factors.

Through data cleaning, statistical analysis, feature engineering, and visualization, the project demonstrates how raw hotel booking data can be transformed into meaningful analytical insights.

---

# 👩‍💻 Author

## **Amisha**

**M.Tech – Computer Science Engineering**
**Aspiring Data Analyst**

### Skills Demonstrated

```text
Python
Pandas
NumPy
Matplotlib
Seaborn
Exploratory Data Analysis
Data Cleaning
Data Visualization
Statistical Analysis
Feature Engineering
```

---

## ⭐ Acknowledgement

This project was developed as part of a **Data Analytics / Exploratory Data Analysis project** using the **Hotel Bookings Dataset**.

The project focuses on applying practical data analysis techniques to understand hotel operations and booking behavior.
