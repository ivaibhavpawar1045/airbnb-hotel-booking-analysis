# Airbnb Hotel Booking Analysis

## 📌 Project Overview

**Airbnb Hotel Booking Analysis** is a data analytics project that
analyzes Airbnb listing data to identify meaningful patterns in pricing,
room types, neighbourhoods, reviews, availability, host characteristics,
cancellation policies, and booking options.

The project combines **Python-based Exploratory Data Analysis (EDA)**
with an **interactive Power BI dashboard** to convert raw Airbnb data
into understandable and actionable insights.

------------------------------------------------------------------------

## 🎯 Objectives

-   Analyze Airbnb listing and accommodation patterns.
-   Compare prices across room types and neighbourhoods.
-   Study the relationship between listing price and service fee.
-   Analyze host identity verification and review ratings.
-   Examine the relationship between host listing count and annual
    availability.
-   Study pricing variations across construction years and neighbourhood
    groups.
-   Analyze cancellation policies and instant-booking options.
-   Build interactive visualizations and a Power BI dashboard.
-   Generate data-driven insights for Airbnb hosts, customers, property
    managers, and analysts.

------------------------------------------------------------------------

## 📊 Dataset

The project uses an Airbnb hotel/listing dataset containing information
related to:

-   Listing ID
-   Host details
-   Host identity verification
-   Neighbourhood and neighbourhood group
-   Latitude and longitude
-   Room type
-   Price
-   Service fee
-   Minimum nights
-   Number of reviews
-   Reviews per month
-   Review rating
-   Calculated host listings count
-   Availability
-   Cancellation policy
-   Instant booking
-   Construction year

### Dataset Size

After data cleaning and duplicate listing removal:

-   **Unique listings analyzed:** 102,058
-   **Features used:** 22

------------------------------------------------------------------------

## 🧹 Data Cleaning

The dataset was prepared before analysis using Python and Pandas.

Major preprocessing steps included:

-   Checking duplicate records.
-   Removing duplicate listing IDs.
-   Handling missing categorical values.
-   Standardizing neighbourhood group names.
-   Converting instant-booking values into readable categories.
-   Handling invalid availability values outside the 0--365 day range.
-   Handling unrealistic minimum-night values.
-   Removing columns that were not required for the analytical
    dashboard.

------------------------------------------------------------------------

## 🔍 Exploratory Data Analysis

The following analytical questions were investigated:

1.  What are the different room types available?
2.  Which neighbourhood group has the highest number of listings?
3.  What is the relationship between price and service fee?
4.  How does host identity verification relate to review ratings?
5.  Is there a relationship between calculated host listings count and
    availability?
6.  How does average price vary across construction years?
7.  How does average price vary across neighbourhood groups?
8.  Which neighbourhoods have the highest average prices?
9.  What is the distribution of cancellation policies?
10. What is the distribution of instant-bookable listings?
11. What relationships can be observed between important numerical
    variables?

------------------------------------------------------------------------

## 📈 Key Results

The analysis produced the following major metrics:

  Metric                               Result
  ----------------------------- -------------
  Unique Listings                     102,058
  Average Price                        625.36
  Average Service Fee                  125.04
  Average Review Rating              3.28 / 5
  Total Reviews                     2,803,391
  Average Annual Availability     140.80 days
  Entire Home/Apt Listings             52.35%
  Private Room Listings                45.37%
  Shared Room Listings                  2.16%
  Hotel Room Listings                   0.11%

### Key Insights

-   Entire home/apartment and private room listings form the majority of
    the available listings.
-   Manhattan and Brooklyn contain the largest concentration of
    listings.
-   Listing price and service fee show an observable relationship, with
    variation between individual listings.
-   Review ratings can be compared across host identity verification
    categories to identify differences between host groups.
-   Host portfolio size and annual availability show varying patterns
    across listings.
-   Average prices differ across neighbourhood groups, demonstrating the
    importance of location in Airbnb pricing.
-   Cancellation policies and instant-booking options vary across
    listings.

------------------------------------------------------------------------

## 🛠️ Technology Stack

### Programming & Data Analysis

-   Python
-   Pandas
-   NumPy

### Data Visualization

-   Matplotlib
-   Seaborn

### Development Environment

-   VS Code
-   Jupyter Notebook

### Data Source / Storage

-   Microsoft Excel

### Business Intelligence

-   Microsoft Power BI
-   Power Query
-   DAX

------------------------------------------------------------------------

