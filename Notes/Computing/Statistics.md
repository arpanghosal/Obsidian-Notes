## Bias
In statistics, bias refers to the tendency of an estimator (a statistical method used to estimate a population parameter) to consistently **overestimate or underestimate the true value** of the parameter it is trying to estimate.

For example, let's say you want to estimate the average height of all people in a certain population, and you take a random sample of 100 people to do so. If the average height of your sample is consistently higher or lower than the true average height of the entire population, then your estimator is biased.

>[!info]
If you don't know the true value of the population parameter, then it's not possible to determine the bias of an estimator directly. However, you can still investigate the bias of an estimator by looking at how it performs on simulated or hypothetical data.
For example, you can generate a large number of random samples from a population with a known true value of the parameter being estimated, and use these samples to estimate the parameter with your chosen estimator. You can then compare the average value of the estimator across all these samples to the true value of the parameter, and see if there is a consistent overestimation or underestimation of the true value.
This type of simulation-based approach can give you a sense of the bias of your estimator, even if you don't know the true value of the population parameter in real-world situations. However, it's important to keep in mind that the bias of an estimator may vary depending on the specific characteristics of the population being studied, so this type of investigation is most useful when it's done in conjunction with other methods for assessing estimator performance.


The degree of bias is determined by comparing the average value of the estimator over many samples to the true value of the population parameter being estimated. If the average value of the estimator is consistently higher or lower than the true value, then the estimator is said to be biased.

Bias can be caused by a variety of factors, such as sampling methods, measurement error, or modeling assumptions. It's important to identify and account for bias in statistical analysis to ensure accurate and reliable results.

In the context of statistical estimators, a good estimator should have low variance. This means that the estimates it produces should be consistent and not vary widely from sample to sample. An estimator with high variance, on the other hand, produces estimates that are more unpredictable and less reliable.

In the context of statistical estimators, a good estimator should have low variance. This means that the estimates it produces should be consistent and not vary widely from sample to sample. An estimator with high variance, on the other hand, produces estimates that are more unpredictable and less reliable.

**"However, it's important to note that there is often a trade-off between bias and variance when selecting an estimator. An estimator with low variance may have higher bias, meaning that its estimates consistently deviate from the true value of the population parameter being estimated. Conversely, an estimator with low bias may have higher variance, meaning that its estimates are more variable from sample to sample."**

![[Pasted image 20230402130707.png]]



Roofit and stuffs : 
Roofit is a toolkit used for modeling and fitting data using maximum likelihood estimators. It allows users to define probability density functions (PDFs) to model the data, and provides tools for performing statistical tests, evaluating goodness of fit, and extracting parameter estimates.

RooStats, on the other hand, is a toolkit that builds upon Roofit and provides statistical tools for hypothesis testing, confidence interval construction, and limit setting.

iminuit is a library used for minimizing the value of a function by adjusting the values of its parameters. It provides a Python interface for the popular MINUIT library, which is used extensively in particle physics for fitting data to models.


