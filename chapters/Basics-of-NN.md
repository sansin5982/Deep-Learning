<script type="text/javascript" async
    src="https://polyfill.io/v3/polyfill.min.js?features=es6">
</script>
<script type="text/javascript" async
    src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/3.2.0/es5/tex-mml-chtml.js">
</script>

# Basics of Neural Networks

------------------------------------------------------------------------

### Weight

A numeric value assigned to each input, representing its importance in
the prediction.

------------------------------------------------------------------------

### Input

The raw data or features provided to the neural network.

------------------------------------------------------------------------

### Output

The final prediction made by the neural network after processing through
all layers.

------------------------------------------------------------------------

### Hidden Layer

The layers between the input and output layers where the actual learning
and pattern extraction happens. They are “hidden” because we do not
directly see their outputs.

------------------------------------------------------------------------

### Multi-Layer Perceptron (MLP)

A neural network with multiple layers of neurons, including one or more
hidden layers, enabling it to learn complex patterns.

------------------------------------------------------------------------

### Activation Function

A function applied to the neuron’s output that introduces
**non-linearity**, allowing the network to learn complex relationships.

------------------------------------------------------------------------

### Loss Function

A function that measures the **difference between the predicted output
and the actual output**. It guides how much the model’s prediction is
wrong.

------------------------------------------------------------------------

### Gradient Descent

An optimization algorithm that updates the weights by minimizing the
loss function using calculated gradients.

------------------------------------------------------------------------

### Optimizer

An algorithm that adjusts weights and biases during training (e.g., SGD,
Adam), using gradient descent or its variations.

------------------------------------------------------------------------

### Epoch

One complete pass over the entire training dataset.

------------------------------------------------------------------------

### Batch

A small subset of the dataset used to train the model at one time.

------------------------------------------------------------------------

### Iteration

One update of the model’s parameters;

$$
\large \text{Iterations per Epoch} = \frac{\text{Dataset Size}}{\text{Batch Size}}
$$
—

### Overfitting

When the model learns the training data too well (including noise), but
performs poorly on new, unseen data.

------------------------------------------------------------------------

### Underfitting

When the model is too simple to capture the patterns in the training
data, leading to poor performance on both training and unseen data.

------------------------------------------------------------------------

### Summary of Basics of Neural Networks

<table>
<colgroup>
<col style="width: 20%" />
<col style="width: 44%" />
<col style="width: 35%" />
</colgroup>
<thead>
<tr>
<th>Topic</th>
<th>Description</th>
<th>Importance</th>
</tr>
</thead>
<tbody>
<tr>
<td>Perceptron</td>
<td>Simplest neural network structure</td>
<td>Foundation for understanding neural networks</td>
</tr>
<tr>
<td>Multilayer Perceptron</td>
<td>Multi-layer networks capable of complex modeling</td>
<td>Essential for real-world neural applications</td>
</tr>
<tr>
<td>Activation Functions</td>
<td>Non-linear transformations enabling complex patterns</td>
<td>Critical for neural network flexibility</td>
</tr>
<tr>
<td>Loss Functions</td>
<td>Measure model accuracy and guide training</td>
<td>Fundamental for model learning</td>
</tr>
<tr>
<td>Training Neural Networks</td>
<td>Methods to adjust weights effectively</td>
<td>Key to optimizing model performance</td>
</tr>
<tr>
<td>Overfitting &amp; Underfitting</td>
<td>Challenges affecting model generalization</td>
<td>Necessary understanding for effective models</td>
</tr>
<tr>
<td>Validation and Testing</td>
<td>Evaluating true model performance</td>
<td>Ensures robust and reliable results</td>
</tr>
</tbody>
</table>

<table style="width:6%;">
<colgroup>
<col style="width: 5%" />
</colgroup>
<tbody>
<tr>
<td>### Summary Understanding these core concepts and techniques
provides a strong foundation in neural networks, enabling further
exploration of advanced deep learning topics and applications.</td>
</tr>
</tbody>
</table>