## 📊 Visualizations

The project includes visualizations such as:

-   Room Type Distribution
-   Listings by Neighbourhood Group
-   Price vs Service Fee Scatter Plot
-   Host Verification vs Review Rating
-   Host Listings Count vs Availability
-   Average Price by Construction Year
-   Average Price by Neighbourhood Group
-   Top 10 Neighbourhoods by Average Price
-   Cancellation Policy Distribution
-   Instant Booking Distribution
-   Correlation Heatmap

------------------------------------------------------------------------

## 📌 Power BI Dashboard

The Power BI dashboard provides an interactive view of the Airbnb
dataset.

### Dashboard Page 1: Airbnb Overview

Includes:

-   Total Listings
-   Average Price
-   Average Rating
-   Total Reviews
-   Average Availability
-   Listings by Room Type
-   Average Price by Room Type
-   Listings by Neighbourhood Group
-   Top 10 Neighbourhoods by Average Price
-   Availability Distribution
-   Cancellation Policy
-   Interactive slicers

### Dashboard Page 2: Pricing & Host Analysis

Includes:

-   Average Price
-   Average Service Fee
-   Average Minimum Nights
-   Average Reviews per Month
-   Average Price by Neighbourhood Group
-   Price vs Number of Reviews
-   Top Hosts by Listing Count
-   Instant Booking Availability
-   Rating Distribution

------------------------------------------------------------------------

## 📁 Project Structure

``` text
Airbnb-Hotel-Booking-Analysis/
│
├── data/
│   └── Airbnb_Hotel_Booking_Analysis_Cleaned.xlsx
│
├── Airbnb_Hotel_Booking_Analysis.ipynb
│
├── outputs/
│   └── charts/
│       ├── room_type_distribution.png
│       ├── neighbourhood_distribution.png
│       ├── price_service_fee.png
│       ├── verification_rating.png
│       ├── host_availability.png
│       ├── construction_price.png
│       ├── neighbourhood_price.png
│       ├── top_10_neighbourhoods.png
│       ├── cancellation_policy.png
│       ├── instant_booking.png
│       └── correlation_heatmap.png
│
├── dashboard/
│   └── Airbnb_Hotel_Booking_Analysis.pbix
│
├── Project_Presentation.pptx
│
└── README.md
```

------------------------------------------------------------------------

## ▶️ How to Run the Project

### 1. Clone the repository

``` bash
git clone https://github.com/YOUR-USERNAME/airbnb-hotel-booking-analysis.git
```

### 2. Navigate to the project

``` bash
cd airbnb-hotel-booking-analysis
```

### 3. Create a virtual environment

``` bash
python -m venv .venv
```

### 4. Activate the environment

#### Windows

``` bash
.venv\Scripts\activate
```

### 5. Install dependencies

``` bash
pip install pandas numpy matplotlib seaborn openpyxl jupyter ipykernel
```

### 6. Open the notebook

Open:

``` text
Airbnb_Hotel_Booking_Analysis.ipynb
```

in VS Code or Jupyter Notebook.

### 7. Run the notebook

Execute the cells sequentially to reproduce the data cleaning, analysis,
and visualizations.

------------------------------------------------------------------------

## 🔮 Future Scope

The project can be extended with:

-   Machine learning-based price prediction.
-   Booking demand prediction.
-   Personalized listing recommendations.
-   Dynamic pricing models.
-   Geospatial analysis using latitude and longitude.
-   Sentiment analysis of guest reviews.
-   Real-time Airbnb data integration.
-   Integration of external data such as weather, events, and economic
    indicators.
-   Advanced host and guest behaviour analysis.

------------------------------------------------------------------------

## 👥 Potential End Users

-   Airbnb Hosts
-   Property Managers
-   Customers
-   Business Analysts
-   Hospitality Businesses

------------------------------------------------------------------------

## 📜 Project Context

This project was developed as part of a **Data Visualization / Data
Analytics learning project** and demonstrates the use of Python,
exploratory data analysis, visualization, and Power BI for solving a
real-world analytics problem.

------------------------------------------------------------------------

## 👨‍💻 Author

**Vaibhav Pawar**

**BE Computer Engineering**\
Suman Ramesh Tulsiani Technical Campus, Pune

------------------------------------------------------------------------

## ⭐ Project Highlights

**Python + Pandas + Matplotlib + Seaborn + Power BI**

Transforming raw Airbnb listing data into meaningful analytical and
business insights.
