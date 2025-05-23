# **Olympic Games Data Analysis**

## **Project Overview** 🎯

This project involves the analysis of the Olympic Games dataset using **SQLite** for database management and **Python** for data manipulation, analysis, and visualization. The goal of this project is to build a relational database for storing Olympic Games data and use **SQL queries** and **Python** tools to gain insights into the history of the Olympic Games.
![Olympics Overview](https://github.com/amramgad8/Olympics-Data-Analysis-Insights-with-Python-and-SQLite/blob/81fa2ce23865dcc3543c717aedaef116d5c84fe3/olympiques.jpeg)
### **Key Features** 🛠️:
- Data cleaning and preprocessing using **pandas**.
- Database creation with **SQLite** to store cleaned data.
- Data analysis using **SQL** and **Python**.
- Data visualization using **matplotlib** and **seaborn** to present key insights.

---

## **Steps Involved** 📝

### **1️⃣ Data Acquisition** 📥

In this step, the data is sourced from two main files:
- **athlete_events.csv**: Contains detailed information about athletes, including personal attributes (age, height, weight) and their participation in various Olympic Games and events.
- **noc_regions.xlsx**: Contains information about regions (countries) and their corresponding NOC codes.

These datasets are read using **pandas** and prepared for further analysis.


### **2️⃣ Data Cleaning** 🧹

- **Handling Missing Values**: We check for missing data using `isnull()` in **pandas** and handle it by imputing or removing the missing values.
- **Removing Duplicates**: We remove any duplicate rows to ensure data consistency.

After cleaning, the data is prepared for transformation and analysis.


### **3️⃣ Data Preparation for Star Schema** 🔄

We begin preparing the **Star Schema** by creating the **Dimension Tables** (e.g., **DimAthletes**, **DimGames**) and the **Fact Table** (**FactResults**). These tables will store descriptive and measurable data, forming the relational structure for efficient analysis.
## **Entity-Relationship Diagram (ERD)** 📊

The diagram below shows the **Star Schema** used to structure the Olympic Games dataset, with the central **FactResults** table connected to the dimension tables: **DimAthletes**, **DimGames**, **DimEvents**, **DimSports**, and **DimCountries**.

![ERD](https://github.com/amramgad8/Olympics-Data-Analysis-Insights-with-Python-and-SQLite/blob/93374efadfafce8bf12d28a3c57da092b35a3ef8/Screenshot%202025-05-09%20015141.png)

### **4️⃣ Create SQLite Database & Tables** 🗃️

We create the **SQLite database** and define the structure of the **Dimension Tables** and the **Fact Table**. This is done using SQL `CREATE TABLE` statements with **primary keys** and **foreign keys** to ensure relationships between tables.

### **5️⃣ Load Data into SQLite Database** 🚀

The cleaned data is loaded into the SQLite database using **pandas** `to_sql()` method. This step inserts the data into the **dimension tables** and **fact table**, making the database ready for analysis.

### **6️⃣ Data Analysis using SQL (via Python)** 📊

We use **SQL queries** to extract valuable insights, such as:
- Top countries by medal count.
- Age distribution among athletes.
- Top athletes with the most medals.
- Cities that hosted both Summer and Winter Olympics.


---

## **Technologies Used** 🛠️

- **Python**: For data manipulation, analysis, and visualization.
- **SQLite**: For storing and managing data.
- **pandas**: For data cleaning and preparation.
- **matplotlib** & **seaborn**: For visualizing the analysis results.

---

## **Setup & Installation** ⚙️

To run this project locally, follow these steps:

1. **Clone this repository**:
   ```bash
   git clone https://github.com/your-username/olympics-data-analysis.git
   cd olympics-data-analysis

2. **Install dependencies**:

   * Ensure **Python** is installed on your system.
   * Install required libraries using **pip**:

     ```bash
     pip install -r requirements.txt
     ```

3. **Run the Jupyter Notebook**:

   * Start Jupyter Notebook in the project directory:

     ```bash
     jupyter notebook
     ```
   * Open the **Olympics Data Analysis** notebook and run the cells to execute the analysis.

---


---

```

