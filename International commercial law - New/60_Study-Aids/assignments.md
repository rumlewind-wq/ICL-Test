---
title: "assignments"
topic: "assignments"
type: concept
related: []
tags: []
---

### Computer Exercises

#### C1

Use the data in **WAGE1** for this exercise.  
(i) Estimate the equation  
$$  
wage = \beta_0 + \beta_1 educ + \beta_2 exper + \beta_3 tenure + u  
$$  
Save the residuals and plot a histogram.

(ii) Repeat part (i), but with $\log(wage)$ as the dependent variable.

(iii) Would you say that Assumption MLR.6 is closer to being satisfied for the level-level model or the log-level model?

---

#### C2

Use the data in **GPA2** for this exercise.  
(i) Using all 4,137 observations, estimate the equation  
$$  
colgpa = \beta_0 + \beta_1 hsperc + \beta_2 sat + u  
$$  
and report the results in standard form.

(ii) Reestimate the equation in part (i), using the first 2,070 observations.

(iii) Find the ratio of the standard errors on **hsperc** from parts (i) and (ii). Compare this with the result from (5.10).

---

#### C3

In equation (4.42) of Chapter 4, using the data set **BWGHT**, compute the **LM statistic** for testing whether **motheduc** and **fatheduc** are jointly significant. In obtaining the residuals for the restricted model, be sure that the restricted model is estimated using only those observations for which all variables in the unrestricted model are available (see Example 4.9).

---

#### C4

Several statistics are commonly used to detect nonnormality in underlying population distributions. Here we will study one that measures the amount of skewness in a distribution. Recall that any normally distributed random variable is symmetric about its mean; therefore, if we standardize a symmetrically distributed random variable, say  
$$  
z = \frac{(y - \mu_y)}{\sigma_y},  
$$  
where $\mu_y = E(y)$ and $\sigma_y = sd(y)$, then $z$ has mean zero, variance one, and $E(z^3) = 0$.  
Given a sample of data ${y_i: i = 1, \ldots, n}$, we can standardize $y_i$ in the sample by using  
$$  
z_i = \frac{(y_i - \hat{\mu}_y)}{\hat{\sigma}_y},  
$$  
where $\hat{\mu}_y$ is the sample mean and $\hat{\sigma}_y$ is the sample standard deviation.  
A sample statistic that measures skewness is  
$$  
n^{-1} \sum_{i=1}^{n} z_i^3,  
$$  
or where $n$ is replaced with $(n - 1)$ as a degrees-of-freedom adjustment.  
If $y$ has a normal distribution in the population, the skewness measure in the sample for the standardized values should not differ significantly from zero.

(i) First use the data set **401KSUBS**, keeping only observations with **fsize = 1**. Find the skewness measure for **inc**. Do the same for **log(inc)**. Which variable has more skewness and therefore seems less likely to be normally distributed?

(ii) Next use **BWGHT2**. Find the skewness measures for **bwght** and **log(bwght)**. What do you conclude?

(iii) Evaluate the following statement: “The logarithmic transformation always makes a positive variable look more nearly normally distributed.”

(iv) If we are interested in the normality assumption in the context of regression, should we be evaluating the unconditional distributions of **y** and **log(y)**? Explain.

---

#### C5

Consider the analysis in Computer Exercise **C11** in Chapter 4 using the data in **HTV**, where **educ** is the dependent variable in a regression.

(i) How many different values are taken on by **educ** in the sample? Does **educ** have a continuous distribution?

(ii) Plot a histogram of **educ** with a normal distribution overlay. Does the distribution of **educ** appear anything close to normal?

(iii)

Which of the CLM assumptions seems clearly violated in the model  
$$  
educ=\beta_0+\beta_1,motheduc+\beta_2,fatheduc+\beta_3,abil+\beta_4,abil^2+u\ ?  
$$  
How does this violation change the statistical inference procedures carried out in Computer Exercise C11 in Chapter 4?

---

#### C6

Use the data in **ECONMATH** to answer this question.  
(i) Logically, what are the smallest and largest values that can be taken on by the variable **score**? What are the smallest and largest values in the sample?  
(ii) Consider the linear model  
$$  
score=\beta_0+\beta_1,colgpa+\beta_2,actmth+\beta_3,acteng+u.  
$$  
Why can Assumption MLR.6 not hold for the error term $u$? What consequences does this have for using the usual $t$ statistic to test $H_0!:\ \beta_3=0$?  
(iii) Estimate the model from part (ii) and obtain the $t$ statistic and associated $p$-value for testing $H_0!:\ \beta_3=0$. How would you defend your findings to someone who states: “You cannot trust that $p$-value because clearly the error term in the equation cannot have a normal distribution.”

---

#### C7

Use the data in **APPLE** to answer the following questions.  
(i) Estimate the following equation by OLS, and report the results in the usual format, including standard errors, sample size, and $R^2$:  
$$  
ecolbs=\beta_0+\beta_1,ecoprc+\beta_2,regprc+\beta_3,faminc+\beta_4,age+\beta_5,educ+u.  
$$  
Are any of the coefficients on **faminc**, **age**, and **educ** individually statistically significant? Do any seem practically large?  
(ii) Obtain the $F$ statistic for joint significance of **faminc**, **age**, and **educ**; report its value and the associated $p$-value, to three decimal places. What do you conclude?  
(iii) Estimate the equation without **faminc**, **age**, and **educ**. Obtain the residuals, $\hat u$. If you regress these residuals on **ecoprc** and **regprc**, what is the $R^2$, and why?  
(iv) Using the residuals from part (iii), obtain the **LM statistic** for joint significance of **faminc**, **age**, and **educ**. Report the statistic to three decimal places, and the associated $p$-value. How similar is your conclusion to the one from the $F$ test?

---