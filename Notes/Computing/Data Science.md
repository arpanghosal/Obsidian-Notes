
What all do we have here? 
Well the basics that you should know :
Programming language - python, r, sql and java for data analyses.
The basis of everything is statistics. One should understand regression analyses, hypotheses testing, ML algorithms. ML algo's are something I should probably look more into.
[[ML  and other Algorithms]]

Next important thing is to do some data visualization. Good softwares would be Tableau, Power BI, matplotlib etc. Well it all comes with python anyway, so why worry about it.

In terms of projects, data scientists work on a variety of projects, including:

1.  Predictive Modeling: Data scientists develop statistical models to predict outcomes based on historical data. These models can be used for forecasting, customer segmentation, or fraud detection.
    
2.  Natural Language Processing: Data scientists use machine learning algorithms to extract meaning from text data. This can be used for sentiment analysis, chatbots, or language translation.
    
3.  Image Processing: Data scientists use machine learning algorithms to analyze and classify images. This can be used for facial recognition, object detection, or medical image analysis.
    
4.  Recommendation Engines: Data scientists develop algorithms to recommend products or services to customers based on their past behavior or preferences.


## Epoch, iterations, batch and folds:

Suppose you have a dataset of 1000 samples and you're training a neural network for a classification task.

**Batch Size:**
- Batch size refers to the number of samples that are processed together in each iteration of training.
- Let's say you set a batch size of 32. This means that in each iteration, the model will process and update its weights based on the predictions and loss computed from 32 samples.
- After processing all samples, the model's weights are updated once, which completes an epoch.

**Epoch Size:**
- An epoch is completed when the model has seen and processed every sample in the dataset once.
- In our example with 1000 samples and a batch size of 32, it would take 1000 / 32 = 31.25 iterations to complete one epoch. Since you can't have fractional iterations, you would typically round this up to 32 iterations.

**Iteration:**
- An iteration refers to a single pass through a batch of data.
- With a batch size of 32 and 1000 samples, you need 1000 / 32 = 31.25 iterations to complete one epoch.

**K-Folds Cross Validation:**
- K-Folds is a technique for evaluating a model's performance using different subsets of the data for training and testing.
- Let's say you choose k = 5. This means you'll divide your 1000 samples into 5 folds, each containing 200 samples.
- You would then train and test your model 5 times, using different folds as the testing set while the remaining folds are used for training. This helps to get a more accurate estimate of the model's performance on different data.

**Summary:**
- Batch Size: 32 (number of samples processed together in each iteration)
- Epoch Size: 32 iterations (number of iterations to see all samples once)
- Iteration: Processing one batch of data
- K-Folds Cross Validation: Dividing data into k subsets for training and testing

In summary, batch size defines how many samples are processed at once, iteration refers to processing one batch, epoch size represents how many iterations are needed to see all data once, and k-folds cross-validation involves dividing the data into subsets for evaluating model performance. Each concept has its own role in training and evaluating machine learning models.


## Beginner's projects ( #beginner )
1.  Exploratory Data Analysis: This project involves analyzing and visualizing data to understand its characteristics, such as distribution, correlation, and outliers. You can use tools like Python or R to perform exploratory data analysis on a dataset of your choice.
    
2.  Linear Regression: Linear regression is a statistical method used to model the relationship between two variables. As a beginner, you can start with simple linear regression models and use them to predict outcomes based on historical data.
    
3.  Sentiment Analysis: Sentiment analysis is the process of analyzing text data to determine the sentiment (positive, negative, or neutral) of a piece of text. You can use tools like Python's NLTK library to perform sentiment analysis on social media data or customer reviews.
    
4.  Data Cleaning: Data cleaning is the process of identifying and correcting errors in a dataset. As a beginner, you can start with simple data cleaning tasks like removing duplicates, filling in missing values, or correcting typos.
    
5.  Image Classification: Image classification involves training a machine learning model to classify images into different categories. You can start with simple image classification tasks like classifying handwritten digits or classifying different types of flowers.


[[Resources]]

## Neural Network Terminologies :
- Batch Normalization: Batch normalization is a technique used in neural networks to normalize the inputs of each layer. It helps address the issue of internal covariate shift, which is the change in the distribution of network activations due to the changing distribution of inputs during training. By normalizing the inputs, batch normalization can improve the training speed and stability of the neural network.
 During training, the inputs to each batch normalization layer are normalized to have zero mean and unit variance based on the statistics computed over the current mini-batch.
 
