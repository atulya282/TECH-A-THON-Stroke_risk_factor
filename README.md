# TECH-A-THON-Stroke_risk_factor
## Team name - PATTERNS
### Team members
#### Bund Agarwal<br />Hritik Kumar<br />Atulya
## DESCRIPTION
Healthcare today is witnessing a revolution due to it's amalgamation with technology. In our project, Stroke Risk Factor, we focus on how machine learning can bring about unforeseen and implementable results in healthcare.<br />
### STEPS OF EXECUTION
#### Exploratory Data Analysis
We begin by reading data from our CSV file to our Pandas Dataframe. To check the datatypes and non null values, .info() is used. This gives the number of entries in the dataframe and the Non-null count of each variable. 
  **S.No.**| **Column**          |**Non-Null Count**|**Dtype** |
----------- |-----------|---------------|------------
 0 |  id               |  5110 non-null|   int64 || 
 1 | gender           |  5110 non-null|   object |
 2 |  age              |  5110 non-null|  float64|
 3 |  hypertension     |  5110 non-null|   int64  |
 4 |  heart_disease    |  5110 non-null|   int64  |
 5 |  ever_married     |  5110 non-null|   object |
 6 |  work_type        |  5110 non-null|   object |
 7 | Residence_type   |  5110 non-null|   object |
 8 |  avg_glucose_level|  5110 non-null|   float64|
 9 |  bmi              |  4909 non-null|   float64|
 10|  smoking_status   |  5110 non-null|   object |
 11| stroke           |  5110 non-null|   int64 |
 ##### Missing data and LabelEncoder
 From the table we can observe that there are some missing BMI values and 5 non-numerical valued variables. Firstly, we deal with the missing data (BMI values in our case) by replacing them with mean values. Then by using ***LabelEncoder***, we replace the string values stored in the gender, ever_married, work_type, Residence_type and smoking_status with integer values.<br />
<br />
**Graphical Analysis**<br />
Using Mutual Info Classifier, we plot a bar graph to should interdepency between stroke risk factor and the variable. In the bar graph below, the lesser the corresponding variable value across the axes, the lesser it's contribution in deciding the risk factor.
<img src="https://github.com/atulya282/TECH-A-THON-Stroke_risk_factor/blob/main/Screenshot%20(144).png" alt="Risk factor dependency" width="700"/><br />
For every variable, we plot graphs to help in better visualization
 

