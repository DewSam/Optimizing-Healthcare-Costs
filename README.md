# Optimizing Healthcare Costs: Predictive Analytics and Strategic Insights for HMOs

## 1. Description
This project revolves around analyzing healthcare data of 7,583 individuals to provide actionable insights for a Health Management Organization (HMO). The goal is to predict which individuals will have high healthcare costs in the next year, and provide recommendations to reduce these costs based on health and lifestyle attributes. Each row in the dataset represents a person, and the analysis focuses on identifying the key factors driving healthcare expenses.

## 2. Project Scope and Objective
The scope of this project includes analyzing a dataset containing healthcare and lifestyle information for individuals and predicting which people will have high healthcare costs. The project’s main objectives are:
- Predicting individuals with high healthcare costs.
- Providing actionable insights and recommendations to the HMO on how to lower their total healthcare expenses.
- Offering suggestions to patients on areas of improvement to reduce their healthcare costs.

## 3. Project Deliverables
1. **Data Cleaning:** Prepare the data by handling missing and invalid values.
2. **Feature Identification:** Identify attributes that most affect healthcare costs using linear regression, correlation, and visualization techniques.
3. **SVM Model:** Predict whether a patient is expensive or not using a Support Vector Machine (SVM) and provide insights.
4. **Decision Tree Model:** Build a decision tree to predict high-cost patients and provide actionable insights.
5. **Shiny App:** Develop a Shiny app based on the best-performing model to allow interactive exploration of the results.
6. **Recommendations:** Provide data-driven suggestions to the HMO to lower healthcare costs, focusing on less satisfied customer segments.

## 4. Business Questions
This project addresses the following business questions:
1. How do attributes such as BMI, Age, Exercise, and Smoking impact healthcare costs?
2. Why don’t parameters like children, location, education, and marital status affect overall healthcare costs?
3. Which attributes affect healthcare costs the most?
4. How can customers reduce healthcare costs?
5. What types of people incur the highest healthcare costs?
6. Why do some individuals have high healthcare costs?
7. What actions can the HMO take to lower total healthcare expenses?

## 5. Data Acquisition
The dataset contains 7,583 rows representing individuals with 15 attributes, including:
- Age
- BMI
- Gender
- Number of children
- Smoker status
- Location
- Education level
- Yearly physical check-up status
- Exercise habits
- Hypertension status

## 6. Data Cleaning & Preprocessing
### 6.1 Addressing Null Values
- **BMI:** Missing values replaced with the mean.
- **Hypertension:** Missing values replaced with the mode.

### 6.2 Expensive Attribute
A new "Expensive" column was created using a cost threshold of $5,000. Patients with costs above this threshold were labeled as expensive.

## 7. Descriptive Statistics and Visualizations
Several analyses and visualizations were conducted to understand the data:
1. **Exercise vs. Cost:** Non-active individuals spend more on healthcare than active individuals.
2. **Age vs. Cost:** Healthcare costs increase with age.
3. **Smoker vs. Cost:** Smokers incur higher healthcare costs than non-smokers.
4. **BMI vs. Cost:** Individuals with a BMI above 30.5 tend to have higher healthcare costs.
5. **Education Level vs. Cost:** Education level does not significantly impact healthcare costs.
6. **Cost Distribution:** Most individuals spend less than $5,000 on healthcare, with a few incurring higher expenses.

Additional analysis focused on relationships between BMI, smoking, exercise habits, and location vs. healthcare costs.

## 8. Predictive Modeling
### 8.1 Support Vector Machine (SVM)
An SVM model was applied to classify individuals as high-cost or low-cost based on selected attributes like Age, BMI, Smoking, and Exercise habits.

### 8.2 Decision Tree
A decision tree was built for classification, providing interpretable rules for identifying high-cost individuals.

## 9. Shiny App
The Shiny app provides an interactive platform to explore the dataset and model results. Users can input specific attributes to predict whether a patient will be high-cost and visualize healthcare cost distributions across different variables.

## 10. Recommendations
The following actionable insights were provided to the HMO:
- Target smokers and individuals with high BMI for interventions to reduce healthcare costs.
- Encourage physical activity among patients, as non-active individuals tend to incur higher costs.
- Focus on older individuals with higher healthcare costs and provide preventive care to lower future expenses.

## 11. Technologies Used
- R (Data cleaning, visualization and modelling)
- R (Shiny app development)
- Jupyter Notebook for data exploration and model development

## 12. How to Run the Project
1. Clone the repository:
   ```bash
   git clone <repository-url>
