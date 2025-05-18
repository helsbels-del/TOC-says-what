# TOC Says What

## Project Overview
Water quality monitoring is an important public health concern. Disinfection by-products such as Trihalomethanes (THMs) can be harmful in high accumulative concentrations. These chemical compounds are formed when disinfectants, used to treat the raw water, react with the organic carbon material that is naturally found in raw waters.
This project uses machine learning to predict THM concentrations based on TOC and other water quality features, identify the conditions under whcih the THM levels become unsafe, and also help in managing chemical dosing strategies.

## Dataset Content

The dataset used for this project is taken from a Kaggle water potability dataset.
All of the data is public and therefore no privacy or ethical issues have been breached.
It contains 3,276 water samples and 10 variables.
The variables are:
- pH
- Hardness
- Solids
- Chloramines
- Sulfate
- Conductivity
- TOC
- Trihalomethanes
- Turbidity
- Potability

## Business Requirements

Business requirement 1 - Accurately Predict THM Levels Using Available Water Quality Data.
The system must be able to predict Trihalomethane (THM) concentrations in drinking water using routinely monitored parameter Total Organic Carbon (TOC).
This prediction will help identify potential THM exceedances before chlorine dosing decisions are made.
By forecasting THM levels ahead of time, treatment plant operators can adjust chlorine dosing or activate additional treatment steps proactively, reducing the risk of regulatory violations and public health concerns.

Business requirement 2 - Identify the conditions resuulting in high THM levels.
The system must provide insights into the most influential water quality parameters contributing to high THM levels. This feature will support decision-makers in adjusting treatment strategies and monitoring priorities.
Understanding the key contributors to THM formation allows water quality teams to prioritize monitoring efforts (e.g., focus on TOC spikes) and implement targeted interventions.

# Hypothesis and how to validate?

Hypothesis 1

- Higher TOC levels means higher THM concentrations.  
  Validation: Use correltation analysis between TOC and THM (Trihalomethanes).
  Visulaise with scatter plots and trend lines.
  Fit a linear regression model and check the coefficient significance for TOC.

Hypothesis 2

- A ML model can predict THM levels with at least 70% accuracy using water quality features.
  Validation: Train regression models (Random Forest, XGBoost), Evaluate performance usiing R2, MAE and RMSE, ensure >70% on the test set.

## The rationale to map the business requirements to the Data Visualizations and ML tasks

# Buisness requirement 1

- To predict THMs accurately, we need to train regression  models on TOC
- We can use Pearsons method to detect a linear relationship.
- Otherwise the Spearman's method can detect monotonic relationships.
  
  



* List your business requirements and a rationale to map them to the Data Visualizations and ML tasks


## ML Business Case
* In the previous bullet, you potentially visualized an ML task to answer a business requirement. You should frame the business case using the method we covered in the course 


## Dashboard Design

### Page 1: Project Summary

- Project Summary
  - Terms and Jargon
  - Project Database
  - Business Requirements
  
### Page 2:   

* List all dashboard pages and their content, either blocks of information or widgets, like buttons, checkboxes, images, or any other item that your dashboard library supports.
* Later, during the project development, you may revisit your dashboard plan to update a given feature (for example, at the beginning of the project you were confident you would use a given plot to display an insight but subsequently you used another plot type).



## Unfixed Bugs
* You will need to mention unfixed bugs and why they were not fixed. This section should include shortcomings of the frameworks or technologies used. Although time can be a significant variable to consider, paucity of time and difficulty understanding implementation is not a valid reason to leave bugs unfixed.

## Deployment
### Heroku

* The App live link is: https://YOUR_APP_NAME.herokuapp.com/ 
* Set the runtime.txt Python version to a [Heroku-24](https://devcenter.heroku.com/articles/python-support#supported-runtimes) stack currently supported version.
* The project was deployed to Heroku using the following steps.

1. Log in to Heroku and create an App
2. At the Deploy tab, select GitHub as the deployment method.
3. Select your repository name and click Search. Once it is found, click Connect.
4. Select the branch you want to deploy, then click Deploy Branch.
5. The deployment process should happen smoothly if all deployment files are fully functional. Click now the button Open App on the top of the page to access your App.
6. If the slug size is too large then add large files not required for the app to the .slugignore file.


## Main Data Analysis and Machine Learning Libraries
* Here you should list the libraries you used in the project and provide an example(s) of how you used these libraries.


## Credits 

* In this section, you need to reference where you got your content, media and extra help from. It is common practice to use code from other repositories and tutorials, however, it is important to be very specific about these sources to avoid plagiarism. 
* You can break the credits section up into Content and Media, depending on what you have included in your project. 

### Content 

- The text for the Home page was taken from Wikipedia Article A
- Instructions on how to implement form validation on the Sign-Up page were taken from [Specific YouTube Tutorial](https://www.youtube.com/)
- The icons in the footer were taken from [Font Awesome](https://fontawesome.com/)

### Media

- The photos used on the home and sign-up page are from This Open-Source site
- The images used for the gallery page were taken from this other open-source site



## Acknowledgements (optional)
* Thank the people who provided support through this project.