<details>
<summary>   How can batch norm be demonstrated? </summary>
<markdown>
    Let's consider a simplified example to illustrate batch normalization mathematically. Suppose we have a mini-batch of training examples with a batch size of 4, and each example consists of a single feature:
     Mini-batch: [x1, x2, x3, x4]
     1. Compute the mean and variance of the mini-batch: mean = (x1 + x2 + x3 + x4) / 4 variance = ((x1 - mean)^2 + (x2 - mean)^2 + (x3 - mean)^2 + (x4 - mean)^2) / 4
     2. Normalize the inputs within the mini-batch using the mean and variance: x1' = (x1 - mean) / sqrt(variance + epsilon) x2' = (x2 - mean) / sqrt(variance + epsilon) x3' = (x3 - mean) / sqrt(variance + epsilon) x4' = (x4 - mean) / sqrt(variance + epsilon)
    Here, epsilon is a small constant added to the denominator for numerical stability to avoid division by zero. After normalization, the values x1', x2', x3', and x4' represent the normalized inputs within the mini-batch. These normalized values have zero mean and unit variance, which helps stabilize and improve the training process.
    During the training process, the mean and variance are estimated using the mini-batch statistics. In inference or testing, the overall mean and variance learned during training are typically used to normalize the inputs.


</markdown>
</details>



- Epochs: An epoch refers to a single pass of the entire training dataset through a neural network. In other words, it is a measure of how many times the model has seen and processed the entire training data. During each epoch, the model processes the training data in mini-batches, updates its parameters (weights and biases), and evaluates its performance.
    Suppose we have a dataset of 10,000 images and we choose to train our neural network for 50 epochs. It means that the entire dataset will be passed through the network 50 times during training.
    
- Patience: Patience is a term commonly used in the context of early stopping, which is a technique to prevent overfitting in neural networks. It refers to the number of epochs the training process waits to see improvement in the validation loss before stopping the training. If the validation loss does not improve for a specified number of epochs (the patience), the training can be halted to prevent overfitting.
  Let's say we set the patience value to 5. It means that if the validation loss does not improve for 5 consecutive epochs, we will stop the training process, assuming that the model has converged.

- Batch Size: Batch size refers to the number of training examples used in one forward/backward pass of the neural network. During training, the training data is divided into smaller groups or batches, and the model's parameters are updated based on the average gradient computed over the batch. A larger batch size can lead to faster training as it allows for parallelization and efficient use of computational resources, but it may also result in increased memory usage.
  Suppose we choose a batch size of 64. It means that during each iteration, the model will process 64 training examples and update its parameters based on the average gradient computed over those examples.

- Iterations: In the context of neural network training, an iteration typically refers to one update step of the model's parameters using a single batch of training examples. In other words, an iteration occurs when a batch is fed forward through the network, the loss is computed, and the gradients are propagated backward to update the model's parameters. The number of iterations required to complete an epoch depends on the batch size and the size of the training dataset. If we have a total of 10,000 training examples and a batch size of 64, it will take approximately 157 iterations to complete one epoch (10,000 / 64 = 156.25).



## Why parameterize model parameters?
 - reduce time taken for model inference
 - reduce file/model size

![[Pasted image 20230724142836.png]]
For the above, we have 
 input = **Input**((**None**, **50**))  
 dense = **Dense**(**100**)(input)  
 dense = **Dense**(**1**)(dense)  
 dense = **Dense**(**100**)(dense)  
 output = **Dense**(**50**)(dense)  
 model = **Model**(input, output)

For any kind of NN, first thing is to make architecture, then build the model according to it. In an NN, the hyperparameters to tune are the number of neurons, activation function, optimizer, learning rate, batch size, and epochs. One can also tune # of layers.
### Keras 
A high-level API, in the context of deep learning, refers to an interface or library that provides a user-friendly and abstracted way to interact with the underlying deep learning framework. It simplifies the process of building, training, and evaluating deep learning models by hiding low-level implementation details and providing easy-to-use abstractions. Keras brings in simplicity with syntax and use, compatibility with backends, creating complex models etc. Transitions to other frameworks is also easier.
Keras, originally a separate deep learning library, is now integrated into TensorFlow as `tf.keras`, providing the high-level API functionality within the TensorFlow framework. Enjoy the ease of Keras while benefiting from the extensive capabilities and ecosystem of TensorFlow as the backend.

