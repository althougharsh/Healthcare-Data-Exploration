Healthcare Data Analysis

Overview

This project provides an analysis of healthcare data, focusing on key health metrics such as:


Age

Blood Pressure

Sugar Level

Weight

The analysis includes:

✅ Generating basic statistics

✅ Identifying patients at risk

✅ Visualizing the distribution of key health metrics


Features

📌 Load Data

The script loads a predefined dataset of 20 patients with attributes:


Patient ID

Age

Blood Pressure

Sugar Level

Weight

📌 Statistics

Displays key statistical insights, such as:

✔ Mean

✔ Median

✔ Standard Deviation


📌 Risk Identification

Identifies patients at risk based on abnormal readings:


Blood Pressure > 140

Sugar Level > 180

📌 Data Visualization

Provides histograms to better understand the distribution of blood pressure and sugar levels.


Requirements

To run this script, you'll need the following Python libraries:

pip install pandas matplotlib

Usage


cd Healthcare-Data-Analysis

Run the script

python healthcare_analysis.py

What the script does

1️⃣ load_data() → Loads a sample dataset with attributes: Patient ID, Age, Blood Pressure, Sugar Level, and Weight

2️⃣ display_statistics(df) → Displays mean, median, standard deviation of the dataset

3️⃣ identify_risk_patients(df) → Identifies patients with abnormal readings

4️⃣ plot_data(df) → Generates histograms to show distribution of blood pressure and sugar levels


Example Output


Basic Statistics:

Age        BloodPressure  SugarLevel  Weight

20.0       124.75        146.59      93.31

std        14.36         18.45       32.08

min        19.0          93.00       87.50

25%        35.5          109.50      123.81

75%        55.0          133.94      93.46

Patients at Risk

PatientID  BloodPressure  SugarLevel  Weight

2          149           144.15      77.79

9          197.73        118.59      10

11         141           181.97      61.41

License

This project is licensed under the MIT License.

