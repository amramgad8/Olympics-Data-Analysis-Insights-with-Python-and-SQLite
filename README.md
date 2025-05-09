# **Olympic Games Data Analysis**

## **Project Overview** 🎯

This project involves the analysis of the Olympic Games dataset using **SQLite** for database management and **Python** for data manipulation, analysis, and visualization. The goal of this project is to build a relational database for storing Olympic Games data and use **SQL queries** and **Python** tools to gain insights into the history of the Olympic Games.

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

![Data Acquisition](images/data_acquisition.png)  <!-- Add the image of data acquisition here -->

### **2️⃣ Data Cleaning** 🧹

- **Handling Missing Values**: We check for missing data using `isnull()` in **pandas** and handle it by imputing or removing the missing values.
- **Removing Duplicates**: We remove any duplicate rows to ensure data consistency.

After cleaning, the data is prepared for transformation and analysis.

![Data Cleaning](images/data_cleaning.png)  <!-- Add the image of data cleaning here -->

### **3️⃣ Data Preparation for Star Schema** 🔄

We begin preparing the **Star Schema** by creating the **Dimension Tables** (e.g., **DimAthletes**, **DimGames**) and the **Fact Table** (**FactResults**). These tables will store descriptive and measurable data, forming the relational structure for efficient analysis.

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

Results are visualized using **matplotlib** and **seaborn**.

![Data Analysis](images/data_analysis.png)  <!-- Add the image of data analysis here -->

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
````

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

## **Usage** 🔍

Once the project is set up, you can run the various steps in the Jupyter Notebook to:

* Import and clean the data.
* Create the SQLite database and tables.
* Perform SQL queries to analyze the Olympic Games data.
* Visualize the results using **matplotlib** and **seaborn**.

---

## **Contributions** 🤝

If you would like to contribute to this project, feel free to fork the repository and submit a **pull request** with your changes.

---

## **License** 📄

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

```

### **Key Points**:
1. **Images**: 
   - Add your images for each section (e.g., data acquisition, data cleaning, etc.) by replacing `images/data_acquisition.png` with the correct image path.
   - You can add images by placing them in a folder named `images/` in your repository.
   
2. **Emojis**: Used throughout to make the README more engaging.

3. **Clear Instructions**: The setup and usage instructions are simple, guiding the user through the project setup.

---

هل هذا مناسب؟ إذا كنت بحاجة لتعديل أو إضافة شيء آخر، أنا جاهز!
```
