Here we will put some ML algorithms as I learn them on the way.

## FFT :

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


[[Self Notes]]



## MM algorithm - minorize-maximize


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
[[Data Science#Autoencoders - huge for anomaly detections]]
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

