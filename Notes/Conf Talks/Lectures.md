# Statistics Lecture [[Statistics]]
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

<mark style="background: #ABF7F7A6;">Talk is neither extensive nor exhaustive....</mark>

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


## Which distribution is relevant where?

Each of the probability distributions mentioned has specific characteristics and is relevant in various real-world scenarios. Here's a general overview of the types of situations where each distribution is often used:

**Bernoulli Distribution:**

- **Relevance:** Binary outcomes with a fixed probability of success.
- **Examples:** Coin flips, pass/fail tests, yes/no questions, presence/absence of an event.

**Binomial Distribution:**

- **Relevance:** Multiple independent Bernoulli trials, counting the number of successes in a fixed number of trials.
- **Examples:** Multiple coin flips, batch quality control, survey responses.

**Gaussian (Normal) Distribution:**

- **Relevance:** Continuous data with a bell-shaped curve, influenced by many factors.
- **Examples:** Human height, measurement errors, IQ scores.

**Poisson Distribution:**

- **Relevance:** Counting the number of rare events occurring within a fixed interval.
- **Examples:** Customer arrivals at a store, accidents at an intersection, typographical errors.

**Uniform Distribution:**

- **Relevance:** Outcomes with equal probability across a fixed range.
- **Examples:** Rolling a fair die, generating random numbers, drawing cards from a well-shuffled deck.

**Exponential Distribution:**

- **Relevance:** Modeling the time between events in a Poisson process (waiting times).
- **Examples:** Time between customer arrivals at a service center, radioactive decay, queue service times.

**Gamma Distribution:**

- **Relevance:** Modeling the sum of waiting times for multiple events (waiting times for multiple Poisson events).
- **Examples:** Waiting times in multi-stage processes, life span of electronic components, rainfall intensity in a storm event.

It's important to note that these distributions are often used as approximations and may be modified or extended in specific cases to better fit the data. Additionally, some situations may require other distributions or more complex models to accurately represent the underlying processes. The choice of distribution depends on the nature of the data and the characteristics of the phenomenon being studied.

### Examples:
**Bernoulli Distribution:**

1. **Coin Flip:** A simple example where the outcome is either success (heads) or failure (tails). It follows a Bernoulli distribution because there are only two possible outcomes, and each has a fixed probability.
2. **Pass/Fail Test:** In a pass/fail test, an individual either passes (success) or fails (failure). The distribution models a binary event.
3. **Click-Through Rate:** In online advertising, the probability of a user clicking an ad (success) or not clicking (failure) can be modeled with a Bernoulli distribution.

**Binomial Distribution:**

1. **Number of Heads in Multiple Coin Flips:** If you flip a coin multiple times and count the number of heads in a series of Bernoulli trials, the distribution of the total heads follows a binomial distribution.
2. **Defective Product Count:** In manufacturing, the number of defective products in a batch can be described using a binomial distribution.
3. **Survey Responses (Yes/No Questions):** If you conduct a survey with yes/no questions, the number of "yes" responses follows a binomial distribution.

**Gaussian (Normal) Distribution:**

1. **Height of Individuals:** Human height tends to follow a normal distribution because it is influenced by many factors, resulting in a bell-shaped curve.
2. **Error in Measurement:** Errors in measurements, such as those in scientific experiments, often follow a normal distribution due to the central limit theorem.
3. **IQ Scores:** Intelligence quotient (IQ) scores in a population exhibit a normal distribution as they result from a combination of many factors.

**Poisson Distribution:**

1. **Arrival of Customers at a Store:** The number of customers arriving at a store within a certain time frame can be modeled using a Poisson distribution.
2. **Accidents at an Intersection:** The number of accidents occurring at an intersection in a day can be described by a Poisson distribution.
3. **Typographical Errors in a Book:** The number of typographical errors on each page of a book may follow a Poisson distribution.

**Uniform Distribution:**

1. **Rolling a Fair Six-Sided Die:** Each outcome (1 to 6) has an equal probability of 1/6, making it a uniform distribution.
2. **Random Number Generation:** When generating random numbers in a specified range, a uniform distribution ensures equal probability for each value.
3. **Selecting a Card from a Well-Shuffled Deck:** Assuming a well-shuffled deck, the probability of drawing any specific card is uniform.

**Exponential Distribution:**

