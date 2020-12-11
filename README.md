# Spark Foundation Gender Pay Gap

Spark Foundation Inc is a well renounded company. They have over 5000 employees all across the globe. Out of which we managed to accumlate data for 174 people (samle) on a random basis. We have data showing us their name, age, gender, nationality, ethenicity, tenure, department, department, position and annual salary. 

We are going to test if there is a significant difference in their salaries, based on gender. We will use hypothesis test for mean salaries to check for gender discrimination.
We will further analyze is there a race or age discrimination as well.

## Let's begin our Hypothesis Testing.

Before proceeding lets assess the situations. The all of the condition satisfies :
* Unknown Variance, since sample data and assumed to be equal
* dependant samples

Therefor we can perform  Student's T Test. Calculate T value , p value to infer the hypothesis.

__Process :__

1. Calucate n (sample size) for both dataset.
2. Standard Deviation
3. Pooled Variance
4. Standard Error 
5. Degree of freedom 
6. T Statistic Value 
7. Calculate P Value

__We choose significance value of 0.05, 95%. α = 0.05__

</br>


__*Thumb Rule*__

1. If T score greater than 2, or lower than -2 we can easily reject the null Hypothesis.
2. P value lower than 0.0000 is extreamly significant, although we consider only upto 3.
    
</br>

## Questions

For each case we consider 2 tail test, because of our hypothesis.

__Q1.__ Is there any gender wage gap in the organisation ?

__Q2.__ Is the company discriminating on the basis of race/ethnicity (white vs else) ?

__Q3.__ Is there racial discrimination for the employees above the age of 35 ?

__Q4.__ Is there gender discrimination for the employees above the age of 35 ?

__Q5.__ Are the top 50 longest working employees facing gender discrimination ?

__Q6.__ Are the top 50 longest working employees facing racial discrimination ?

__Q7.__ We should check for each position is there gender discrimination ?

__Q8.__ We should check for each position is there racial discrimination ?