### workflow of NN
An **activation function is a parameter in each layer**.
  Input data are fed to the input layer, followed by hidden layers, and the final output layer. The output layer contains the output value. 
     The input values moving from a layer to another layer keep changing according to the activation function. 
           **The activation function decides how to compute the input values of a layer into output values**. 
              The output values of a layer are then passed to the next layer as input values again.

Each activation function has its own formula (and graph) to compute the input values.

**Optimizer** - responsible to change the LR (learning rate) and weights of neurons in the NN to reach minimum loss fn.

 Trade off always between LR and epochs, less capacity and memory. More one is, others have to be less. 
      A higher learning rate makes the model learn faster, but it may miss the minimum loss function and only reach the surrounding of it. A lower learning rate gives a better chance to find a minimum loss function. As a tradeoff lower learning rate needs higher epochs, or more time and memory capacity resources.


**Batch size** - sub sets of total training set. If I have X = 100,000 images, i can train in sets of 10,000 ten times. But variance between batches is a major factor to train. However, such batching improves learning and size management. Huge batches/datasets means model building can take time.

After batching comes epoch, i.e. number of times a whole dataset is passed through the neural network model is called an epoch. One epoch means that the training dataset is passed forward and backward through the neural network once.

---

### Backpropagation
Passing a training dataset backward through a neural network is a fundamental step in the training process, known as "Backpropagation".
1. **Forward Pass**: In the forward pass, the input data (training dataset) is fed into the neural network, and the data propagates layer by layer through the network. At each layer, the input is transformed through a series of weighted transformations (linear operations) and activation functions (non-linear operations). Eventually, the network generates predictions or output.
2. **Loss Calculation**: After the forward pass, the output of the neural network is compared to the actual labels (ground truth) from the training dataset. This comparison is done using a loss function (e.g., Mean Squared Error, Cross-Entropy) that quantifies the discrepancy between the predicted values and the true values.
3. **Backpropagation**: Backpropagation is the process of computing the gradients of the loss function with respect to the model's parameters (weights and biases). It involves working backward through the layers of the neural network to calculate how much each parameter contributed to the overall error.
4. **Gradient Descent**: Once the gradients have been computed, the optimization algorithm (typically a variant of gradient descent) uses these gradients to update the model's parameters in a way that minimizes the loss function. This step is essential for "learning" in the neural network as it guides the model to improve its predictions. 
5. **Parameter Updates**: The computed gradients are used to update the model's parameters using an optimization algorithm (e.g., gradient descent or its variants). The optimization algorithm adjusts the model's parameters to minimize the loss function, effectively improving the model's performance on the training data.
6. **Iterative Process**: The forward pass, loss calculation, backpropagation, and parameter update are iteratively performed multiple times (across multiple epochs) during the training process. Each iteration helps the model adjust its parameters to reduce the prediction error and improve its performance on the training data.
In backpropagation, we pass the output of the neural network backward through the layers, but we do not pass it all the way back to the original input data (input dataset). Instead, we pass it back to the layers of the network to update the model's parameters (weights and biases) so that the network learns from the training data.

### Optimizers 
Algorithms used to update parameters. There can be multiple, most famous being ADAM, Nadam etc.


## Optuna 


## Parts of a DNN
_Nodes_ are individual units within a neural network that receive input from the previous layer and produce output for the next layer. Each node performs a weighted sum of the input data, applies an activation function to the result, and passes the output to the next layer.

_Activation functions_ are used within nodes to introduce nonlinearity into the network output. They are used to model complex relationships between the input and output data and ensure that the network output is bounded and can be easily interpreted.

_Dropout layers_ reduce overfitting in a neural network by randomly dropping out a percentage of nodes during training. This helps prevent the network from becoming too specialised in the training data and ensures that it can generalise to new data.

_Batch normalisation layers_ are used to normalise the input data to each layer of the network, improving the stability and performance of the network. They work by normalising the output of each layer to have a mean of 0 and a standard deviation of 1, making it easier for the network to learn the appropriate weights and biases for each layer.

