# Basics of Neural Networks

---

### Perceptron
A simple type of artificial neuron that outputs either **0 or 1** based on a linear combination of inputs and a step function. It is the oldest model of a neural network.

### Neuron (Artificial Neuron)
A mathematical unit that receives inputs, applies weights and bias, passes the result through an activation function, and produces an output.

### Weight
A numeric value assigned to each input, representing its importance in the prediction.

### Input
The raw data or features provided to the neural network.

### Output
The final prediction made by the neural network after processing through all layers.

### Hidden Layer
The layers between the input and output layers where the actual learning and pattern extraction happens. They are "hidden" because we do not directly see their outputs.

### Multi-Layer Perceptron (MLP)
A neural network with multiple layers of neurons, including one or more hidden layers, enabling it to learn complex patterns.

### Activation Function
A function applied to the neuron's output that introduces **non-linearity**, allowing the network to learn complex relationships.

### Loss Function
A function that measures the **difference between the predicted output and the actual output**. It guides how much the model's prediction is wrong.

### Gradient Descent
An optimization algorithm that updates the weights by minimizing the loss function using calculated gradients.

### Optimizer
An algorithm that adjusts weights and biases during training (e.g., SGD, Adam), using gradient descent or its variations.

### Epoch
One complete pass over the entire training dataset.

### Batch
A small subset of the dataset used to train the model at one time.

### Iteration
One update of the model's parameters;  
$$
\large \text{Iterations per Epoch} = \frac{\text{Dataset Size}}{\text{Batch Size}}
$$

### Overfitting
When the model learns the training data too well (including noise), but performs poorly on new, unseen data.

### Underfitting
When the model is too simple to capture the patterns in the training data, leading to poor performance on both training and unseen data.

---