1. **Time Between Arrival of Poisson-distributed Events:** If events occur according to a Poisson process (e.g., customer arrivals), the time between events often follows an exponential distribution.
2. **Radioactive Decay:** The time it takes for a radioactive substance to decay follows an exponential distribution.
3. **Service Time in a Queue:** The time a customer spends waiting in a queue before being served can be modeled using an exponential distribution.

**Gamma Distribution:**

1. **Waiting Time for Multiple Poisson Events:** When multiple Poisson-distributed events occur in succession (e.g., waiting for several customers), the waiting time can be modeled using a gamma distribution.
2. **Life Span of Electronic Components:** The distribution of the life span of electronic components can sometimes be approximated using a gamma distribution.
3. **Rainfall Intensity:** The distribution of rainfall intensity during a storm event can be described by a gamma distribution.
----

## Flow of the talk :
Absolutely! Let's weave a narrative around these topics.

**The Dawn of Probability**: Imagine a time when games of chance, like dice and cards, fascinated the elite and commoners alike. They often wondered: How can one predict the outcomes? This curiosity laid the foundation of what we now understand as probability. It all began as an attempt to understand games, but soon, it was realized that these mathematical principles are ubiquitous.

**The Categorization of Data**: As humans, we naturally attempt to make sense of our world by categorizing and organizing information. In the realm of probability and statistics, this categorization is vital. We deal with massive amounts of data, and unless we categorize or classify them efficiently, we'd be overwhelmed. Categorization helps in answering the questions: What are we studying? How often does a particular event occur?

**How is Probability Calculated?** It's the ratio of the favorable outcomes to the total number of outcomes. Think of rolling a dice: the probability of getting a '3' is 1 out of 6, because there's 1 favorable outcome and 6 possible outcomes.

**Venturing into Functions**: As we gather data, we realize that it can be random. This randomness can be captured by functions, aptly named probability functions. These functions can be **discrete** (think about the number of heads when flipping coins) or **continuous** (like measuring the height of people).

**Diving Deeper with Statistics**: Here, we bring in the heavy hitters like mean, median, variance, and standard deviation. These statistics tell us about the central tendency and spread of data. For instance, the average height (mean) of a group of people might be 5.5 feet, but the spread (standard deviation) tells us how much individual heights vary from this average. 
Lumping up of data. 

**Interdependence and Relationships**: Sometimes, two variables might move together. This movement can be quantified using covariance and correlation. While covariance simply indicates the direction of the linear relationship, correlation measures both direction and strength. 
- *Definitions* :
	- Covariance is a measure that indicates the direction of the linear relationship between two variables. If we have two sets of data, X and Y, covariance gives us insight into how changes in X might be associated with changes in Y.
	- Correlation standardizes the measure of interdependence between two variables and ranges between -1 and 1. It not only captures the direction but also the strength of the linear relationship.

**Understanding Distributions**: Life rarely fits into neat boxes, but certain patterns emerge again and again. Distributions like binomial, poisson, and gaussian encapsulate these patterns. The bell curve of the Gaussian distribution, for instance, is iconic.

**Testing Our Knowledge**: As we base our decisions on data, we need tests to ensure our conclusions are sound. The t-test and chi-square test are methods that help us discern if our observations are genuine or just flukes.

**The Magic of Central Limit Theorem (CLT)**: Why is the Gaussian distribution everywhere? CLT provides the answer. No matter the original distribution of data, as we take more samples and average them, their distribution becomes increasingly Gaussian.

**Measuring with Precision**: Every measurement comes with uncertainty. By understanding error propagation, we can predict how individual measurement uncertainties affect our final result. The topics of covariance and correlation become vital here, showing their intertwined nature with measurement precision.

**Frequentist vs. Bayesian**: These are two philosophies of interpreting probability. The frequentist approach considers probability as long-term frequencies, while the Bayesian view incorporates prior knowledge and updates probabilities based on new evidence.

So, from the toss of a coin to the intricacies of Bayesian statistics, our journey through probability is filled with interconnections and revelations. Each concept builds on the previous, offering a deeper understanding of our world and the randomness that permeates it.

----

## Discrete vs. Continuous : 
Terms are different :
### Discrete - 
Concern is with lumps/masses on histograms. And they should all add up to 1.

### Continuous - 
Concern is with intervals of random variables. The probability is spread out or "smeared" over intervals of outcomes, and this is described by a density.


-----

# SiPM:

