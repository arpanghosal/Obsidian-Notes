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

