# 2022-ACIC-Data-Challenge

Our notebooks mentioned below are used for building and evaluating various statistical models 
as part of our [ACIC 2022 Data Challenge Project](https://acic2022.mathematica.org/)  These models are designed to estimate the 
effects of certain interventions using methods commonly employed in causal inference studies.

## Repository Structure
## Notebooks
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

## Running the Notebooks
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






# Window-Manufacturing-DSS

## Shiny App Demo and Presentation
[Shiny app link](https://jensenren.shinyapps.io/test/)  

[Presentation video link](https://drive.google.com/file/d/1madBGUTI6_453hEE7OGBcnkW1289v0_V/view?usp=sharing)

## General Description
This project involves developing a Shiny application that serves as a Decision Support System (DSS) to help identify optimal manufacturing process settings, suppliers, and customer window specifications to reduce the window breakage rate. The project demonstrates the integration of descriptive, predictive, and prescriptive analytics using R libraries and functions.

## Project Description
The Shiny app developed in this project aims to provide actionable insights and recommendations to window manufacturing technicians. It leverages interactive data analytics to support decision-making and improve manufacturing processes. The application includes the following components:

### Descriptive Analytics
- Utilizes the `ggplot2` library to create visually appealing graphs that highlight key relationships in the data.
- Includes various descriptive statistics and summaries to understand the current state of the manufacturing process.

### Predictive Analytics
- Implements linear regression models using the `lm()` and `caret` libraries to predict window breakage rates based on different process settings.
- Displays the estimated parameters and p-values, as well as model fit evaluation statistics.

### Prescriptive Analytics
- Uses the final predictive model as an objective function in an optimization model.
- Identifies controllable and non-controllable decision variables, allowing users to set values for non-controllable variables and solve for optimal settings.
- Adds relevant constraints to ensure the solution is practical and within the scope of the original data.

## Dataset
The dataset used in this project, `Window_Manufacturing.xlsx`, contains various parameters related to the manufacturing process of windows. It includes information such as supplier details, process settings, and breakage rates. The data is used to build and validate the descriptive, predictive, and prescriptive models in the Shiny app.

## Outcomes
The Shiny app provides the following outcomes:
- Visualizations and descriptive statistics that offer insights into the factors affecting window breakage rates.
- Predictive models that estimate the likelihood of window breakage based on different settings.
- Optimal recommendations for process settings to minimize window breakage rates, improving overall manufacturing efficiency.

## Usage
To run the Shiny app locally:
1. Clone this repository to your local machine.
2. Open the R project file in RStudio.
3. Install the required libraries using `install.packages()` if not already installed.
4. Run the app by executing `shiny::runApp('path_to_app')`.

## Conclusion
This project showcases the application of R for developing a comprehensive DSS that integrates various analytics methods. The Shiny app serves as a valuable tool for window manufacturing technicians to make data-driven decisions and enhance the efficiency and quality of the manufacturing process.
