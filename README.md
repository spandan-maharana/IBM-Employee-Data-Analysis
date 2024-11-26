# IBM Employee Data Analysis

## Description
This project analyzes IBM's employee dataset, which includes demographic information and various aspects like job roles, hourly rates, education levels, and business travel data. The goal is to derive insights from this dataset, such as understanding employee distribution across departments, salary trends, and other key metrics.

## Project Overview
The project involves analyzing IBM's HR dataset to uncover patterns and trends related to employee attributes. This analysis is supported by several visualizations that segment employees based on attributes like:
1. Age
2. Gender
3. Hourly rate
4. Job role
5. Education level
6. Department
7. Marital status
8. Business travel status


### Technologies Used
1. Python (for data analysis and processing)
2. Pandas (for data manipulation)
3. Matplotlib / Seaborn (for data visualization)
4. Excel (for storing and managing employee data)
5. Jupyter Notebook (if used for running analysis)

## Data Source
IBM.xlsx : IBM's HR dataset to uncover patterns and trends related to employee attributes.

## Getting Started
### Prerequisites
To get started with the analysis, you’ll need the following:
1. Python: Ensure that Python is installed on your machine.
2. Required Libraries: pip install pandas matplotlib seaborn
3. IBM HR Dataset: Download the IBM.xlsx file and extract it to your working directory.

### Installation Instructions
1. Download the IBM.xlsx file to your local machine.

2. Open the dataset using Python or your preferred tool:
import pandas as pd
#Load the main dataset
df = pd.read_excel('IBM.xlsx', sheet_name='IBM HR Dataset')

#Display the first few rows of the dataset
print(df.head())

### Running the Analysis
1. Load the Dataset: Load the IBM HR dataset using Pandas:
df = pd.read_excel('IBM.xlsx', sheet_name='IBM HR Dataset')

2. Explore Different Sheets: You can explore different aspects of the employee data by looking at specific sheets, such as:
a. Employees by Age: Age distribution of IBM employees.
b. Employees by Job Role: Employee count by job role.
c. Employees by Gender: Gender distribution across the company.
d. Employees by Department: Employee distribution by department.

For example:
age_data = pd.read_excel('IBM.xlsx', sheet_name='Employees by Age')
print(age_data.head())

3. Visualizations: Visualize key metrics such as employee distribution, salary trends, and more using Matplotlib or Seaborn.
Example:
import matplotlib.pyplot as plt
import seaborn as sns

#Visualizing the age distribution
sns.histplot(df['Age'])
plt.title('Age Distribution of IBM Employees')
plt.show()