<mark style="background: #FFB8EBA6;">ReLU -> f(x) = max(0,x)</mark>

---

##  Local Minima in a loss function (how to deal)
Dealing with multiple local minima in a loss function is a common challenge in training machine learning models. While techniques like k-fold cross-validation and sampling can help improve the model's performance, they may not directly address the issue of getting stuck in local minima. Here's how these techniques can play a role:

1. **K-Fold Cross-Validation:** K-fold cross-validation is a technique used to assess the model's performance by partitioning the dataset into k subsets. It helps in estimating the model's generalization ability and robustness. While k-fold cross-validation can provide a better understanding of the model's performance on different subsets of data, it doesn't directly address the issue of local minima during training.

2. **Sampling Techniques:**
   - **Random Sampling:** Randomly shuffling the training data or using random sampling for mini-batch training can help the optimization process escape from some local minima and explore different parts of the loss landscape. This is because random sampling introduces more variability in the gradient updates.
   - **Mini-Batch Gradient Descent:** Using mini-batch gradient descent instead of full-batch can help the model navigate out of local minima more effectively. The noise introduced by mini-batch updates can help the optimization process escape from flat regions of the loss landscape.
   - **Stochastic Gradient Descent (SGD):** In SGD, a single randomly chosen sample is used for each update, which introduces even more noise. While this noise can help escape local minima, it might also lead to slower convergence.

3. **Initialization:** Proper initialization of model parameters can also influence whether the optimization process gets stuck in a local minimum. Using techniques like Xavier/Glorot initialization or He initialization can help the optimization process start from a better point in the loss landscape.

4. **Learning Rate Scheduling:** Adjusting the learning rate during training can help the optimization process navigate around the loss landscape more effectively. Learning rate scheduling techniques like learning rate decay or adaptive learning rate methods can be beneficial.

5. **Regularization:** Regularization techniques like L1 or L2 regularization can have a smoothing effect on the loss landscape, potentially reducing the presence of sharp local minima.

6. **Network Architecture:** The architecture of the neural network itself can influence the presence of local minima. Complex architectures might have more complicated loss landscapes, but they can also increase the chances of finding good solutions.

7. **Optimization Algorithms:** Some optimization algorithms, like Adam and RMSProp, use adaptive learning rates and momentum, which can help navigate the loss landscape more effectively.

It's important to note that while these techniques can help the optimization process escape local minima, there's no guarantee that they will find the global minimum. Often, the choice of optimization algorithm, learning rate, and initialization strategy depends on empirical experimentation to find the best combination for a specific problem.

---

## Bias - Variance Tradeoff :
Sources:  US ml 2023 Javier's 1st lecture, ask chatgpt.
If L is squared loss, it can be decomposed to two parts while calculating the Expected Test Error: 
E[Lp] = Const. * (Variance  + Bias$^2$)

**Variance** : difference in predictions when training on different datasets. 
Variance in the context of machine learning refers to how much the predictions of a model vary or deviate from the actual target values in the training data. A model with high variance can fit the training data very closely, sometimes even capturing noise and outliers, but it might not generalize well to new, unseen data because it's too sensitive to small changes in the training data.

**Bias** : difference in ground truth.
Bias refers to the error that occurs due to overly simplistic assumptions in the learning algorithm. It's the difference between the predicted values of the model and the true values (ground truth). A high bias means the model is underfitting the data and isn't capturing the underlying patterns well. It consistently misses the target, leading to systematic errors.

Both high bias and high variance can lead to poor generalization and reduced predictive performance on new data. The challenge is finding the right balance between bias and variance to create a model that performs well on both the training and new data.

Example - Robot shooting nicely precise arrows but as soon as you change angle by little bit, it goes off totally wrong. Variance.
Robot consistently shoots arrows with less accuracy. Means in build bias. 

### How to deal with it? Or how to see it?
When evaluating a machine learning model to understand variance, you can consider several metrics and visualizations that provide insights into its performance and potential issues related to variance:

1. **Learning Curves:** Plot the model's performance (e.g., accuracy or loss) on both the training and validation sets as a function of the number of training examples. High variance can be observed if the training performance is much better than the validation performance, indicating overfitting.

