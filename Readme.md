# Purpose
In this challenge, we will help Jeremy and the data analytics team do the following:

Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes
Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
Run t-tests to determine if the manufacturing lots are statistically different from the mean population
Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.

# Deliverables:
Deliverable 1: Linear Regression to Predict MPG
Deliverable 2: Summary Statistics on Suspension Coils
Deliverable 3: T-Test on Suspension Coils
Deliverable 4: Design a Study Comparing the MechaCar to the Competition

# Input Data used for challenge 

# Files/Data Set used
     MechaCar MPG dataset
     Suspension Coil dataset

# Deliverable 1 Requirements
    
     The MechaCar_mpg.csv file is imported and read into a dataframe. Complete. 
          Refer to: MechaCarChallenge.R
     An RScript is written for a linear regression model to be performed on all six variables. Complete.
          Refer to: MechaCarChallenge.R
     An RScript is written to create the statistical summary of the linear regression model with the intended p-values Complete.
          Refer to: MechaCarChallenge.R
     There is a summary that addresses all three questions
          Refer to code: MechaCarChallenge.R
          Refer to image: Resources\Deliverable1.PNG

# Deliverable 2 
  
# Deliverable 2 Instructions
The MechaCar Suspension_Coil.csv dataset contains the results from multiple production lots. In this dataset, the weight capacities of multiple suspension coils were tested to determine if the manufacturing process is consistent across production lots. Using your knowledge of R, you’ll create a summary statistics table to show:

     The suspension coil’s PSI continuous variable across all manufacturing lots
     The following PSI metrics for each lot: mean, median, variance, and standard deviation.
     Then, in the README.md, you’ll briefly detail and interpret the suspension coil summary statistics.

# Deliverable 2 Requirements
You will earn a perfect score for Deliverable 2 by completing all requirements below:

     The Suspension_Coil.csv file is imported and read into a dataframe
          Refer to code: MechaCarChallenge.R
     An RScript is written to create a total summary dataframe that has the mean, median, variance, and standard deviation of the PSI for all manufacturing lots
          Refer to code: MechaCarChallenge.R
     
     An RScript is written to create a lot summary dataframe that has the mean, median, variance, and standard deviation for each manufacturing lot
          Refer to code: MechaCarChallenge.R
     
     There is a summary that addresses the design specification requirement for all the manufacturing lots and each lot individually
          Refer to code: MechaCarChallenge.R
          Refer to images: 
                    Resources\Deliverable2.PNG
                    Resources\Module_15.PNG

# Technical Analysis
Download the Suspension_Coil.csv file, and place it in the active directory for your R session.

In your MechaCarChallenge.RScript, import and read in the Suspension_Coil.csv file as a table.
Write an RScript that creates a total_summary dataframe using the summarize() function to get the mean, median, variance, and standard deviation of the suspension coil’s PSI column.
Your total_summary dataframe should look like this:

The total summary dataframe showing the mean, median, variance, and standard deviation

Write an RScript that creates a lot_summary dataframe using the group_by() and the summarize() functions to group each manufacturing lot by the mean, median, variance, and standard deviation of the suspension coil’s PSI column.
Your lot_summary dataframe should look like this:

The lot summary dataframe showing the mean, median, variance, and standard deviation for each manufacturing lot



# Written Summary
In your README, create a subheading ## Summary Statistics on Suspension Coils, and write a short summary using screenshots from your total_summary and lot_summary dataframes, and address the following question:

Refer to code: MechaCarChallenge.R
          Refer to images: 
                    Resources\Deliverable2.PNG
                    Resources\Module_15.PNG

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

# Deliverable 3: T-Tests on Suspension Coils

# Deliverable 3 Instructions
     Using your knowledge of R, perform t-tests to determine if all manufacturing lots and each lot individually are statistically different from the population mean of 1,500 pounds per square inch.

# Technical Analysis
     In your MechaCarChallenge.RScript, write an RScript using the t.test() function to determine if the PSI across all manufacturing lots is statistically different from the population mean of 1,500 pounds per square inch.
     
     Next, write three more RScripts in your MechaCarChallenge.RScript using the t.test() function and its subset() argument to determine if the PSI for each manufacturing lot is statistically different from the population mean of 1,500 pounds per square inch.

