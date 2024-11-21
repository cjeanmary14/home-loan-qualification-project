# Home Loan Qualifiacation Project

## Objective:

The company wants to automate the loan eligibility process (real-time) based on customer detail provided while filling out the online application form. These details are Gender, Marital Status, Education, Number of Dependents, Income, Loan Amount, Credit History and others. To automate this process, they have given a problem identifying the customer segments eligible for loan amounts to target these customers specifically.

## About Project

-I plan to make a machine learning algorithm that would determine if a future applicant about be approved for a home loan based on provided existing data.

-This project is not finished yet, but the goal is to automate the home loan application process by giving the applicant information on whether he/she would qualify using the information that was entered by loan applicants.

-In the meantime, I made a report of the applicants and co-applicants that qualify for home loan from each gender. It also provides information on average monthly income, marital status, existing credit, etc.

-With this information, this can give lenders a better idea in whom they going to lend loans to.

## Data Preparing Process:

-I mainly used python in a Jupyter Notebook file to analyze, clean, and transform the data in order to make the visualization report.

-I then used another Jupyter Notebook to make predictions with the cleaned data set. 

[Click Here](https://github.com/cjeanmary14/home-loan-qualification-project-data-preparation/tree/main) for viewing the preparation and existing cleaned data set.

-Here is where I took the data data and did some data cleaning to help best what I would like to convey when conveying data. This involved, alternating data types, filling in null values for "gender" field, changing the values in "credit history" field, and some exploration.

[Click Here](https://github.com/cjeanmary14/home-loan-qualification-project-data-preparation/blob/main/main.ipynb) to view the Jupyter Notebook for cleaning.

-Next, here is where I did the prediction modeling for the newly submitted applications. What I used to make the predictions was using a Decision Tree Classifier for Sci-Kit Learn, and want to predict the loan status for the new applications. I turned all the values in all the other fields into dummy variables, and turn the boolean data types of the values into float data types. This would make it easier for the model to read and learn. And it's great becasue I want the model to consider all fields when making the prediction so that the user can put in their credentials while using the app.

-After creating the model, I then try to avoid any possibilities over over/underfitting by pruning the tree a little bit.

-To view the code in the preditions Jupyter Notebook, [Check it Out](https://github.com/cjeanmary14/home-loan-qualification-project-data-preparation/blob/main/Home_Loan_Prediction_Notebook.ipynb) here.

## Home Loan Qualification Analytics

### Click "Dashboard" to view interactive dashboard

[Dashboard](https://public.tableau.com/app/profile/chadwick.jeanmary/viz/HomeLoanData_17203883842580/Dashboard1)

![image](https://github.com/user-attachments/assets/ab3c32cd-8396-4941-bdf6-1c386b78379d)

-The data shows the average monthly income for both the applicant and the co-applicant alongside with the overall monthly incomes for each loan application (individual), agian for both applicant and co-applicant. And that accounts for all genders and all monthly loan terms.

-On the bottom, is the data for Marriage, Credit History, and Number of Dependants.

-The dashboard can easily be filtered. 

-It shows that the co-applicant is always making much less on average than the applicant applying for the loan. This could also signify that most of the applicants didn't need a co-applicant to be qualified for a loan as income would just populate to $0.00, but some of them do which explains why co-applicant income have varying numbers.

-It seems that most of the people who are qualified are already married, have existing credit, and most of them didn't need any dependents but some did. And it is the same result for eceryone possible alteration no matter how it can be filtered.

## Home Loan Qualification Analytics (Cont'd)

### Click "Dashboard" to view interactive dashboard

[Dashboard](https://public.tableau.com/app/profile/chadwick.jeanmary/viz/HomeLoanData_17203883842580/Dashboard2)

![image](https://github.com/user-attachments/assets/385be264-c52d-4345-9a90-322428d86583)

-This is all data of people who qualified for a home loan.

-We want to set a benchmark or a minimum of how much the applicants should be making.

-This can help come up with a particular range in which it will tell us the minimum monthly income an applicant must have in order to qualify for a loan.

-A good view of minimum monthly income is displayed on the top per gender because the minimum monthly income on the whisker chart may not be visiable at first glance.

-It is also set by each loan amount per month.

-What was found interesting was that females seem to mostly likely have a co-applicant to apply when males do not nessiarily need to. And they seem to qualify by earn more just on a minimal scale.

And of course, the whisker charts show applicants making more money, but we want to focus more on the minimum monthly income earned to set a benchmark for qualification.



