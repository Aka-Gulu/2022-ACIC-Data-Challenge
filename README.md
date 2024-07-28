# 2022-ACIC-Data-Challenge

Our notebooks mentioned below are used for building and evaluating various statistical models 
as part of our ACIC 2022 Data Challenge Project. These models are designed to estimate the 
effects of certain interventions using methods commonly employed in causal inference studies.

Repository Structure
Notebooks
1. Group 6_Exploratory Data Analysis
o Description: This notebook includes the exploratory data analysis for the 
methods listed below. Each method provides important aspects of the data we 
are dealing with which is necessary to understand any underlying biases and 
confounders.
o Methods Covered:
§ Data Inspection and Covariate Balance Diagnostic
§ Subgroup Analysis for Treatment Effect Heterogeneity

2. Group 6_Model Analysis 1.ipynb
o Description: This notebook includes the model building and evaluation for the 
methods listed below. Each model is constructed and assessed to determine its 
effectiveness in estimating causal impacts.
o Methods Covered:
§ Simple Linear Regression
§ Propensity Score Matching (PSM)
§ Propensity Score Stratification (PSS)
§ Simple DiD method
§ Simple DiD method for year 2 & 3 comparison
§ DiD with Interaction Terms and IPTW

3. Group 6_Model Analysis 2_1.ipynb
o Description: This notebook focuses on the model building for the DiD with IPW 
method, detailing the setup and implementation of the model.
o Methods Covered:
§ DiD with IPW (Model Building)

4. Group 6_Model Analysis 2_2.ipynb
o Description: Complements the previous notebook by providing a detailed 
evaluation of the DiD with IPW model constructed in 'Group 6_Model Analysis 
2_1.ipynb'. This includes assessing the model's performance and analyzing 
residuals.
o Methods Covered:
§ DiD with IPW (Model Evaluation)

Running the Notebooks
Follow below instructions to run these notebooks successfully:
• Ensure you have Jupyter Notebook or JupyterLab installed or other platform that runs 
ipynb file.
• It is recommended to use a virtual environment to manage dependencies.
• Install required libraries like pandas, numpy, statsmodels, scikit-learn, matplotlib, etc.
• Sequence to run the notebooks is as below:
§ Step 1: Make sure datasets: practice, practice_year and 
ACIC_estimand_truths.csv are downloaded/loaded
§ Step 2: Change file path if needed
§ Step 3: Exceute Group 6_Exploratory Data Analysis.ipynb 
§ Step 4: Execute Group 6_Model Analysis 1.ipynb
§ Step 5: Execute Group 6_Model Analysis 2_1.ipynb
§ Step 6: Execute Group 6_Model Analysis 2_2.ipynb (note this 
notebook has dependency on csv generated from step 5)
