## Stat Lecture
### Std. deviation calculation:
To calculate the standard deviation (SD) of a dataset, such as the one you've provided (x = [1, 2, 3, 4, 5]), you can follow these steps:

1. **Calculate the Mean (Average):** First, find the mean (average) of the dataset. To do this, add up all the numbers in the dataset and then divide by the number of data points. In this case:
    
    Mean (μ) = (1 + 2 + 3 + 4 + 5) / 5 = 15 / 5 = 3
    
2. **Find the Differences from the Mean:** For each data point, subtract the mean from that data point. These are the deviations from the mean. Then square each of these differences.
    
    Deviations from the mean: (1 - 3) = -2 (2 - 3) = -1 (3 - 3) = 0 (4 - 3) = 1 (5 - 3) = 2
    
3. **Calculate the Variance:** Calculate the variance by finding the average of the squared differences you calculated in the previous step.
    
    Variance (σ^2) = [( (-2)^2 + (-1)^2 + (0)^2 + (1)^2 + (2)^2 )] / 5 = (4 + 1 + 0 + 1 + 4) / 5 = 10 / 5 = 2
    
4. **Find the Standard Deviation:** Finally, to get the standard deviation, take the square root of the variance.
    
    Standard Deviation (σ) = √(Variance) = √(2) ≈ 1.414
    

So, the standard deviation of the dataset x = [1, 2, 3, 4, 5] is approximately 1.414.


### Bayesian vs. frequentist example :
Certainly! Let's use a simple example to explain the difference between frequentist and Bayesian probabilities.

**Frequentist Probability:** Imagine you have a regular six-sided die, and you want to find the probability of rolling a 6 (i.e., getting a 6 on a single roll). In frequentist probability:

- You would roll the die a large number of times, let's say 1,000 times.
- You count how many times you get a 6, let's say it comes up 150 times.
- The frequentist probability of rolling a 6 is calculated as the number of times you rolled a 6 (150) divided by the total number of rolls (1,000), which is 150/1,000 = 0.15 or 15%.

So, in frequentist probability, you estimate the probability based on the long-term relative frequency of the event (rolling a 6 in this case) occurring over many trials.

**Bayesian Probability:** Now, let's consider the Bayesian approach. In this case:

- You start with an initial belief or prior probability, which could be based on some information or your own judgment. Let's say you start with a prior probability of 10% (0.10) for rolling a 6.
    
- You roll the die once and observe the outcome, which is a 6.
    
- After this observation, you update your probability based on the new evidence. This updated probability is called the posterior probability.
    

To calculate the posterior probability, you use Bayes' Theorem, which takes into account both your prior belief and the new evidence. For simplicity, let's say Bayes' Theorem updates your probability to 80% (0.80) for rolling a 6 after observing it once.

#### Bayesian example :
**Scenario:**

Imagine you are taking a medical test for a rare disease, and the test result is positive. You're concerned about the accuracy of the test and want to estimate the probability that you actually have the disease, given the positive test result.

Here are the key pieces of information:

1. **Prior Probability (Your Belief):** Before taking the test, you estimate that there's a 1% chance you have the disease. This is your initial belief or prior probability, denoted as P(Disease) = 0.01.
    
2. **Test Accuracy:** The test is known to have some rate of false positives. In this case, the test has a 5% false positive rate, meaning that 5% of the time, it gives a positive result for people who do not have the disease. This is the probability of a positive test result when you are healthy, denoted as P(Positive | No Disease) = 0.05.
    
3. **Disease Prevalence:** The disease is quite rare, with a prevalence of 0.1% in the population. This is the overall rate at which people have the disease, denoted as P(Disease) in the population = 0.001.
    

**Bayesian Calculation:**

Now, using Bayesian statistics, you can update your probability of having the disease after getting a positive test result.

1. **Calculate the Probability of a Positive Test Result When You Have the Disease:** You already know that the test has a 5% false positive rate. So, the probability of a positive test result when you actually have the disease (true positive rate) is 95% or 0.95, because it's complementary to the false positive rate.
    
2. **Apply Bayes' Theorem:** Use Bayes' Theorem to update your probability of having the disease:
    
    P(Disease | Positive Test) = [P(Positive Test | Disease) * P(Disease)] / P(Positive Test)
    
    - P(Positive Test | Disease) = 0.95 (true positive rate)
    - P(Disease) = 0.01 (your prior belief)
    - P(Positive Test) is the overall probability of getting a positive test result, which can be calculated as follows:
    
    P(Positive Test) = [P(Positive Test | Disease) * P(Disease)] + [P(Positive Test | No Disease) * P(No Disease)]
    
    - P(Positive Test | No Disease) = 0.05 (false positive rate)
    - P(No Disease) is the complementary probability of having the disease, calculated as 1 - P(Disease) = 0.999.
    
    Now, plug in the values:
    
    P(Positive Test) = [0.95 * 0.01] + [0.05 * 0.999]
    
