# Excel Salary Dashboard
![1_Salary_Dashboard_Final_Dashboard](https://github.com/user-attachments/assets/58a3f412-779e-4522-a158-792ce1cc2207)
## Introduction  
This data jobs salary dashboard was created to help job seekers investigate salaries for their desired jobs and ensure they are being adequately compensated.  

The data is a example dataset, which provides a foundation in analyzing data using this powerful tool. The data contains detailed information on job titles, salaries, locations, and essential skills that are presented here.

### Dashboard File

My final dashboard is in [1_Salary_Dashboard.xlsx](https://github.com/user-attachments/files/19545383/1_Salary_Dashboard.xlsx)

### Excel Skills Used

The following Excel skills were utilized for analysis:
* 📊 Charts
* 🧮 Formulas and Functions
* ✅ Data Validation

### Data Jobs Dataset

The dataset used for this project includes detailed information on:
* 👨‍💼 Job titles
* 💵 Salaries
* 📌 Locations
* 🛠️ Skills

## Dashboard Build

### 📈 Charts
#### 📊 Data Science Job Salaries - Bar Chart
![1_Salary_Dashboard_Chart1](https://github.com/user-attachments/assets/34103355-eeca-4f92-9cde-61729ac64fc7)

* 🛠️ **Excel Features**: Utilized bar chart feature (with formatted salary values) and optimized layout for clarity.
* 🎨 **Design Choice**: Horizontal bar chart  for visual comparison of median salaries.
* 📲 **Data Organization**: Sorted job titles by descending salary for improved readability/
* 💡 **Insights Gained**: This enables quick identification of salary trends, noting that Senior roles and Engineers are higher-paying than Analyst roles.

#### 🧭 Country Median Salary - Map Charts
![1_Salary_Dashboard_Country_Map](https://github.com/user-attachments/assets/ed77ce08-b1d1-4ba5-919c-49eaad4feba4)  
* 🛠️ **Excel Features**: Utilized Excel's map chart feature to plot median salaries globally.
* 🎨 **Design Choice**: Color-coded map to visually differentiate salary levels across regions.
* 📊 **Data Representation**: Plotted median salary for each country with available data.
* 👁️ **Visual Enhancement**: Improved readability and immediate understanding of geographic salary trends.
* 💡 **Insights Gained**: Enables quick grasp of global salary disparities and highlights high/low salary regions.

### 🧮 Formulas and Functions
#### 💰 Median Salary by Job titles
```
=MEDIAN(
IF(
    (jobs[job_title_short]=A2)*
    (jobs[job_country]=country)*
    (ISNUMBER(SEARCH(type,jobs[job_schedule_type])))*
    (jobs[salary_year_avg]<>0),
    jobs[salary_year_avg]
)
)
```
* 🔎 **Multi-Criteria**: Checks for job title, country, schedule type, and excludes blank salaries.
* 📊 **Array Formula**: Utilizes `MEDIAN()` function with nested `IF()` statement to analyze an array.
* 🎯 **Tailored Insights**: Provides specific salary information for job titles, regions, and schedule types.
* #️⃣ **Formula Purpose**: This formula populates the table below, returning the median salary based on job title, country, and type specified.

#### 📅 Background Table
![1_Salary_Dashboard_Screenshot1](https://github.com/user-attachments/assets/97a409a6-48cf-473d-998e-5220de1a2403)

#### 📈 Dashboard Implementation
![1_Salary_Dashboard_Job_Title](https://github.com/user-attachments/assets/6199d136-a5c4-4aa0-b0ba-87c5929ab202)

#### ⏰ Count of Job Schedule Type
```=FILTER(J2#,(NOT(ISNUMBER(SEARCH("and",J2#))+ISNUMBER(SEARCH(",",J2#))))*(J2#<>0))```  
* 🔎 **Unique List Generation**: This Excel formula below employs the `FILTER()` function to exclude entries containing "and" or commas, and omit zero values.
* #️⃣ **Formula Purpose**: This formula populates the table below, which gives us a list of unique job schedule types.

#### 📅 Background Table

![1_Salary_Dashboard_Screenshot2](https://github.com/user-attachments/assets/41a081ab-d7fb-48ac-a243-033bcbf1cc71)

#### 📈 Dashboard Implementation

![1_Salary_Dashboard_Type](https://github.com/user-attachments/assets/0b2df1e4-fd6a-4f37-94fa-987d71293fb5)

### ✅ Data Validation

#### 🔎 Filtered List
* 🔒 **Enhanced Data Validation**: Implementing the filtered list as a data validation rule under the `Job Title`, `Country`, and `Type` option in the Data tab ensures.
   * 🎯 User Input is restricted to predefined, validation schedule types
   * 🚫 Incorrect or inconsistent entries are prevented
   * 🏋🏼‍♂️ Overall usability of the dashboard is enhanced

![1_Salary_Dashboard_Data_Validation](https://github.com/user-attachments/assets/d9ef451b-4dc6-444f-8033-60c5e0d6aa8a)

## Conclusion

I created this dashboard to showcase insights into salary trends across various data-related job titles. Utilizing data from the dataset, this dashboard allows users to make informed decisions about their career paths. Exploring the functionalities to understand how location and job type influence salaries.

 ---

## 📬 Contact

For any questions, suggestions, or feedback, feel free to reach out:

- **Email**: [Tushar Yadav](mailto:tyadav940@gmail.com)
- **GitHub**: [tusharyadav99](https://github.com/tusharyadav99/)
- **LinkedIn**: [Tushar Yadav](https://www.linkedin.com/in/tushar-yadav-865237183/)

I would love to hear from you!

---
