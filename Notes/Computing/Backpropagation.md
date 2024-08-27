
Backpropagation is the method for training neural networks, involving two main steps: a forward pass to compute the loss, and a backward pass to update the weights and biases.

### Forward Pass:
1. **Output Calculation**: 
   $$\hat{y} = f(W \cdot X + b)$$
   Here, \(f\) is the activation function, \(W\) and \(b\) are the weights and biases, \(X\) is the input, and $$ \hat{y} $$ is the predicted output.

2. **Loss Calculation**: 
   $$L = loss(y, \hat{y})$$
   \(L\) is the loss comparing predicted output \(\hat{y}\) to actual output \(y\).

### Backward Pass (Backpropagation):
Calculate gradients and update weights and biases:
- **Gradient of Loss wrt Outputs**: Compute $$\frac{\partial L}{\partial \hat{y}}$$.
- **Update Rules**: 
   - Weights: $$W = W - \alpha \frac{\partial L}{\partial W}$$
   - Biases: $$b = b - \alpha \frac{\partial L}{\partial b}$$
   $$\alpha $$ is the learning rate.

### Conceptual Diagram:

```
[Input X] --> [WX + b] --> [Activation f] --> [\hat{y}] --> [Loss L]
     |                                                                  |
     |_______________________ Backpropagate ____________________________|
                                      |                      |
                              Update W                  Update b
```

- Forward pass computes output and loss.
- Backpropagation calculates gradients and updates weights and biases to minimize the loss. This cycle repeats, improving the model.