## Trigger types 
In the context of Silicon Photomultipliers (SiPMs) like those produced by companies such as Hamamatsu, the terms "internal trigger" and "external trigger" refer to different methods of initiating the readout or data acquisition process in response to detected signals. Understanding the distinction between these two types of triggers is important for designing and implementing effective detection systems.

### Internal Trigger:

1. **Definition**: An internal trigger is generated by the detection system itself, based on the signals it receives. In the case of SiPMs, this usually means that the trigger is generated when the signal from the photodetector crosses a predefined threshold.

2. **Working Mechanism**:
   - When a SiPM detects photons and produces a corresponding electrical signal, the internal circuitry of the system monitors this signal.
   - If the signal amplitude exceeds a certain set level (threshold), the system recognizes this as an event of interest and generates a trigger signal.
   - This trigger then initiates the data acquisition or readout process.

3. **Applications**:
   - Internal triggers are commonly used in applications where the event of interest can be clearly defined by the signal generated by the SiPM itself, such as in certain types of particle detectors or photon counting applications.

### External Trigger:

1. **Definition**: An external trigger is generated by a separate system or device, not by the signal from the SiPM itself. This type of trigger is used to synchronize the SiPM's data acquisition with an external event or process.

2. **Working Mechanism**:
   - An external source, which could be another detector system or a control unit, sends a trigger signal to the SiPM system.
   - The SiPM system then starts its data acquisition or readout process in response to this external trigger, regardless of the signals it might be receiving at that moment.

3. **Applications**:
   - External triggers are useful in complex experiments where synchronization between different systems or stages is crucial. For example, in large-scale physics experiments where multiple detectors need to be synchronized, or in medical imaging techniques like PET scans, where the timing of the detector needs to be synchronized with other imaging components.

### Key Differences:

- **Source of Trigger**: Internal triggers are generated by the signals within the SiPM system, while external triggers come from outside the SiPM system.
- **Control and Synchronization**: Internal triggers are useful for autonomous operation based on signal thresholds, whereas external triggers allow for precise control and synchronization with other systems or processes.

In systems like those developed by Hamamatsu, the choice between internal and external triggering depends on the specific application requirements, including factors like the nature of the signal, the need for synchronization, and the complexity of the overall experimental setup.


## DCR:
A SiPM (Silicon Photomultiplier) experiment typically involves characterizing the performance of the SiPM, and one of the key parameters to measure is the Dark Count Rate (DCR). The DCR is the rate at which the SiPM registers signals (counts) even in the absence of light, primarily due to thermal noise. Understanding the DCR is crucial for applications where low light levels are detected, such as in particle physics or medical imaging.

### How DCR is Calculated:

1. **Data Collection**: The SiPM is operated in a dark environment (no incident photons), and the output is recorded. The output typically consists of discrete pulses corresponding to the detection of photons or thermal noise events.

2. **Threshold Scanning**: To discriminate between actual photon detection events and noise, a threshold is set. Only signals that exceed this threshold are counted. By varying this threshold, you can assess the sensitivity of the SiPM to noise and actual light signals.

3. **Counting Dark Events**: The number of times the output exceeds the threshold in a given time period is counted. These counts are primarily due to thermal noise (since no light is present) and represent the DCR.

4. **Normalization**: The total counts are then normalized to time (e.g., counts per second) to get the DCR.

### Staircase Plot:

A "staircase" plot in this context likely refers to a plot showing how the DCR changes as a function of the threshold level. This plot can resemble a staircase, where each step represents a change in the DCR with different threshold settings. 

- **Higher Thresholds**: At higher thresholds, the DCR typically decreases since fewer noise events are strong enough to exceed the threshold.
- **Lower Thresholds**: At lower thresholds, the DCR increases as more noise events are counted.

### Purpose and Logic:

1. **Noise Characterization**: By scanning across a range of thresholds, you can characterize the noise behavior of the SiPM. This helps in understanding the sensitivity and noise characteristics of the device.

2. **Optimizing Threshold**: For practical applications, it's crucial to set an optimal threshold that minimizes noise while still detecting real photon events. The staircase plot helps in identifying this optimal point.

3. **Device Comparison**: Different SiPMs might have different noise behaviors. The DCR as a function of threshold provides a means to compare different devices or the same device under different operating conditions (like temperature).

In summary, the DCR measurement and the staircase plot are important tools in characterizing and understanding the performance of SiPMs, particularly in terms of their noise behavior and sensitivity. This information is crucial for optimizing SiPM-based systems for various applications.


----