# Written Summary
     In your README, create a subheading ## T-Tests on Suspension Coils, then briefly summarize your interpretation and findings for the t-test results. Include screenshots of the t-test to support your summary.

     1. Lot 1 sample actually has the **true sample mean of 1500**, again as we saw in the summary statistics above. With a **p-Value of 1**, clearly we cannot reject (i.e. accept) the null hypothesis that there is no statistical difference between the observed sample mean and the presumed population mean (1500).
     
     2. Lot 2 has essentially the same outcome with a **sample mean of 1500.02**, a **p-Value of 0.61**; the null hypothesis cannot be rejected, and the sample mean and the population mean of 1500 are statistically similar.
     
     3. However, Lot 3, not surprisingly is a different scenario. Here **the sample mean is 1496.14** and the **p-Value is 0.04**, which is lower than the common significance level of 0.05.  All indicating to **reject the null hypothesis** that this sample mean and the presumed population mean are not statistically different.

     # Refer to image: MechaCar_Statistical_Analysis\Resources\Module_15.PNG
                       MechaCar_Statistical_Analysis\Resources\Deliverable3.PNG

# Deliverable 3 Requirements 


     An RScript is written for t-test that compares all manufacturing lots against mean PSI of the population
     An RScript is written for three t-tests that compare each manufacturing lot against mean PSI of the population
     There is a summary of the t-test results across all manufacturing lots and for each lot
     Deliverable 4: Design a Study Comparing the MechaCar to the Competition

          Refer to image: Resources\Deliverable3.PNG   
          Refer to code: MechaCarChallenge.R 

# Deliverable 4 Instructions
     Using your knowledge of R, design a statistical study to compare performance of the MechaCar vehicles against performance of vehicles from other manufacturers.


 ## Study Design: MechaCar vs Competition.


# Deliverable 4 Requirements
     Using your knowledge of R, design a statistical study to compare performance of the MechaCar vehicles against performance of vehicles from other manufacturers.

     The statistical study design has the following:
     - A metric to be tested is mentioned
     - A null hypothesis or an alternative hypothesis is described
     - A statistical test is described to test the hypothesis


     This study would involve collecting data on MechaCar and its comparable models across several different manufacturers over the last 3 years.

     * What are the competitions' comparable models, 
     * Which cars will MechaCar be competing with head-to-head? which cars will be included in the study?
     * Which factors will look at the study to determine the relevant to selling price?

# Metrics
Collecting data for comparable models across all major manufacturers for past 3 years for the following metrics:

<<<<<<< HEAD
*  Safety Feature Rating: Independent Variable
*  Current Price (Selling): Dependent Variable
*  Drive Package : Independent Variable
*  Engine (Electric, Hybrid, Gasoline / Conventional): Independent Variable
*  Resale Value: Independent Variable
*  Average Annual Cost of ownership (Maintenance): Independent Variable
*  MPG (Gasoline Efficiency): Independent Variable
=======
*  Safety Feature Rating: **Independent Variable**
*  Current Price (Selling): **Dependent Variable**
*  Drive Package : **Independent Variable**
*  Engine (Electric, Hybrid, Gasoline / Conventional): **Independent Variable**
*  Resale Value: **Independent Variable**
*  Average Annual Cost of ownership (Maintenance): **Independent Variable**
*  MPG (Gasoline Efficiency): **Independent Variable**
>>>>>>> 096d81723c87ca5c6903458dfc76c74d2d598845

# Hypothesis: Null and Alternative
After determining which factors are key for the MechaCar's genre:

<<<<<<< HEAD
  Null Hypothesis (Ho): MechaCar is priced correctly based on its performance of key factors for its genre.
  Alternative Hypothesis (Ha): MechaCar is NOT priced correctly based on performance of key factors for its genre.
 
# Statistical Tests
A multiple linear regression would be used to determine the factors that have the highest correlation/predictability with the list selling price (dependent variable); which combination has the greatest impact on price.
=======
 * Null Hypothesis (Ho): MechaCar is priced correctly based on its performance of key factors for its genre.
 * Alternative Hypothesis (Ha): MechaCar is NOT priced correctly based on performance of key factors for its genre.
 
# Statistical Tests
A **multiple linear regression** would be used to determine the factors that have the highest correlation/predictability with the list selling price (dependent variable); which combination has the greatest impact on price.
>>>>>>> 096d81723c87ca5c6903458dfc76c74d2d598845
