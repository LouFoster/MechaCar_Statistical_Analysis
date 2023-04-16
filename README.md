# MechaCar_Statistical_Analysis

Module 16 Notes

Before You Start
Create a new GitHub repository, "MechaCar_Statistical_Analysis," and initialize the repository with a README.

After you’ve completed the technical analysis for each part, provide a short summary of the results in the README.md of the analysis. For the final part, you’ll write up a short description of the study design for additional statistical analysis. In the written summaries, we would like you to think critically about your analysis, not demonstrate proficiency of automotive manufacturing.

## Instructions

##Part 1: Linear Regression to Predict MPG

Follow the instructions below to complete Part 1.

##Technical Analysis
1.	Download the MechaCar_mpg.csv file, and place it in the active directory for your R session.

2.	Create a new RScript in your R source pane, name it MechaCarChallenge.RScript, and save it to your active directory.

3.	Use the library() function to load the dplyr package.

4.	Import and read in the MechaCar_mpg.csv file as a dataframe.

![image](https://user-images.githubusercontent.com/117233641/232278837-d7864176-62f6-41e1-8767-9ef3fc7c0906.png)

![image](https://user-images.githubusercontent.com/117233641/232278944-5f6118c4-0a49-42f0-b9a1-4ee1cf5956c9.png)

5.	Perform linear regression using the lm() function. In the lm() function, pass in all six variables (i.e., columns), and add the dataframe you created in Step 4 as the data parameter.

![image](https://user-images.githubusercontent.com/117233641/232278964-f16b3fe4-2be1-4d93-b08f-88904a8d8aba.png)
 

6.	Using the summary() function, determine the p-value and the r-squared value for the linear regression model.

 ![image](https://user-images.githubusercontent.com/117233641/232278972-e7d0f4b8-a620-4fa1-acea-1fe0b727a95b.png)
 
 ![image](https://user-images.githubusercontent.com/117233641/232278988-e021b4b2-5c7b-4be9-a049-4e13e1b7d1b4.png)
 
 ![image](https://user-images.githubusercontent.com/117233641/232279005-d2db2e63-abed-44a6-a22d-284ee73e487d.png)

7.	Save your MechaCarChallenge.RScript file to your GitHub repository.

##Part 2: Create Visualizations for the Trip Analysis

The MechaCar Suspension_Coil.csv dataset contains the results from multiple production lots. In this dataset, the weight capacities of multiple suspension coils were tested to determine if the manufacturing process is consistent across production lots. Using your knowledge of R, you’ll create a summary statistics table to show:

•	The suspension coil’s PSI continuous variable across all manufacturing lots.

![image](https://user-images.githubusercontent.com/117233641/232279133-38d1e0a4-a4c3-4521-bb51-159ca7839579.png)

•	The following PSI metrics for each lot: mean, median, variance, and standard deviation.

![image](https://user-images.githubusercontent.com/117233641/232279149-70d01236-4c23-4435-804c-29a5aff958d0.png)


##Written Summary

In your README, create a subheading, ## Linear Regression to Predict MPG, and write a short summary using a screenshot of the output from the linear regression, and address the following questions:
•	The linear regression was calculated using R in RStudio.

•	The MechaCar dataset contains a sample size of prototypes measuring the miles per gallon across multiple variables. 

•	Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

    o	A 95% level of confidence was predetermined, meaning the p-value should be compared to alpha = .05 level of significance to verify if statistically significant.
    
    o	The RScript shows serval variables in the data set and after calculations produces the follow tables 

 ![image](https://user-images.githubusercontent.com/117233641/232279054-4d306170-58a9-4a1c-b856-77ca6c82e712.png)

•	Is the slope of the linear model considered to be zero? Why or why not?

    o	Converting from scientific notation, all of the slopes of the variables are shown to be non-zero even though some are close to zero:

•	Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

    o	“NO” for our example vehicle length and ground clearance variables represent non-random amounts of variance as applied to the mpg values.

•	A summary of the linear regression can be displayed to determine the quality of the dataset.

    o	 However, In this distribution the dataset fits in with the normal parameters.

    o	Absolute value of the min and max are comparable |-19.4|~|18.5| and the median -.07 is close to zero.



##Part 2: Create Visualizations for the Trip Analysis

The MechaCar Suspension_Coil.csv dataset contains the results from multiple production lots. In this dataset, the weight capacities of multiple suspension coils were tested to determine if the manufacturing process is consistent across production lots. Using your knowledge of R, you’ll create a summary statistics table to show:
•	The suspension coil’s PSI continuous variable across all manufacturing lots.
 

•	The following PSI metrics for each lot: mean, median, variance, and standard deviation.
 

Then, in the README.md, you’ll briefly detail and interpret the suspension coil summary statistics.
Follow the instructions below to complete Part 2.

Technical Analysis
1.	Download the Suspension_Coil.csv file, and place it in the active directory for your R session.

2.	In your MechaCarChallenge.RScript, import and read in the Suspension_Coil.csv file as a table.

3.	Write an RScript that creates a total_summary dataframe using the summarize() function to get the mean, median, variance, and standard deviation of the suspension coil’s PSI column.


 
Your total_summary dataframe should look like this:

 

##Part 3: T-Tests on Suspension Coils
 



## Study Design: MechaCar vs Competition
Part 4: Design a Study Comparing the MechaCar to the Competition

Follow the instructions below to complete Part 4.
1.	In your README, create a subheading ## Study Design: MechaCar vs Competition

2.	Write a short description of a statistical study that can quantify how the MechaCar performs against the competition. In your study design, think critically about what metrics would be of interest to a consumer: for a few examples, cost, city or highway fuel efficiency, horse power, maintenance cost, or safety rating.

Using a multiple linear regression statistical summary shows how each manufacturer’s data analysis can impact the safety ratings for MechaCar and their competitors.

3.	In your description, address the following questions:

o	What metric or metrics are you going to test?

Most Car Buyers consider a variety of characteristics and vital car metrics that could be of interest to a consumer. This consumer comparison /data analysis could include the following. 

•	cost, 

•	car color, 

•	city fuel efficiency, 

•	highway fuel efficiency, 

•	maintenance cost, and/or 

•	safety rating .


o	What is the null hypothesis or alternative hypothesis?

As per Module 16: “The null hypothesis is that the mean of the safety rating is zero. The alternative hypothesis is that the mean of the safety rating is not zero.”

o	What statistical test would you use to test the hypothesis? And why?

A multiple linear regression statistical summary would show how the variables impact the safety ratings for MechaCar and their competitors.

o	What data is needed to run the statistical test?

A random sample of n > 30 for as we examine data sets from MechaCar as compare to potential competitors, would need to be collected including highway fuel efficiency (start during this Challenge), the safety ratings, , and maintenance cost plus running the data through RStudio.