3. **Calculate P(Disease | Positive Test):** With these values, you can calculate P(Disease | Positive Test) using Bayes' Theorem. This will give you the updated probability of having the disease given the positive test result.
    

By performing this calculation, you can estimate the probability of having the disease after considering the positive test result and your prior belief. Bayesian statistics allow you to incorporate prior knowledge and update probabilities as new information becomes available.

---

----

## Linking the jargon :

**Slide 1: Introduction**

- Brief overview of the importance of probability and statistics in decision-making and data analysis.

**Slide 2: Probability Basics**

- Introduce the concept of probability.
- Discuss the three probability axioms: non-negativity, additivity, and total probability.
- Explain how these axioms form the foundation of probability theory.

**Slide 3: Discrete and Continuous Probability**

- Differentiate between discrete and continuous probability.
- Provide examples of discrete and continuous random variables.
- Explain the key differences in how we analyze and model them.

**Slide 4: Probability Functions**

- Define probability functions as mathematical tools to model random variables.
- Discuss how probability mass functions (PMFs) are used for discrete variables.
- Introduce probability density functions (PDFs) for continuous variables.
   _Probability functions are mathematical tools used to model random variables._

- **Definition:** Probability functions are mathematical functions that describe the probability distribution of random variables. They allow us to quantify the likelihood of different outcomes.
    
- **Purpose:** Probability functions are fundamental in probability theory and statistics. They help us make sense of uncertainty and randomness, whether in discrete or continuous scenarios.
    
- **Types:** Two common types of probability functions are Probability Mass Functions (PMFs) and Probability Density Functions (PDFs). The choice between these functions depends on whether the random variable is discrete or continuous.

**Slide 5: Probability Mass Function (PMF)**

- Define and explain PMF.
- Provide examples of using PMFs to describe probabilities of discrete outcomes.
- Discuss properties of PMFs, such as normalization.
   _Probability Mass Functions describe probabilities of discrete outcomes._

- **Definition:** A Probability Mass Function (PMF) is a function that assigns probabilities to each possible discrete outcome of a random variable. It summarizes the probability distribution for discrete variables.
    
- **Example:** Consider a six-sided die. The PMF would specify the probabilities of rolling each number: P(1), P(2), P(3), P(4), P(5), and P(6).
    
- **Properties:** PMFs have certain properties, including non-negativity (all probabilities are non-negative), and the sum of all probabilities equals 1 (they are normalized).

**Slide 6: Probability Density Function (PDF)**

- Define and explain PDF.
- Provide examples of using PDFs to describe probabilities of continuous outcomes.
- Discuss properties of PDFs, including area under the curve.
   _Probability Density Functions describe probabilities of continuous outcomes._

- **Definition:** A Probability Density Function (PDF) is a function used for modeling continuous random variables. It characterizes the probability distribution over a range of values rather than specific outcomes.
    
- **Example:** The PDF of a continuous variable, such as the height of adults, describes the likelihood of observing various heights within a given range.
    
- **Properties:** PDFs are characterized by their shape, and the area under the curve represents the probability of observing values within a certain range. Unlike PMFs, PDFs do not assign probabilities to individual values, but rather to intervals.
    
- **Normalization:** The integral (area under the curve) of a PDF over its entire range equals 1, ensuring that the total probability is conserved.
    
- **Smoothing:** PDFs are often smoothed with a continuous curve for easier analysis and integration.

**Slide 7: Probability Statistics and Parameters**

- Introduce common probability statistics and parameters.
- Discuss the concept of the mean (expected value) and its importance.
- Explain the standard deviation as a measure of data dispersion.
- Mention "5 sigma" and its relevance in statistics and hypothesis testing.

**Slide 8: Mean and Standard Deviation**

- Go into greater detail about calculating the mean and standard deviation.
- Explain the significance of these statistics in data analysis and modeling.

**Slide 9: Hypothesis Building and Testing**

- Transition to the topic of hypothesis testing.
- Explain the importance of hypothesis testing in scientific research and decision-making.
- Discuss how probability and statistics are essential for hypothesis testing.

**Slide 10: Hypothesis Testing Process**

- Walk through the steps of hypothesis testing: formulating hypotheses, collecting data, performing statistical tests, and drawing conclusions.
- Emphasize the role of probability distributions in hypothesis testing.

**Slide 11: Conclusion**

- Summarize the key points covered in the lecture.
- Highlight the interconnectedness of probability, statistics, and hypothesis testing in making informed decisions.
- Encourage further exploration of these topics in data analysis and scientific research.

----