2. **Cross-Validation:** Use k-fold cross-validation to assess the model's performance on multiple folds of the data. If the model's performance varies significantly across different folds, it could indicate high variance.

3. **AUC-ROC Curve:** The Area Under the ROC Curve (AUC-ROC) measures the model's ability to discriminate between classes. If the AUC is very high on the training set but drops significantly on the validation or test set, it might indicate variance.

4. **Precision-Recall Curve:** Similar to AUC-ROC, the Precision-Recall curve provides insights into the model's performance across different thresholds. High variance can be observed if there's a significant gap between training and validation/test curves.

5. **Validation Metrics:** Keep an eye on metrics like accuracy, precision, recall, F1-score, etc., on both training and validation/test data. If there's a significant drop in these metrics on validation/test data compared to training data, it suggests variance.

6. **Overfitting Detection:** Observe when the model starts to overfit. If the training loss continues to decrease while the validation loss starts increasing or stagnating, it's a sign of high variance.

7. **Bias-Variance Trade-off:** Analyze the bias-variance trade-off. If increasing model complexity (e.g., adding more features, increasing model parameters) leads to better training performance but worse validation performance, it's an indication of high variance.

8. **Feature Importance:** Check the importance of features. If the model heavily relies on a subset of features and doesn't generalize well to new data, it might be due to high variance.

Remember that while AUC and other metrics can provide insights, the main goal is to identify a model that performs well on both training and validation/test data. If the model shows excellent performance on the training data but significantly worse performance on new data, it's likely experiencing high variance and overfitting.

Variance can be squeezed, but that means that bias needs to be shifted a bit. There's a trade-off involved in them.

---



## Autoencoders - huge for anomaly detections


Autoencoders are a type of artificial neural network used in unsupervised machine learning and dimensionality reduction tasks. They are a specific class of neural network architecture designed to encode input data into a lower-dimensional representation and then decode it back to its original form. The primary purpose of autoencoders is to learn a compressed representation of the input data, capturing its most important features while discarding unnecessary details.

Here's how autoencoders work:

1. **Encoder**: The encoder component of an autoencoder takes the input data and maps it to a lower-dimensional representation, often referred to as a "latent space" or "encoding." This encoding typically has a much lower dimensionality than the original input. The encoder network consists of one or more layers of neurons responsible for reducing the input's dimensionality.

2. **Latent Space**: The encoding produced by the encoder network contains a compressed representation of the input data. It captures essential features and patterns in the data while reducing noise and less relevant information. The dimension of the latent space is a hyperparameter set by the designer and can be adjusted based on the specific task.

3. **Decoder**: The decoder component of an autoencoder takes the encoded representation from the latent space and attempts to reconstruct the original input data. Like the encoder, the decoder network consists of one or more layers of neurons, but it typically mirrors the structure of the encoder in reverse order. The decoder's output should ideally match the input data as closely as possible.

4. **Loss Function**: To train an autoencoder, a loss function is defined to measure the difference between the reconstructed data and the original input. Common loss functions for this purpose include mean squared error (MSE) or binary cross-entropy, depending on the nature of the data (continuous or binary).

The training process involves minimizing the loss function by adjusting the network's weights and biases using optimization techniques like gradient descent. Once trained, the autoencoder can be used for various tasks:

- **Dimensionality Reduction**: The learned encoding in the latent space can be used for dimensionality reduction. It can capture the most important features of the data while reducing its dimensionality, making it useful for visualization or feature extraction.

- **Anomaly Detection**: Autoencoders can be used to detect anomalies or outliers in data. When the reconstruction error is significantly higher for a particular input, it may indicate an anomaly.
- "We set a threshold for the reconstruction error. Transactions with reconstruction errors above this threshold are considered anomalies or potential fraud"

- **Data Denoising**: Autoencoders can be used to remove noise from data by learning to represent the underlying patterns while ignoring noise.

- **Image Generation**: Variational Autoencoders (a type of autoencoder) are used in generating new data samples, such as generating realistic images.

Autoencoders have found applications in a wide range of fields, including computer vision, natural language processing, and signal processing, among others. They are a versatile tool for various unsupervised and generative tasks.

![[Pasted image 20231003033916.png]]

---
