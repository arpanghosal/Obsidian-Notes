Here we will put some ML algorithms as I learn them on the way.

## FFT :
??

## PageRank :
PR(A) = (1-d) + d (PR(T1)/C(T1) + ... + PR(Tn)/C(Tn))
where:

-   PR(A) is the PageRank of page A,
-   PR(Ti) is the PageRank of pages Ti which link to page A,
-   C(Ti) is the number of outbound links on page Ti and;
-   d is a damping factor which can be set between 0 and 1.

A particular page is ranked recursively depending on what other pages link to it.

## Monte Carlo :
This [important algorithm](http://ib.berkeley.edu/labs/slatkin/eriq/classes/guest_lect/mc_lecture_notes.pdf) is used to approximate solutions to numerical problems of unmanageable complexity by mimicking a random process. It relies on repeated random sampling to obtain a result - in effect using randomness to solve problems that might be deterministic in principle.


[[Self Notes]] #selfnotes


## MM algorithm - minorize-maximize
### Mathematical Insight

The MM Algorithm is a method used in optimization that stands for "Majorize-Minimization" or "Minorize-Maximization," depending on the context. It's a powerful technique for solving difficult optimization problems by breaking them down into simpler, solvable steps. Let's explore the mathematical concept behind it and provide an example in Python.

### Mathematical Insight

The MM algorithm is an iterative procedure that simplifies complex optimization problems. The idea is to replace a hard problem by a sequence of easier problems.

1. **Majorization (for minimization problems)**: 
 If you want to minimize a function  $( f(x))$, find a surrogate function $\( g(x | x^{(t)}) \)$ that is easier to minimize and that majorizes $\( f(x) \)$ at the current estimate \( x^{(t)} \). This means \( g(x | x^{(t)}) \geq f(x) \) for all \( x \) and \( g(x^{(t)} | x^{(t)}) = f(x^{(t)}) \). 

2. **Minimization**: Minimize \( g(x | x^{(t)}) \) to get the next estimate \( x^{(t+1)} \).

3. **Iteration**: Repeat the process until convergence.

### Python Example: MM Algorithm for Quadratic Approximation

Let's consider a simple example where we want to find the minimum of a function using the MM algorithm. Suppose we want to minimize the function \( f(x) = x^4 - 4x^2 \).

We'll use a quadratic function to majorize \( f(x) \) at each step.

#### Python Code:

```python
import numpy as np
import matplotlib.pyplot as plt

def f(x):
    return x**4 - 4*x**2

def g(x, x_t):
    # Quadratic majorizer
    return f(x_t) + 2*x_t**3 * (x - x_t) + 6*x_t**2 * (x - x_t)**2

# Initial guess
x_t = 0.5

# Lists to store iterations
x_vals, y_vals = [x_t], [f(x_t)]

# MM algorithm iterations
for _ in range(10):
    # Find the next point by minimizing the majorizer
    x_next = x_t - x_t**3 / (3*x_t**2)
    
    # Update the current point
    x_t = x_next

    # Store values for plotting
    x_vals.append(x_t)
    y_vals.append(f(x_t))

# Plotting
plt.plot(np.linspace(-2, 2, 100), f(np.linspace(-2, 2, 100)), label='f(x)')
plt.scatter(x_vals, y_vals, color='red')
plt.title('MM Algorithm Optimization')
plt.xlabel('x')
plt.ylabel('f(x)')
plt.legend()
plt.show()
```

#### Explanation:

1. **Function Definitions**: `f(x)` is the function we want to minimize, and `g(x, x_t)` is its majorizing quadratic function.

2. **Initialization**: We start with an initial guess for \( x \).

3. **Iterative Process**: In each iteration, we minimize the majorizer to update our estimate of \( x \). The minimization step here is simplified due to the quadratic nature of the majorizer.

4. **Plotting**: The code plots the original function and the points found in each iteration.

This example illustrates the MM algorithm in a simple context. The real power of the MM algorithm lies in its application to more complex problems where direct minimization is challenging. In such cases, the choice of the majorizing function and the minimization step can be more intricate.



----


## Sorting mechanisms:
1. **Bubble Sort**:
    
    - Feature: Simple and easy to implement.
    - Distinctive Feature: Repeatedly steps through the list, compares adjacent elements, and swaps them if they are in the wrong order. It repeats this process until the list is sorted. Bubble Sort is easy to understand but not efficient for large datasets.
2. **Selection Sort**:
    
    - Feature: In-place sorting algorithm.
    - Distinctive Feature: It repeatedly finds the minimum element from the unsorted part of the list and places it at the beginning. Selection Sort has a time complexity of O(n^2) but requires minimal additional memory space.
3. **Insertion Sort**:
    
    - Feature: Efficient for small lists or partially sorted data.
    - Distinctive Feature: It builds the final sorted list one item at a time by iteratively selecting elements and inserting them into the correct position. It is particularly useful for nearly sorted or small datasets.
4. **Merge Sort**:
    
    - Feature: Divide-and-conquer algorithm with stable sorting.
    - Distinctive Feature: It divides the unsorted list into smaller sub-lists, sorts them individually, and then merges them back together. Merge Sort has a time complexity of O(n log n) and is efficient for large datasets.
5. **Quick Sort**:
    
    - Feature: Divide-and-conquer algorithm with in-place sorting.
    - Distinctive Feature: It picks a "pivot" element and partitions the list into two sub-lists, one with elements less than the pivot and the other with elements greater than the pivot. It then recursively applies the same process to the two sub-lists. Quick Sort is widely used and performs well in practice.
6. **Heap Sort**:
    
    - Feature: Efficient for large datasets.
    - Distinctive Feature: It builds a binary heap data structure from the input list and repeatedly extracts the maximum element from the heap to build the sorted list. Heap Sort has a time complexity of O(n log n) and requires no additional memory space.
7. **Radix Sort**:
    
    - Feature: Efficient for sorting integers with fixed size keys.
    - Distinctive Feature: It sorts elements based on their individual digits, starting from the least significant digit to the most significant digit. Radix Sort has linear time complexity for integers with a fixed number of digits.
8. **Counting Sort**:
    
    - Feature: Efficient for sorting small integers with a limited range.
    - Distinctive Feature: It counts the occurrences of each element in the input list and uses this information to place elements in their correct sorted positions. Counting Sort has a time complexity of O(n + k), where k is the range of input elements.

---
### Anomaly Detection:
[[Data Science and ML#Autoencoders - huge for anomaly detections]]
Suppose we want to use an autoencoder for credit card fraud detection. We have a dataset of credit card transactions, where the majority of transactions are legitimate (normal), but a small percentage are fraudulent (anomalies). We want to build an anomaly detection system to flag potentially fraudulent transactions.

1. **Training Phase**:
    
    - We take the dataset of credit card transactions, which includes both normal and fraudulent transactions.
        
    - We split the dataset into two parts: one containing only normal transactions (the majority class) and the other containing both normal and fraudulent transactions.
        
    - We use the part of the dataset containing only normal transactions to train the autoencoder. The autoencoder learns to encode and decode normal transactions accurately. During training, the autoencoder tries to minimize the reconstruction error, which is the difference between the input (normal transaction) and the reconstructed output.
        
    - The learned autoencoder essentially models the normal behavior of credit card transactions.
        
2. **Testing/Inference Phase**:
    
    - Once the autoencoder is trained, we can use it for anomaly detection.
        
    - For each new credit card transaction, we pass it through the trained autoencoder to reconstruct it.
        
    - We then calculate the reconstruction error, which is a measure of how well the autoencoder can reproduce the input. A low reconstruction error suggests that the transaction is similar to what the autoencoder has seen during training (i.e., normal), while a high reconstruction error suggests that the transaction is different from what the autoencoder has learned (i.e., potentially fraudulent).
        
3. **Anomaly Detection**:
    
    - We set a threshold for the reconstruction error. Transactions with reconstruction errors above this threshold are considered anomalies or potential fraud.
        
    - If the reconstruction error for a transaction exceeds the threshold, it is flagged as an anomaly and subjected to further investigation by a fraud analyst or automated system.
        
    - Transactions with low reconstruction errors are assumed to be normal and can be processed without additional scrutiny.
---

## Summary of ML, AI and DL :

- AI is the broad goal of autonomous machine intelligence.
- Machine Learning is a method to achieve that goal by letting machines learn from data.
- Deep Learning is a technique in machine learning that uses deep neural networks to analyze various factors of data.

---


## Backpropagation Algorithm: 
[[Data Science and ML#History and advancements in ML]]
Certainly! Backpropagation is a fundamental algorithm in the field of artificial neural networks, specifically used for training multi-layer feedforward neural networks. It is a supervised learning algorithm that adjusts the network's internal parameters (weights and biases) to minimize the difference between the actual output and the desired output (target) for a given input.

Here's a more detailed explanation of the backpropagation method:

1. **Forward Pass:**
   - Backpropagation begins with the forward pass, where input data is fed into the neural network, and calculations are performed layer by layer to produce an output.
   - Each neuron in a layer calculates a weighted sum of its inputs, applies an activation function, and passes the result to the next layer.

2. **Calculate Error:**
   - After obtaining the network's output, the algorithm calculates the error or loss, which is a measure of how far the predicted output deviates from the actual target output.
   - Common loss functions include Mean Squared Error (MSE) for regression tasks and Cross-Entropy Loss for classification tasks.

3. **Backward Pass (Backpropagation Proper):**
   - Backpropagation derives its name from this step. It involves propagating the error backward through the network to update the weights and biases.
   - The gradient of the loss with respect to each weight and bias is calculated. This gradient represents how much a small change in the weight or bias would affect the overall error.

4. **Weight and Bias Updates:**
   - The weights and biases of the network are updated using the gradients calculated during the backward pass. The goal is to adjust them in a way that minimizes the loss function.
   - Gradient Descent is commonly used to update the parameters. It involves subtracting a fraction of the gradient from the current weights and biases to move them in the direction that reduces the loss.

5. **Repeat:**
   - Steps 1 to 4 are repeated iteratively for multiple training examples (a process called mini-batch training) or epochs until the model's performance converges to a satisfactory level.

6. **Hyperparameters:**
   - Backpropagation involves several hyperparameters, such as the learning rate (controls the size of weight updates), the choice of activation functions, the network architecture (number of layers and neurons), and regularization techniques to prevent overfitting.

Backpropagation is the cornerstone of training deep neural networks, enabling them to learn complex patterns from data. While it has been highly successful, it's important to note that training deep networks can be computationally intensive and may require significant amounts of data to perform effectively. Additionally, the choice of hyperparameters and network architecture plays a crucial role in the success of the backpropagation algorithm.

----


## Random Generators:
The concept of randomness in computing is quite interesting. Most random number generators in computers are actually "pseudo-random," meaning they generate numbers that appear random, but are actually produced by a deterministic process. True randomness, on the other hand, requires some kind of inherently unpredictable physical process.

### Pseudo-Random Number Generators (PRNGs)

1. **Algorithm-Based**: PRNGs use algorithms to generate a sequence of numbers that only appear random. These are deterministic, meaning if you know the algorithm and its initial state (seed), you can predict all subsequent numbers.

2. **Common Use**: PRNGs are widely used in applications like simulations, games, and basic statistical sampling because they're fast and their "randomness" is sufficient for these purposes.

3. **Limitation**: However, because PRNGs are ultimately predictable, they're not suitable for applications requiring high levels of security, like encryption keys in cryptography.

### True Random Number Generators (TRNGs)

1. **Physical Processes**: True randomness is derived from physical processes that are inherently unpredictable, such as radioactive decay, thermal noise, or atmospheric noise.

2. **Hardware RNGs**: These devices, often called hardware random number generators (HRNGs), generate true random numbers by measuring physical processes. For instance, some HRNGs measure the electrical noise across a resistor.

3. **Security Applications**: HRNGs are used in high-security applications where unpredictability is crucial, such as in generating cryptographic keys, secure tokens, and for high-stakes gambling.

4. **Limitations**: True random number generation can be slower and more resource-intensive than PRNGs. Also, the quality of randomness depends on the physical process and the measurement precision.

### Quantum Random Number Generators

1. **Quantum Physics**: Quantum mechanics, with its inherent unpredictability, provides a basis for generating true random numbers. Quantum random number generators (QRNGs) use quantum phenomena like the superposition of states or quantum tunneling.

2. **Increasing Popularity**: With the advancement of quantum computing and communication, QRNGs are becoming more prominent, especially for cryptographic purposes.

### Software Access to True Randomness

1. **Online Services**: There are online services that provide access to true random numbers generated by physical processes. For example, RANDOM.ORG uses atmospheric noise to generate random numbers.

2. **Combining Approaches**: In some cases, software systems combine both PRNGs and TRNGs to balance speed and unpredictability.

While true randomness requires physical processes, pseudo-random number generators are sufficient for most everyday applications. True random number generators, including those based on quantum phenomena, are reserved for applications where unpredictability is paramount. Advances in quantum technologies may make true random number generation more accessible in the future.

-----

## Bootstrapping

Bootstrapping is a statistical technique used to estimate properties (like the mean, variance, confidence intervals) of a population by sampling with replacement from a data set. It's particularly useful when the theoretical distribution of a statistic is complex or unknown.

### Basic Concept

- **Sampling with Replacement**: From your original data set, you repeatedly take random samples, but after each draw, you put the data point back. This means the same data point can be chosen more than once in each sample.
- **Many Samples**: You create a large number of these "bootstrap samples", typically thousands or more.
- **Calculate Statistics**: For each bootstrap sample, calculate the statistic of interest (e.g., the mean).
- **Estimate Distribution**: By examining the distribution of these bootstrap statistics, you can estimate the properties of the statistic in the population.

### Example: Estimating the Mean

Suppose you have a small data set and you want to estimate the mean and its confidence interval:

Original Data Set: \([4, 7, 10, 15]\)

1. **Create Bootstrap Samples**: Randomly draw numbers from the data set with replacement, making new samples of the same size. For example:
   - Sample 1: \([4, 7, 7, 15]\)
   - Sample 2: \([15, 10, 4, 4]\)
   - … (continue for many samples)

2. **Calculate the Mean of Each Sample**: Compute the mean for each bootstrap sample.
   - Mean of Sample 1: \(8.25\)
   - Mean of Sample 2: \(8.25\)
   - … (calculate for all samples)

3. **Analyze the Bootstrap Means**: After many such samples, you'll have a distribution of means. Analyze this distribution to estimate the mean of the original population and its confidence interval.

### Advantages of Bootstrapping

- **Versatility**: Can be applied to many types of data and statistical measures.
- **Non-Parametric**: Does not assume a specific parametric distribution of the data.
- **Simple and Powerful**: Especially useful for complex data sets where theoretical calculations are difficult or impossible.

### Limitations

- **Not Always Appropriate**: May not work well with extremely small data sets or data with certain types of distributions.
- **Computationally Intensive**: Requires a large number of resampling operations, which can be computationally demanding.


Bootstrapping is widely implemented in various coding practices and computational fields to estimate the statistical properties of a dataset. Its implementation typically involves generating multiple resamples of the original data and then computing the statistic of interest for each resample.

### Implementation in Code

Here’s a simple example of how bootstrapping might be implemented in Python, using a dataset to estimate the mean and its confidence interval:

```python
import numpy as np

# Original dataset
data = np.array([4, 7, 10, 15])

# Number of bootstrap samples
n_bootstrap_samples = 10000

# Array to store means of bootstrap samples
bootstrap_means = np.zeros(n_bootstrap_samples)

# Generate bootstrap samples and compute means
for i in range(n_bootstrap_samples):
    bootstrap_sample = np.random.choice(data, size=data.size, replace=True)
    bootstrap_means[i] = np.mean(bootstrap_sample)

# Compute the 95% confidence interval of the mean
conf_interval = np.percentile(bootstrap_means, [2.5, 97.5])

print(f"Estimated mean: {np.mean(bootstrap_means)}")
print(f"95% confidence interval: {conf_interval}")
```

In this example, we randomly resample the original dataset with replacement 10,000 times, calculate the mean for each resample, and then determine the 95% confidence interval from the distribution of these means.

### Bootstrapping and Central Limit Theorem

Bootstrapping is related to the Central Limit Theorem (CLT) in several ways:

1. **Distribution of Sample Means**: The CLT states that the distribution of the sample means will approximate a normal distribution as the sample size gets larger, regardless of the shape of the population distribution. <mark style="background: #FFB8EBA6;">Bootstrapping takes advantage of this by generating a distribution of sample means (or other statistics) from resamples, which often converge to a normal-like distribution, allowing for the estimation of confidence intervals and other properties.</mark>

2. **Non-Normal Data**: Bootstrapping is particularly useful when the CLT cannot be directly applied, such as with small sample sizes or non-normally distributed data. Because bootstrapping does not rely on the assumption of normality, it can provide robust estimates in cases where traditional parametric methods might fail.

3. **Empirical Distribution**: Bootstrapping essentially uses the empirical distribution of the data (obtained from the resamples) to estimate properties of the population distribution. This can be seen as a practical application of the principles underlying the CLT, extending them to situations where the standard assumptions (like large sample size) do not hold.

In summary, bootstrapping in coding and computational fields involves creating multiple resamples of the original data to estimate statistical properties. While related to the CLT, bootstrapping provides a more flexible and often more robust approach, especially when dealing with complex or limited data.


<details>
<summary>qth percentile </summary>
The qth percentile is a statistical measure that indicates the value below which a given percentage (q) of observations in a group fall. Let's break down how it's calculated and what it means:

### Understanding Percentiles

1. **Percentile Definition**: If you have a value that is at the qth percentile of a dataset, it means that q% of the data is equal to or less than that value.

2. **Example**: If you're at the 50th percentile in terms of height in a group, you are taller than or as tall as 50% of the people in that group.

### How It's Calculated

The calculation of the qth percentile typically involves the following steps:

1. **Sort the Data**: Arrange all the data points in ascending order.

2. **Find the Rank**: Calculate the rank (position in the sorted list) of the qth percentile. This can be done using the formula:

   \[ \text{Rank} = \frac{q}{100} \times (N + 1) \]

   where \( N \) is the number of data points in the dataset, and \( q \) is the percentile you want to find (a number between 0 and 100).

3. **Interpolation**: If the rank is not a whole number, you interpolate between the two nearest data points.

### An Example

Suppose you have a dataset: \([1, 3, 5, 7, 9]\), and you want to find the 20th percentile.

1. The data is already sorted.
2. Calculate the rank: \( \frac{20}{100} \times (5 + 1) = 1.2 \). 
3. The rank is 1.2, which means the 20th percentile is slightly above the 1st value in the dataset. Since the 1st value is 1 and the 2nd value is 3, you interpolate between these values. The 20th percentile would be closer to 1 than to 3.

### Using np.percentile

In your code, `np.percentile` does this computation for you. When you call `np.percentile(bootstrap_means, [2.5, 97.5])`, it calculates the values below which 2.5% and 97.5% of your bootstrap means fall, respectively. This function handles the sorting, ranking, and interpolation steps internally.

### Conclusion
The qth percentile is a way of expressing a position within a sorted dataset relative to the rest of the data. It's particularly useful for understanding the distribution of data and for calculating confidence intervals, as in your bootstrapping example.

</details>

### Conclusion

Bootstrapping is a powerful tool in statistics for estimating the properties of a population from a sample. Its strength lies in its simplicity and versatility, making it applicable to a wide range of situations in data analysis.

---

## Coding practices:

These practices are designed to improve code quality, enhance maintainability, and facilitate collaboration among developers. Here's a rundown of some common and effective coding practices:

### 1. Version Control

- **Purpose**: To manage changes to source code over time and facilitate collaboration among multiple developers.
- **Accomplishment**: Tools like Git allow developers to track revisions, revert to previous states, branch out for new features, and merge changes. It's essential for coordinating work in team environments.

### 2. Code Review

- **Purpose**: To ensure code quality and adherence to coding standards.
- **Accomplishment**: Code reviews involve examining new or changed code by one or more developers other than the author. This practice catches bugs, ensures readability, and promotes knowledge sharing within the team.

### 3. Test-Driven Development (TDD)

- **Purpose**: To ensure code reliability and facilitate refactoring.
- **Accomplishment**: In TDD, developers first write tests for a new feature or functionality and then write code to pass those tests. This leads to more robust and well-tested code.

### 4. Continuous Integration and Continuous Deployment (CI/CD)

- **Purpose**: To automate the integration and deployment of code.
- **Accomplishment**: CI/CD practices involve automatically testing and deploying code changes to ensure that the integration process is seamless and that the deployed software is stable.

### 5. Refactoring

- **Purpose**: To improve the internal structure of code without changing its external behavior.
- **Accomplishment**: Refactoring makes code more readable, maintainable, and efficient. It's a crucial practice for managing technical debt and improving code quality over time.

### 6. Pair Programming

- **Purpose**: To improve code quality and facilitate knowledge transfer.
- **Accomplishment**: Two programmers work together at one workstation. One writes code while the other reviews it in real-time. This practice can lead to fewer bugs and more creative solutions.

### 7. Documentation

- **Purpose**: To provide clear explanations of how the code works and its intended use.
- **Accomplishment**: Good documentation, both within the code (as comments) and external (like user manuals or API documentation), makes software easier to understand, use, and maintain.

### 8. Modular Design

- **Purpose**: To make code more manageable and scalable.
- **Accomplishment**: By dividing software into smaller, independent modules, developers can work on separate parts without affecting others, making the codebase easier to manage and extend.

### 9. Use of Design Patterns

- **Purpose**: To solve common problems in software design.
- **Accomplishment**: Design patterns are proven solutions to common issues. Using them can speed up the development process and make the code more robust and maintainable.

---

## FFT:

### Discrete Fourier Transform (DFT)

The DFT transforms a sequence of complex numbers into another sequence, providing a frequency domain representation of the original sequence.

#### DFT Equation

If you have a sequence $$ x_0, x_1, \ldots, x_{N-1} $$, the DFT is defined by the formula:

$$ X_k = \sum_{n=0}^{N-1} x_n \cdot e^{-\frac{2\pi i}{N}kn} $$

where:
- $$ X_k $$ is the value of the sequence in the frequency domain.
- $$ N $$ is the total number of samples.
- $$ i $$ is the imaginary unit.
- $$ e $$ is Euler's number, and the expression $$ e^{-\frac{2\pi i}{N}kn} $$ represents a complex exponential.

The DFT converts the original sequence (usually in the time domain) into a representation in the frequency domain.

### Fast Fourier Transform (FFT)

The FFT is an efficient way to compute the DFT. The most common form of the FFT is the Cooley-Tukey algorithm, which divides a DFT of any composite size $$ N = N_1 \times N_2 $$ into many smaller DFTs. This significantly reduces the number of computations needed.

#### FFT Efficiency

The direct computation of the DFT using its definition involves $$ O(N^2) $$ complex multiplications, but the FFT reduces this to $$ O(N \log N) $$. This efficiency makes the FFT a powerful tool in digital signal processing.

#### FFT Algorithm (Conceptual Overview)

1. **Decompose**: The FFT algorithm decomposes the original DFT into smaller DFTs, exploiting properties like symmetry and periodicity.

2. **Combine**: The results of these smaller DFTs are combined to produce the final result.

#### Application Example

Consider a time-series data set representing a signal. The FFT can quickly transform this data to its frequency domain representation, allowing you to analyze the frequency components present in the original signal.

### In Summary

The FFT is an algorithm that efficiently computes the DFT, which is a fundamental tool in signal processing for analyzing the frequencies present in a signal. Its ability to transform signals into the frequency domain quickly and efficiently makes it invaluable in many fields, such as audio processing, image analysis, and telecommunications.

### Explaining NumPy's FFT Module

The Fast Fourier Transform (FFT) algorithm implemented in NumPy's FFT module (`numpy.fft`) efficiently computes the Discrete Fourier Transform (DFT) of a sequence. Here's what it fundamentally does:

1. **DFT Basics**: The DFT transforms a sequence of complex numbers (or real numbers, in many practical cases) from the time domain to the frequency domain. It decomposes the signal into its constituent frequencies.

2. **FFT Algorithm**: NumPy's FFT is an efficient implementation of the DFT. The FFT algorithm, as opposed to the naive DFT computation, reduces computational complexity from \(O(N^2)\) to \(O(N\log N)\), where \(N\) is the number of samples in the sequence.

3. **Frequency Bins**: The result of the FFT is a series of complex numbers, each representing the amplitude and phase of a particular frequency component of the original signal. The magnitude of these complex numbers indicates the strength of the corresponding frequency in the signal.

### Enhanced Python Code with Detailed Explanations

```python
import numpy as np
import matplotlib.pyplot as plt

def generate_signal(freq, sampling_rate, duration):
    # Create a time array and a sine wave signal
    t = np.linspace(0, duration, int(sampling_rate * duration), endpoint=False)
    signal = np.sin(2 * np.pi * freq * t)
    return t, signal

def perform_fft(signal, sampling_rate):
    # Apply the FFT on the signal
    fft_signal = np.fft.fft(signal)

    # Calculate the frequencies for each FFT component
    fft_freq = np.fft.fftfreq(len(signal), 1/sampling_rate)

    # Return the complex FFT output and corresponding frequencies
    return fft_signal, fft_freq

# Signal parameters
freq = 5  # Frequency of the sine wave in Hz
sampling_rate = 100  # Samples per second
duration = 2  # Duration of the signal in seconds

# Generate the signal
t, signal = generate_signal(freq, sampling_rate, duration)

# Plot the original signal
plt.figure(figsize=(12, 6))
plt.subplot(2, 1, 1)
plt.plot(t, signal)
plt.title('Original Signal')
plt.xlabel('Time [s]')
plt.ylabel('Amplitude')

# Perform the FFT
fft_signal, fft_freq = perform_fft(signal, sampling_rate)

# Plot the frequency spectrum
# We use np.abs to compute the magnitude of the complex FFT output
plt.subplot(2, 1, 2)
plt.plot(fft_freq, np.abs(fft_signal))
plt.title('Frequency Spectrum')
plt.xlabel('Frequency [Hz]')
plt.ylabel('Magnitude')
plt.tight_layout()
plt.show()
```

#### Additional Code Explanation

1. **Signal Generation**: The `generate_signal` function creates a sine wave with the specified frequency, sampling rate, and duration. It simulates a real-world signal like a sound wave or a radio signal.

2. **Applying FFT**: In `perform_fft`, `np.fft.fft` computes the FFT of the signal. This transformation reveals the frequency components of the original time-domain signal.

3. **Frequency Array**: `np.fft.fftfreq` generates an array of frequencies corresponding to each FFT output component. The `1/sampling_rate` argument calculates the correct time interval between samples.

4. **Plotting**: The script plots both the time-domain signal and its frequency spectrum. The magnitude of the FFT result (computed with `np.abs`) shows how much each frequency contributes to the original signal.


--- 


## Hepstats - modeling

### z-fit:
The basic idea behind zfit is to offer a Python oriented alternative to the very successful RooFit library from the [ROOT](https://root.cern.ch/) data analysis package that can integrate with the other packages that are part if the scientific Python ecosystem. Contrary to the monolithic approach of ROOT/RooFit, the aim of zfit is to be light and flexible enough t o integrate with any state-of-art tools and to allow scalability going to larger datasets.

These core ideas are supported by two basic pillars:

- The skeleton and extension of the code is minimalist, simple and finite: the zfit library is exclusively designed for the purpose of model fitting and sampling with no attempt to extend its functionalities to features such as statistical methods or plotting.
- zfit is designed for optimal parallelisation and scalability by making use of TensorFlow as its backend. The use of TensorFlow provides crucial features in the context of model fitting like taking care of the parallelisation and analytic derivatives.

### bayesian blocks:
https://arxiv.org/pdf/1207.5578.pdf
Bayesian Blocks is a method used primarily in astronomical data analysis for adapting histograms and time series data. It's especially useful for identifying and characterizing structure in datasets that contain time-tagged events, like photon arrivals in astrophysical observations. The method was developed in the context of gamma-ray astronomy but has found applications in other areas of astrophysics and beyond.

#### Key Aspects of Bayesian Blocks:

1. **Adaptive Binning**: Unlike traditional histograms with fixed-width bins, Bayesian Blocks adaptively determines the sizes and positions of bins based on the structure of the data. This adaptability allows it to effectively capture significant features in the data, such as variations in signal rate.

2. **Bayesian Methodology**: The method uses Bayesian statistics to optimize a fitness function over the data, determining the optimal segmentation of the data into blocks (bins). Each block is characterized by a constant value, typically the count rate, over its range.

3. **Change-Point Detection**: Bayesian Blocks is effective at identifying change points (points where the data's statistical properties change) in the data. This makes it particularly useful for detecting transient or variable signals in noisy backgrounds.

4. **Applications in Astronomy**: In astronomy, Bayesian Blocks is used for tasks like analyzing light curves from variable stars, detecting gamma-ray bursts, or identifying other transient astronomical events. The method is effective at handling both irregularly spaced data and varying observational efficiencies.

#### Advantages:

- **Flexibility**: Capable of handling various types of data, including time series, point measurements, and event data.
- **Sensitivity to Features**: Efficiently identifies significant structures in the data, even with background noise.
- **Objective Binning**: Reduces subjectivity in choosing bin sizes for histograms, providing a data-driven approach.

#### Implementation:

Bayesian Blocks can be implemented in Python, often using libraries like `astropy` that provide built-in functionality for this algorithm. The implementation involves computing a fitness function for different potential partitions of the data and choosing the partition that maximizes this function, subject to a Bayesian prior.

#### Limitations:

- **Computational Complexity**: The algorithm can be computationally intensive for very large datasets.
- **Choice of Priors**: The performance of Bayesian Blocks can depend on the choice of Bayesian priors, which may require careful selection based on the nature of the data.

In summary, Bayesian Blocks is a powerful tool for adaptively binning data, particularly in astronomical contexts. Its ability to reveal the intrinsic structure of complex datasets makes it a valuable method in the toolbox of astronomers and data scientists alike.


----

# Gradient Boosting : #bdt 

Boosting algorithms, including gradient boosting, are indeed widely used in machine learning, and their applications extend beyond just boosting decision trees, although that is one of their most common and effective uses.

The core idea behind boosting is to combine multiple weak learners to form a strong learner. A weak learner is a model that is only slightly correlated with the true classification (it's better than random guessing). By combining these weak learners in a specific manner, boosting algorithms can achieve high accuracy in various predictive modeling tasks.

Gradient boosting is a particularly popular boosting technique. It builds the model in stages, and at each stage, it adds a new weak learner to correct the errors made by the previous ensemble of learners. While decision trees are commonly used as the base learners in gradient boosting, the framework itself is more general and can be used with other types of models as well.

The reason decision trees are often used in conjunction with gradient boosting is that they complement each other well. Decision trees are simple and computationally efficient to train, but they tend to overfit the training data. Gradient boosting improves on this by focusing on correcting the mistakes of previous trees, which typically leads to a more robust model that generalizes better to unseen data. See [[Data Science and ML#Boosted Decision Trees (BDTs)]]

Outside of decision trees, gradient boosting can be applied to other types of models, but its effectiveness will depend on the nature of the data and the specific problem. The adaptability of gradient boosting to different kinds of data and its ability to handle various types of predictive modeling tasks—ranging from regression to classification—make it a versatile and powerful tool in the machine learning toolkit.

In practice, gradient boosting, especially with decision trees, is often a go-to method due to its high performance on a wide range of tasks. It's particularly well-regarded for structured, tabular data where relationships between features are complex and non-linear. The success of frameworks like XGBoost, LightGBM, and CatBoost, which implement variations of gradient boosting, further attests to its popularity and effectiveness in both academic and industrial applications.


## Bagging vs. Boosting:
 Bagging and boosting are both ensemble learning techniques that combine multiple models to improve performance.- Bagging focuses on reducing variance by independently training models in parallel on randomly sampled subsets of data. It aims to introduce diversity among models. - The most common bagging algorithm is Random Forest which also randomly selects features for splits. The final prediction averages individual model predictions.- Boosting sequentially trains models to correct errors of previous ones. It assigns weights to instances based on misclassifications to guide following models.- Bagging samples data randomly for each model while boosting iteratively adjusts instance weights based on errors.- Bagging averages predictions while boosting assigns weights based on model performance, giving more influence to better performing models.- Bagging is more robust to noise and outliers due to averaging, while boosting can overfit to noise if weights are adjusted too aggressively.  - Bagging introduces diversity through random sampling and features, while boosting focuses on correcting errors.- Bagging primarily reduces variance, while boosting addresses both bias and variance with an emphasis on reducing bias.- Examples given are Random Forest for bagging and AdaBoost for boosting which sequentially trains weak learners like decision trees.- Bagging works well for unstable models prone to overfitting, while boosting can improve weak learners and handle complex patterns.

----


# Affinity 
Affinity, in a broad sense, refers to a <mark style="background: #FFB8EBA6;">relationship or connection between things, where one influences or has relevance to the other</mark>. In different fields of research such as mathematics, physics, computer science, and beyond, the concept of affinity manifests in various ways, often reflecting the intrinsic connections that underpin these disciplines. Here's how affinity overlaps between some of these fields:

### Mathematics

In mathematics, affinity can refer to an affine transformation, which is a type of linear mapping method that preserves points, straight lines, and planes. Sets of parallel lines remain parallel after an affine transformation. The concept of affine spaces—an extension of the concept of vector spaces—is crucial in fields like geometry and algebra. This mathematical foundation finds applications in numerous other domains, illustrating a deep affinity between abstract mathematical principles and practical applications.
![[Pasted image 20240311105648.png]]
### Physics

In physics, the term affinity has been used in various contexts, including in thermodynamics and chemical kinetics to describe the<mark style="background: #ABF7F7A6;"> force that drives chemical reactions</mark>. For example, in the context of chemical thermodynamics, affinity measures the tendency of a chemical reaction to occur. This concept is closely related to the Gibbs free energy change of a reaction. The mathematical treatment of these concepts shows the overlap between mathematics and physics, especially in how differential equations and linear algebra are used to model physical phenomena.
![[Pasted image 20240311105808.png]]
### Computer Science

Computer science often utilizes mathematical concepts to solve computational problems. Algorithms, data structures, and information theory are just a few areas where the affinity between mathematics and computer science is evident. For instance, affine transformations are widely used in computer graphics for scaling, rotating, and translating images and shapes. Moreover, concepts from physics, such as optimization and systems modeling, are applied in computational simulations, machine learning, and artificial intelligence, showing a rich interplay between these fields.

### Overlapping Affinities

The overlapping affinities between these fields are evident in interdisciplinary areas like computational physics, numerical analysis, and quantum computing. For example:

- **Computational Physics** utilizes algorithms and numerical methods (from mathematics) to solve physical problems, showing the affinity between computational techniques and physical theories.
- **Numerical Analysis**, a field of mathematics, is crucial for developing efficient algorithms to solve problems in science and engineering, demonstrating an affinity between theoretical mathematics and its practical applications in other fields.
- **Quantum Computing** is an area where physics, mathematics, and computer science converge. It leverages quantum mechanics (physics) to perform computations, employing mathematical concepts in algorithm design and computer science principles in hardware and software development.

### Example:

---

The affine transformation \(T\) applied to a point \((x, y)\) in the plane can be represented as:

$$
T(x, y) = A \cdot \begin{pmatrix} x \\ y \end{pmatrix} + \vec{b}
$$

where \(A\) is the rotation and scaling matrix, and \(\vec{b}\) is the translation vector.

In the given code example, the affine transformation involves:

- Scaling by a factor of \(s = 2\),
- Rotation by an angle of \(\theta = 30^\circ\),
- Translation by a vector \(\vec{b} = \begin{pmatrix} 2 \\ 3 \end{pmatrix}\).

The rotation and scaling matrix \(A\) is defined as:

$$
A = s \cdot \begin{pmatrix} \cos(\theta) & -\sin(\theta) \\ \sin(\theta) & \cos(\theta) \end{pmatrix}
$$

Given \(s = 2\) and \(\theta = 30^\circ\), we can substitute these values into the matrix to get:

$$
A = 2 \cdot \begin{pmatrix} \cos(30^\circ) & -\sin(30^\circ) \\ \sin(30^\circ) & \cos(30^\circ) \end{pmatrix}
$$

$$
A = 2 \cdot \begin{pmatrix} \sqrt{3}/2 & -1/2 \\ 1/2 & \sqrt{3}/2 \end{pmatrix}
$$

$$
A = \begin{pmatrix} \sqrt{3} & -1 \\ 1 & \sqrt{3} \end{pmatrix}
$$

So, the final affine transformation formula combining scaling, rotation, and translation is:

$$
T(x, y) = \begin{pmatrix} \sqrt{3} & -1 \\ 1 & \sqrt{3} \end{pmatrix} \cdot \begin{pmatrix} x \\ y \end{pmatrix} + \begin{pmatrix} 2 \\ 3 \end{pmatrix}
$$

This formula represents the mathematical background for the affine transformation applied in the Python code.
From git projects:

![[Pasted image 20240311110752.png]]

---

These examples illustrate how the concept of affinity reflects the interconnectedness of various disciplines, highlighting the importance of cross-disciplinary knowledge and collaboration in advancing our understanding of complex problems.

----

# Activation functions:

https://medium.com/@tariqanwarph/activation-function-and-glu-variants-for-transformer-models-a4fcbe85323f

### Markdown Format with Human-Readable Math Expressions
prompt - "Markdown with LaTeX for mathematical expressions"

### Activation Functions Overview

This document provides a brief overview of some commonly used activation functions in neural networks, including their expressions and pros and cons.

Activation functions are a way to introduce nonlinearity to neural networks. Without this non-linearity, the overall learned function would be linear which cannot account for the complex nonlinear relationships that a neural network needs to learn.

## ReLU (Rectified Linear Unit)

**Expression:**
- $$f(x) = \max(0, x)$$

**Pros:**
- Simple and computationally efficient.
- Helps mitigate the vanishing gradient problem for positive inputs.

**Cons:**
- Gradient can vanish for negative input values, leading to dead neurons.

## GELU (Gaussian Error Linear Unit)

**Expression:**
- $$f(x) = 0.5x\left(1 + \tanh\left(\sqrt{\frac{2}{\pi}}(x + 0.044715x^3)\right)\right)$$

**Pros:**
- Non-linearities introduce flexibility, allowing the network to learn more complex patterns.
- Smooth curve makes it more effective for deeper networks.

**Cons:**
- More computationally expensive than ReLU.

## Swish

**Expression:**
- $$f(x) = x \cdot \text{sigmoid}(x)$$
- Where sigmoid(x) is $$\sigma(x) = \frac{1}{1 + e^{-x}}$$

**Pros:**
- Smooth, non-monotonic function that has been found to outperform ReLU in some deep learning tasks.
- Non-zero gradient everywhere helps mitigate the dying ReLU problem.

**Cons:**
- More complex and computationally expensive than ReLU.

## Sigmoid

**Expression:**
- $$f(x) = \frac{1}{1 + e^{-x}}$$

**Pros:**
- Smooth and differentiable.
- Historically popular for output layers in binary classification problems.

**Cons:**
- Suffers from vanishing gradients for inputs with large magnitude, which can slow down training.
- Outputs are not zero-centered, which can lead to gradient update directions being inconsistent.

## Tanh (Hyperbolic Tangent)

**Expression:**
- $$f(x) = \tanh(x) = \frac{2}{1 + e^{-2x}} - 1$$

**Pros:**
- Zero-centered output, which can lead to more efficient training in some cases.
- Smooth and differentiable.

**Cons:**
- Like the sigmoid, it suffers from vanishing gradients for inputs with large magnitude.

![[Pasted image 20240311155242.png]]
## Impact:
While activation functions like ReLU, GELU, Swish, Sigmoid, and Tanh may seem similar at a glance, especially in their graphical representations, they can have significantly different impacts on the training and performance of deep learning models. The <mark style="background: #ABF7F7A6;">choice of activation function can affect the learning process, convergence speed, and even the ability of the model to generalize from training to unseen data</mark>. The impact of these differences indeed depends on various factors, including the architecture, the specific problem being addressed, and the characteristics of the dataset. Here's how:

<mark style="background: #FFF3A3A6;">Without an activation function, a neural network (NN) or model effectively becomes a linear regressor or classifier</mark>. This is because each layer in the NN would only be performing a linear transformation (a matrix multiplication followed by a bias addition) on its inputs. Without non-linear activation functions, no matter how many layers you stack together, the entire network would still represent a single linear transformation, as the composition of linear functions is itself linear. This severely limits the network's capacity to model complex, non-linear relationships within the data.

<mark style="background: #FFB8EBA6;">For classification tasks, the output of such a linear model would be a linear function of the input features. </mark>For a binary classification problem, for example, the model might output a single scalar value for each input, where the sign of the scalar (positive or negative) could be interpreted as belonging to one class or the other.

### Impact on the Model

1. **Vanishing and Exploding Gradients**: Activation functions like Sigmoid and Tanh can suffer from vanishing gradients on deep networks, where gradients become very small, slowing down training or stopping it altogether. ReLU and its variants (like Leaky ReLU or Parametric ReLU) were introduced to mitigate this issue, particularly in deep networks, by maintaining larger gradients. However, ReLU can lead to the "dying ReLU" problem, where neurons can "die" during training and stop responding to variations in error because they get stuck in the regime where they output zero.

2. **Learning Dynamics**: Non-linear functions like<mark style="background: #FFB8EBA6;"> GELU and Swish introduce more complex learning dynamics than ReLU, potentially allowing models to learn more complex patterns or relationships within the data</mark>. This is because they offer smoother gradients over a wider range of input values, which can be beneficial in tasks where capturing subtle nuances in the data is crucial.

3. **Model Convergence**: The choice of activation function can affect how quickly a model converges to a solution during training. For example, smoother functions like GELU or Swish might allow for more stable gradient descent in some scenarios, potentially leading to faster convergence.

### Dependency on Architecture and Task

- **Architecture**: Certain architectures might be specifically designed or optimized to work with particular activation functions. For instance, Convolutional Neural Networks<mark style="background: #FFB8EBA6;"> (CNNs) have been found to work exceptionally well with ReLU</mark> and its variants for tasks like image recognition, while Recurrent Neural Networks <mark style="background: #FFB8EBA6;">(RNNs) might benefit from the properties of Tanh or Sigmoid</mark> in handling time-series data.

- **Task Complexity**: For simple tasks, the difference between activation functions might not be very pronounced, and basic functions like ReLU might suffice. However, for more complex problems, such as natural language processing (NLP) or highly nuanced classification tasks, more sophisticated functions like<mark style="background: #FFB8EBA6;"> GELU or Swish could provide a performance edge by enabling the model to capture complex patterns </mark>more effectively.

- **Dataset Characteristics**: The nature of the dataset, including the scale of input features and the complexity of the relationships within the data, can also influence the effectiveness of different activation functions. Functions that provide smoother transitions and non-linearities (like GELU or Swish) might handle nuanced data relationships better than simpler functions.

### Conclusion

The choice of an activation function is an empirical question and often depends on experimentation within the specific context of a given model, architecture, and dataset. While ReLU and its variants remain popular for their simplicity and effectiveness in many scenarios, the exploration of alternative functions like GELU, Swish, or even newer ones can lead to performance improvements in certain situations. This decision can be influenced by factors such as the need to address vanishing or exploding gradients, the desire for faster convergence, or the requirement to model complex patterns within the data.


---

# Vectorizer:


The TF-IDF Vectorizer, short for Term Frequency-Inverse Document Frequency Vectorizer, is a technique used to convert text documents into a matrix of token counts while also considering the importance of each token across the documents. It is implemented in Python through libraries such as scikit-learn (`TfidfVectorizer`). Here’s what it does:

### 1. **Term Frequency (TF):**
This measures how frequently a term occurs in a document. Since documents can vary in length, the term frequency is often divided by the document length (the total number of terms in the document) to normalize it.

\[ \text{TF}(t, d) = \frac{\text{Number of times term } t \text{ appears in document } d}{\text{Total number of terms in document } d} \]

### 2. **Inverse Document Frequency (IDF):**
This measures how important a term is across all documents in the corpus. The idea is that terms that appear in many documents are less important or informative than terms that appear in fewer documents. It is calculated as the logarithmically scaled inverse fraction of the documents that contain the word, obtained by dividing the total number of documents by the number of documents containing the term, and then taking the logarithm of that quotient.

$$\text{IDF}(t) = \log \left( \frac{\text{Total number of documents}}{\text{Number of documents with term } t} \right) $$

### TF-IDF Calculation:
The TF-IDF value is calculated by multiplying TF and IDF. This gives high values for terms that are more unique to a particular document, helping to identify and weigh the most important words in each document.

$$[ \text{TF-IDF}(t, d) = \text{TF}(t, d) \times \text{IDF}(t) ]$$

### Application and Purpose:
- **Feature Extraction from Text:** Converts text data into a format that machine learning algorithms can work with, by creating a numerical representation of the documents.
- **Importance Weighting:** Helps in emphasizing words that are more relevant to a document’s context, improving the performance of algorithms on tasks like classification, clustering, and information retrieval.
- **Dimensionality Reduction:** By considering only the most important terms, TF-IDF can help reduce the number of features in a high-dimensional dataset.

In summary, the TF-IDF Vectorizer is a powerful tool for processing text data, transforming it into a structured, numerical format that highlights the relative importance of terms within and across documents in a corpus. This makes it invaluable for many NLP tasks where the significance of words plays a crucial role in understanding and analyzing the text.

### Feature Extraction - Example
vectorizer = TfidfVectorizer(max_features=1000)
X = vectorizer.fit_transform(df['processed_reviews'])

---



## Linear and Logistic Regress:
Logistic Regression is used for binary classification tasks, predicting probabilities that map to two categories. It applies a sigmoid (logit) function to model the probability, ensuring the output lies between 0 and 1.

Linear Regression is used for predicting continuous outcomes, modeling the relationship between dependent and independent variables with a linear equation.

---


# GNNs:

### Equivariance:
Certainly! Here is the example with LaTeX symbols enclosed in `$$`.

### Example

Imagine we have a graph with three nodes \(A\), \(B\), and \(C\). The nodes are connected as follows: \(A\) is connected to \(B\), and \(B\) is connected to \(C\).

#### Original Graph
- **Nodes**: $$A, B, C$$
- **Edges**: $$A-B, B-C$$

Now, let's define a transformation $$g$$ which permutes the nodes: $$A \to C$$, $$B \to A$$, and $$C \to B$$.

#### Transformed Graph
- **Nodes**: $$C, A, B$$
- **Edges**: $$C-A, A-B$$

#### Applying GNN (Function $$f$$)
The GNN $$f$$ computes some features based on the graph structure. Suppose the GNN outputs features $$\{f_A, f_B, f_C\}$$ for nodes $$A, B, C$$ in the original graph.

#### Equivariance Property
Equivariance means that if we apply the permutation $$g$$ to the input (nodes $$A, B, C$$), the GNN’s output should transform accordingly with a corresponding permutation $$g'$$:

$$ f(g(\text{input})) = g'(f(\text{input})) $$

In our example, if $$g$$ permutes $$A$$ to $$C$$, $$B$$ to $$A$$, and $$C$$ to $$B$$, then the corresponding permutation $$g'$$ should permute the GNN’s output features similarly:

$$ \{f_A, f_B, f_C\} \to \{f_C, f_A, f_B\} $$

### Summary
- **Input Graph**: $$A \to B \to C$$
- **Transformed Graph**: $$C \to A \to B$$
- **Original Output**: $$\{f_A, f_B, f_C\}$$
- **Transformed Output**: $$\{f_C, f_A, f_B\}$$

This illustrates that the GNN’s output respects the same structure and relationships as the transformed input graph, demonstrating equivariance.




---

# Compilation vs. Linking:

### Difference Between Compilation and Linking

#### Compilation
- **Purpose**: Translates source code written in a high-level programming language (like C, C++, or Java) into machine code or intermediate code (like assembly language or bytecode).
- **Process**:
  1. **Lexical Analysis**: Breaks down the source code into tokens.
  2. **Syntax Analysis**: Parses tokens to check for syntax errors.
  3. **Semantic Analysis**: Ensures the code makes sense semantically.
  4. **Optimization**: Improves the performance and efficiency of the code.
  5. **Code Generation**: Converts the parsed code into machine code or an intermediate representation.
- **Output**: Generates object files or intermediate code files.
- **Example Tools**: GCC (GNU Compiler Collection), Clang, javac (Java compiler).

#### Linking
- **Purpose**: Combines one or more object files and libraries into a single executable or library.
- **Types**:
  1. **Static Linking**: Copies all necessary library modules into the final executable. The resulting executable is self-contained.
  2. **Dynamic Linking**: Links library modules at runtime, rather than at compile-time. The executable contains references to the shared libraries.
- **Process**:
  1. **Symbol Resolution**: Matches function calls and variable references in one object file with their definitions in another object file or library.
  2. **Address Binding**: Assigns final memory addresses to the various code and data sections.
- **Output**: Produces an executable file or a library file.
- **Example Tools**: `ld` (Unix linker), `link.exe` (Windows linker).

### Summary
- **Compilation**: Converts source code into machine code or intermediate code.
- **Linking**: Combines multiple object files and resolves references to create an executable or library.

### Example

#### Compilation Example
```bash
gcc -c myfile.c -o myfile.o
```
This command compiles `myfile.c` into an object file `myfile.o`.

#### Linking Example
```bash
gcc myfile.o -o myprogram -lmylib
```
This command links `myfile.o` with the library `mylib` to create the executable `myprogram`.

### References
- [Compilation Process](https://en.wikipedia.org/wiki/Compiler)
- [Linking (computing)](https://en.wikipedia.org/wiki/Linker_(computing))


-----


