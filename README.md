# 🏥 Healthcare Appointment No-Show Prediction

## 📌 Project Overview

This is a Machine Learning project focused on analyzing healthcare appointment data and predicting whether a patient will attend or miss a scheduled medical appointment.

The main objective is to understand patient appointment patterns and identify factors that may contribute to missed appointments.

## 📂 Dataset

**Dataset Name:** Medical Appointment No Shows

**Source:** [Kaggle – Medical Appointment No Shows](https://www.kaggle.com/datasets/joniarroba/noshowappointments)

- Total Records: 110,527
- Total Features: 14
- File Format: CSV

The dataset contains information about patients, appointment dates, medical conditions, SMS reminders, and appointment attendance.

## 🛠️ Technologies Used

- Python
- Pandas
- Google Colab
- Jupyter Notebook

## 📊 Project Workflow

### Day 1 – Data Loading and Initial Inspection

- Imported Pandas.
- Loaded the dataset.
- Explored data using head(), tail(), info(), describe(), and shape.
- Checked missing values.
- Checked duplicate records.

### Day 2 – Unique Value Analysis and Data Exploration

- Checked unique values across dataset columns.
- Identified categorical and binary features.
- Explored the target variable (No-show).
- Analyzed Age using minimum, maximum, and mean.
- Identified a negative age value for further investigation.

### Day 3 – Data Cleaning and Exploratory Data Analysis (EDA)

**Tasks Completed:**

- Removed one invalid record where Age was -1.
- Analyzed the age distribution of patients.
- Created a histogram to visualize patient age distribution.
- Visualized appointment attendance using a bar chart.
- Calculated the percentage distribution of the target variable (`No-show`).

**Key Findings:**

- Total records after cleaning: 110,526
- Total features: 14
- Patients who attended appointments: 79.81%
- Patients who missed appointments: 20.19%

**Observation:**

The target variable is imbalanced because approximately 80% of patients attended their appointments, while 20% missed them. This will be considered during model training and evaluation.

**Next Steps:**

- Continue exploratory data analysis.
- Analyze categorical and numerical features.
- Perform feature engineering.
- Prepare data for machine learning models.
- ### Day 4 – Feature Analysis and Feature Engineering

**Tasks Completed:**
- Compared gender with appointment attendance.
- Created age groups and analyzed no-show rates.
- Visualized no-show rates by age group.
- Analyzed SMS reminders and scholarship status.
- Explored neighbourhood-wise no-show rates.
- Converted appointment dates into datetime format.
- Created a new feature: `WaitingDays`.

**Key Findings:**
- The 18–35 age group had the highest no-show rate among the analyzed age groups.
- Patients who received SMS reminders showed a higher no-show percentage in this dataset.
- Average waiting time was approximately 10.18 days.
- Median waiting time was 4 days.
- Some negative waiting-day values require further investigation.

**Next Steps:**
- Investigate negative waiting days.
- Complete data preprocessing.
- Train and evaluate machine learning models.
