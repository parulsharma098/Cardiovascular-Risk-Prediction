# Cardiovascular Risk Prediction
------
![This is an image](https://cpb-eu-w2.wpmucdn.com/blogs.brighton.ac.uk/dist/f/6375/files/2019/12/website-pic-2.gif)

*This project is based upon a medical domain dataset, and it has been collected from various patients. It includes entries of over 3000 patients and has 16 different attributes for the prediction of **Coronary Heart Diseases** in patients for the next 10 years.*

#### Tags: Classification, Python, Machine learning, Data Science
#### Team members: Parul Sharma, Shivank Dubey
#### Links: Project Presentation: [SlideShow](https://docs.google.com/presentation/d/1NW_sfkkuO1YEilrpqhfQq_EMWiCL9czEXIDXBTc6ooI/edit#slide=id.p)

### PROBLEM STATEMENT:
-----
The dataset is from an ongoing cardiovascular study on residents of the town of Framingham, Massachusetts.The dataset provides the patient's information. It includes over 4,000 records and 15 attributes.
### OBJECTIVE:
-----
The classification goal is to predict whether the patient has a 10-year risk of future coronary heart disease (CHD) considering the other features.
### KEY FACTS:
-----
- Cardiovascular diseases (CVDs) are the leading cause of death globally, taking an estimated 17.9 million people died from CVDs in 2019, representing 32% of all global deaths. Of these deaths, 85% were due to heart attack and stroke.
- More than four out of five CVD deaths are due to heart attacks and strokes, and one third of these deaths occur prematurely in people under 70 years of age.
- The most important behavioural risk factors of heart disease and stroke are unhealthy diet, physical inactivity, tobacco use and harmful use of alcohol.
- Over three quarters of CVD deaths take place in low- and middle-income countries.

### Variables
*Each attribute is a potential risk factor. There are both demographic, behavioral, and medical risk factors.*

#### Data Description

##### Demographic:
• **Sex:** male or female("M" or "F")

• **Age:** Age of the patient;(Continuous - Although the recorded ages have been truncated to whole numbers, the concept of age is continuous)

##### Behavioral:
• **is_smoking:** whether or not the patient is a current smoker ("YES" or "NO")

• **Cigs Per Day:** the number of cigarettes that the person smoked on average in one day.(can be considered continuous as one can have any number of cigarettes, even half a cigarette.)

##### Medical( history):
• **BP Meds:** whether or not the patient was on blood pressure medication (Nominal)

• **Prevalent Stroke:** whether or not the patient had previously had a stroke (Nominal)

• **Prevalent Hyp:** whether or not the patient was hypertensive (Nominal)

• **Diabetes:** whether or not the patient had diabetes (Nominal)

##### Medical(current):
• **Tot Chol:** total cholesterol level (Continuous)

• **Sys BP:** systolic blood pressure (Continuous)

• **Dia BP:** diastolic blood pressure (Continuous)

• **BMI:** Body Mass Index (Continuous)

• **Heart Rate:** heart rate (Continuous - In medical research, variables such as heart rate though in fact discrete, yet are considered continuous because of large number of possible values.)

• **Glucose:** glucose level (Continuous)

##### Predict variable (desired target):
• **10-year risk of coronary heart disease CHD** - DEPENDANT VARIABLE
## STEPS INVOLVED DOING THIS PROJECT:

Import data from dataset and perform initial high-level analysis: look at the number of rows, look at the missing values, look at dataset columns and their values respective to the target variable.

Clean the data: remove irrelevant columns, deal with missing and incorrect values, turn categorical columns into dummy variables.

Use machine learning techniques to predict the Risk of CHDs and to find out factors, which affect target variable.

### LIST OF CLASSIFICATION MODELS BUILT IN THIS PROJECT:
| Sr.  |          MODELS             | TEST ACCURACY |
|-----:|-----------------------------|---------------|
|     1| LOGISTIC REGRESSION         |   **0.6621**  |
|     2| DECISION TREE CLASSIFIER    |   **0.7613**  |
|     3| RANDOM FOREST CLASSIFIER    |   **0.8512**  |
|     4| KNN CLASSIFIER              |   **0.9986**  |
|     5| NAIVE BAYES CLASSIFIER      |   **0.7975**  |
|     6| XGBOOST CLASSIFIER          |   **0.9745**  |
|     7| SUPPORT VECTORMACHINE       |   **0.7104**  |

# Conclusions:
**In conclusion, All the features provided in the dataset are extremely important and contribute towards the risk of getting CHDs. Although, we can conclude some majorly important features like:**

- **As age increases the risk of getting diagnosed with heart disease also increases.**

- **Cigarette consumption is also a major factor that causes CHDs.**

- **Patients having Diabetes and cholesterol problems show a higher risk of CHDs.**

- **Patients having high glucose levels are more prone to CHDs.**

- **Patients with a history of “strokes” have a higher chance of developing CHDs.**

- **Patients with high BMI(Body Mass Index) are at more risk of getting diagnosed with CHDs.**

- **Finally we can say that, XGBoost Classifier has performed best among all the models with the accuracy of 97% & f1-score of 0.9745. It is by far the second highest score we have achieved.So,It's safe to say that XGBoost Classifier provides an optimal solution to our problem.**
