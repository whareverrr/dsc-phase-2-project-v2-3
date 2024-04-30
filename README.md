# Phase 2 Project Description

## UrbanCraft Development company : Enhancing Renovation and Construction Services in Real Estate

GROUP 2 MEMBERS:

- ***Alvin Kimathi***
- ***Lynn Oloo***
- ***Hawkins Murithi***
- ***Firdosa Mohamed***

## PROJECT OVERVIEW

UrbanCraft Development company in King County specializes in renovating and constructing residential properties, offering services such as renovation , remodelling and new construction. 
They cater to homeowners, real estate investors, and property developers seeking to enhance the value and appeal of their properties.
According to the regression models in our project we take a keen look at the key factors influencing property prices and that will help increase the estimated value of the houses and by how much 

## BUSINESS UNDERSTANDING

#### Stakeholders in this project include:

- UrbanCraft Development Company: They are directly involved in renovating and constructing residential properties. They look at key factors influencing property prices to enhance their services and increase the value of the houses they work on.

- Homeowners of King County: Homeowners are interested in maximizing the value of their properties. They rely on UrbanCraft to provide renovation and construction services that will increase the value and appeal of their homes.

- Real Estate Investors: Investors in real estate are interested in properties that offer good returns on investment.
  
#### Business Problem

UrbanCraft Development is a start-up renovation and construction company operating in King County, Washington. 
With a focus on enhancing property value and meeting the diverse needs of clients, UrbanCraft aims to leverage market insights, innovation, and sustainable practices to deliver exceptional results in the dynamic real estate landscape of King County.

#### Business Objectives

- Customer Satisfaction: Tailor renovation and construction services based on regression model findings to meet customer preferences, expectations, and budget constraints, ensuring high levels of satisfaction.

- Enhance Property Value: Utilize insights from linear regression models to identify key factors influencing property prices, informing renovation and construction projects aimed at maximizing property value.

- Brand Differentiation: Utilize regression model findings to establish UrbanCraft as a reputable provider of renovation and construction services known for innovation, quality craftsmanship, and superior customer service.

#### Business Questions

- How do bedrooms, bathrooms, square footage, waterfront views, and other property features impact the value of residential properties?

- How does the condition of a property, including its age, renovation history, and overall quality, affect its market value?

- What role does the grade or quality rating of a property play in determining its selling price, and how can we leverage this information to enhance our construction and renovation services?

## DATA UNDERSTANDING

#### King County House CSV Dataset

- The dataset contains 21,597 entries and 20 columns.

- Some columns have missing values, such as "waterfront", "view", and "yr_renovated".

- The data types include integers, floats, and objects (likely representing categorical variables).


#### Column Names Dataset

- The provided dataset consists of a single column named "Text" with 26 entries.

- Each entry is of type object (likely representing strings or text data).

- There are no missing values in the dataset.

- It is  a small dataset containing textual data, representing descriptions of the columns in the kc house dataset.

## DATA ANALYSIS

- The data analysis process began with cleaning the dataset, where errors, duplicates, and missing values are addressed to ensure data integrity.
 
- Preprocessing follows, involving the transformation of categorical features into numerical format.
 
- Subsequently, exploratory data analysis (EDA) is conducted to gain insights into the dataset's characteristics through visualizations and statistical measures.
 
- Moving on to modeling, a simple linear regression model is employed to predict the target variable(price) using one predictor (sqft of living room).
 
- Finally, a multiple linear regression model is built by incorporating multiple predictors to enhance predictive accuracy, with the significance of each predictor assessed alongside the overall model fit using statistical tests and metrics. 

## RECOMMENDATION

![image](https://raw.githubusercontent.com/learn-co-curriculum/dsc-phase-2-project-v2-3/main/halfway-there.gif)

![image](https://raw.githubusercontent.com/learn-co-curriculum/dsc-phase-2-project-v2-3/main/halfway-there.gif)

1. **Constant (Intercept)**:
   - Coefficient: 6.464e+06
   - Interpretation: This is the baseline price when all independent variables are zero.
   - Impact: It represents the estimated price of a property with zero bedrooms, zero bathrooms, zero square feet of living space, etc.

2. **Bedrooms**:
   - Coefficient: -1.571e+04
   - Interpretation: For each additional bedroom, the price decreases by $15,710.
   - Impact: More bedrooms might indicate larger properties, but too many bedrooms without corresponding features might lower the price.

3. **Bathrooms**:
   - Coefficient: 3.156e+04
   - Interpretation: For each additional bathroom, the price increases by $31,560.
   - Impact: Bathrooms are often considered a luxury feature, so more bathrooms generally lead to higher prices.

4. **Square Feet of Living Space (sqft_living)**:
   - Coefficient: 103.9754
   - Interpretation: For each additional square foot of living space, the price increases by $103.98.
   - Impact: Larger living spaces typically command higher prices.

5. **Square Feet of Lot (sqft_lot)**:
   - Coefficient: -0.0712
   - Interpretation: For each additional square foot of lot size, the price decreases by $0.07.
   - Impact: Larger lots might be desirable for some buyers, but if not properly utilized, they might not contribute significantly to price.

6. **Floors**:
   - Coefficient: 3.384e+04
   - Interpretation: Each additional floor increases the price by $33,840.
   - Impact: Multiple floors might indicate more living space and can increase the price.

7. **Waterfront**:
   - Coefficient: 1.289e+05
   - Interpretation: Having a waterfront view increases the price by $128,900.
   - Impact: Waterfront properties are often highly desirable and command premium prices.

8. **Year Built (yr_built)**:
   - Coefficient: -2987.4915
   - Interpretation: Each year of age decreases the price by $2,987.49.
   - Impact: Older properties may have lower prices due to potential maintenance issues or outdated features.

9. **Year Renovated (yr_renovated)**:
   - Coefficient: 3.6783
   - Interpretation: Each year since renovation increases the price by $3.68.
   - Impact: Renovated properties typically command higher prices due to updated features and aesthetics.

10. **Grade Categories** (e.g., grade_11Excellent, grade_12Luxury, etc.):
    - Coefficients: Vary based on the grade category.
    - Interpretation: Each grade category represents a different level of property quality, with higher grades indicating better quality and higher prices.
    - Impact: Properties with higher grade categories command higher prices due to superior features and construction quality.

11. **View Categories** (e.g., view_EXCELLENT, view_FAIR, etc.):
    - Coefficients: Vary based on the view category.
    - Interpretation: Each view category represents a different level of view quality, with better views generally associated with higher prices.
    - Impact: Properties with better views command higher prices due to the premium associated with scenic views.

Overall, this regression model provides insights into how various features of a property influence its price, allowing for better understanding and prediction in the real estate market.

**Interpretation**:
- Model 4, with the lowest RMSE, outperforms the other models in predicting property values. This indicates that the features included in Model 4, such as square footage of living space, square footage of the lot, waterfront status, number of floors, year built, year renovated, bedrooms, bathrooms, grade, and view, collectively provide the most effective predictors for property values.
  
- Therefore, Model 4 is the most suitable among the four models for predicting property values based on the given features, as it demonstrates the highest level of predictive accuracy.
Based on the analysis conducted using Model 4, we recommend focusing on specific features to enhance property value through renovation and construction efforts:



