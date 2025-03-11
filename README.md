Healthcare Exploration System
Overview
The Healthcare Exploration System is a Python-based project designed to analyze patient data, identify potential health risks, and visualize key health metrics such as Blood Pressure and Sugar Levels. The program processes data from a CSV file and provides statistical insights to assist in healthcare analysis.

Features
Loads patient data from a CSV file.
Provides basic statistical summaries of patient data.
Identifies patients with high blood pressure or sugar levels.
Generates visualizations to analyze trends in patient health data.
Installation and Setup
Clone the repository
git clone https://github.com/althougharsh/Healthcare-Explorer.git
cd Healthcare-Explorer
Install required dependencies
Ensure Python is installed on your system, then run:

pip install pandas matplotlib

Prepare the CSV file
Create a file named healthcare_data.csv in the project directory and add the patient data in the following format:
PatientID,Age,BloodPressure,SugarLevel,Weight
1,44,118,87.89,105.57
2,39,109,177.32,105.70
3,49,149,144.15,77.79
4,58,121,90.36,115.24
5,35,109,126.42,70.38
6,25,129,95.27,119.05
7,46,132,146.61,62.18
8,28,93,109.75,81.79
9,60,145,103.19,94.64
10,55,125,197.73,118.59
11,41,143,180.58,103.58
12,48,141,181.97,61.45
13,58,93,181.78,50.68
14,35,145,133.39,113.19
15,67,176,87.01,84.94
16,70,109,193.27,77.72
17,43,148,135.94,106.58
18,74,122,129.41,83.30
19,19,147,125.48,74.08
20,56,119,160.72,111.87
Run the script

python healthcare_analysis.py
How It Works
The script reads data from the CSV file and loads it into a Pandas DataFrame.
It calculates statistical summaries such as mean, minimum, maximum, and quartiles.
It identifies patients with Blood Pressure > 140 or Sugar Level > 180 as potential risk cases.
It generates histograms to visualize Blood Pressure and Sugar Level distributions.
Example Output
Basic Statistics:
       PatientID        Age  BloodPressure  SugarLevel      Weight
count  20.000000  20.000000      20.000000   20.000000   20.000000
mean   10.500000  47.000000     126.500000  137.224000   92.104000
std     5.916080  16.270845      25.672592   40.829174   22.498722
min     1.000000  19.000000      93.000000   87.010000   50.680000
25%     5.750000  35.000000     109.000000  109.750000   74.080000
50%    10.500000  47.000000     125.000000  133.385000  103.580000
75%    15.250000  58.000000     145.000000  177.320000  113.190000
max    20.000000  74.000000     176.000000  197.730000  119.050000

Patients at Risk:
    PatientID  Age  BloodPressure  SugarLevel  Weight
3           3   49           149      144.15   77.79
9           9   60           145      103.19   94.64
11         11   41           143      180.58  103.58
12         12   48           141      181.97   61.45
14         14   35           145      133.39  113.19
15         15   67           176       87.01   84.94
16         16   70           109      193.27   77.72
The script also generates two histograms showing the distribution of Blood Pressure and Sugar Levels among the patients.

Technologies Used
Python
Pandas (for data analysis)
Matplotlib (for data visualization)
Contributing
If you'd like to improve this project, feel free to fork the repository and submit a pull request.

License
This project is open-source and available under the MIT License.
