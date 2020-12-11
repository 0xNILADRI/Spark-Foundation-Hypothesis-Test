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
2. Standard Deviation , s<sub>x</sub><sup>2</sup>, s<sub>y</sub><sup>2</sup>
3. Pooled Variance

   Formula : $$s_{p}^2 = \frac {(n_{x} - 1)s_{x}^2 + (n_{y} - 1)s_{y}^2}{n_{x} + n_{y} - 2}$$

4. Standard Error 

    Formula : $$std. err = \sqrt { \frac { s_{p}^2 }{n_{x}} + \frac { s_{p}^2 }{n_{y}}}$$

5. Degree of freedom 

    Formula : $$df = n_{x} + n_{y} -2$$

6. T Statistic Value 

    Formula : $$T = \frac {\bar d - \mu_{o}}{std.err} $$

7. Calculate P Value

    * Refer T Table for P value significance.

__We choose significance value of 0.05, 95%. α = 0.05__

</br>


__*Thumb Rule*__

1. If T score greater than 2, or lower than -2 we can easily reject the null Hypothesis.
2. P value lower than 0.0000 is extreamly significant, although we consider only upto 3.
    
</br>

__Questions and Hypothesis.__

For each case we consider 2 tail test, because of our hypothesis.

__Q1.__ Is there any gender wage gap in the organisation ?

$$H_{0}  :  \mu_{male} - \mu_{female} = 0 \space , \space no \space gender \space gap$$
$$H_{1}  :  \mu_{male} - \mu_{female} \neq 0 \space , \space gender \space gap \space present$$


__Q2.__ Is the company discriminating on the basis of race/ethnicity (white vs else) ?

$$H_{0}  :  \mu_{white} - \mu_{non-white} = 0 \space , \space no \space racial \space gap$$
$$H_{1}  :  \mu_{white} - \mu_{non-white} \neq 0 \space , \space racial \space gap \space present$$


__Q3.__ Is there racial discrimination for the employees above the age of 35 ?

$$H_{0}  :  \mu_{white-above35} - \mu_{non-white-above35} = 0 \space , \space no \space racial \space gap$$
$$H_{1}  :  \mu_{white-above35} - \mu_{non-white-above35} \neq 0 \space , \space racial \space gap \space present$$

__Q5.__ Is there gender discrimination for the employees above the age of 35 ?

$$H_{0}  :  \mu_{male-above35} - \mu_{female-above35} = 0 \space , \space no \space racial \space gap$$
$$H_{1}  :  \mu_{male-above35} - \mu_{female-above35} \neq 0 \space , \space racial \space gap \space present$$

__Q6.__ Are the top 50 longest working employees facing gender discrimination ?

$$H_{0}  :  \mu_{male-top50} - \mu_{female-top50} = 0 \space , \space no \space gender \space gap$$
$$H_{1}  :  \mu_{male-top50} - \mu_{female-top50} \neq 0 \space , \space gender \space gap \space present$$

__Q7.__ Are the top 50 longest working employees facing racial discrimination ?

$$H_{0}  :  \mu_{white-top50} - \mu_{non-white-top50} = 0 \space , \space no \space racial \space gap$$
$$H_{1}  :  \mu_{white-top50} - \mu_{non-white-top50} \neq 0 \space , \space racial \space gap \space present$$

__Q8.__ We should check for each department is there gender discrimination ?

$$H_{0}  :  \mu_{male-department} - \mu_{female-department} = 0 \space , \space no \space gender \space gap$$
$$H_{1}  :  \mu_{male-department} - \mu_{female-department} \neq 0 \space , \space gender \space gap \space present$$

__Q9.__ We should check for each department is there racial discrimination ?

$$H_{0}  :  \mu_{white-department} - \mu_{non-white-department} = 0 \space , \space no \space racial \space gap$$
$$H_{1}  :  \mu_{white-department} - \mu_{non-white-department} \neq 0 \space , \space racial \space gap \space present$$
