# TECH-A-THON-Stroke_risk_factor
## Team name - PATTERNS
## Domain - Health and safety
### Domain - Machine Learning
### Team members
#### Atulya <br/>Bund Agarwal<br />Hritik Ritesh<br/>
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
Using Mutual Info Classifier, we plot a bar graph to should interdepency between stroke risk factor and the variable. In the bar graph below, the lesser the corresponding variable value across the axes, the lesser it's contribution in deciding the risk factor for stroke.
<img src="https://github.com/atulya282/TECH-A-THON-Stroke_risk_factor/blob/main/Screenshot%20(144).png" alt="Risk factor dependency" width="700"/><br />
<br />
For every variable, we plot graphs to help in better visualization. In each of the following graphs we can see which categorization of the variable gets a higher ratio of stroke cases.<br />
<br />
<img src="https://github.com/atulya282/TECH-A-THON-Stroke_risk_factor/blob/main/Screenshot%20(155).png" width="300"/>
<img src="https://github.com/atulya282/TECH-A-THON-Stroke_risk_factor/blob/main/Screenshot%20(157).png" width="300"/>
<img src="https://github.com/atulya282/TECH-A-THON-Stroke_risk_factor/blob/main/Screenshot%20(158).png" width="300"/>
<img src="https://github.com/atulya282/TECH-A-THON-Stroke_risk_factor/blob/main/Screenshot%20(159).png" width="300"/>
<img src="https://github.com/atulya282/TECH-A-THON-Stroke_risk_factor/blob/main/Screenshot%20(160).png" width="300"/>
<img src="https://github.com/atulya282/TECH-A-THON-Stroke_risk_factor/blob/main/Screenshot%20(161).png" width="300"/><br />
This leads us to deciding on which factors to include in our model's execution. Residence, gender and ID are inconsequential in deciding the risk factor for the stroke. Therefore those will be dropped in the model execution.
### Logistic Regression
Following is the number of stroke cases:<br />
<img src="https://github.com/atulya282/TECH-A-THON-Stroke_risk_factor/blob/main/Screenshot%20(147).png" alt="" width="600"/><br />
Logistic regression is a statistical model that in its basic form uses a logistic function to model a binary dependent variable, although many more complex extensions exist.
It is similar to linear regression but is used to model the probability of a finite number of outcomes, typically two. There are a number of reasons why logistic regression is used over linear regression when modeling probabilities of outcomes (see here). In essence, a logistic equation is created in such a way that the output values can only be between 0 and 1.<br />
We apply Logistic Regression in our model due to the high compatibility of datatypes, outcome and classification nature of our problem.
##### Accuracy of Model
Accuracy=0.9405320813771518
##### Matrix Description
A confusion matrix is a technique for summarizing the performance of a classification algorithm.
COLUMN 1 |	COLUMN 2
------|------
True positive	|1202
False positive |	1
False negative |	75
True negative	| 0




 

