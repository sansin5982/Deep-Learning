<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async
  src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
</script>

# Weight

In deep learning, **weights are numbers that represent the importance of
each input to a neuron**.  
They **control how much influence an input has on the output of a
neuron**.

------------------------------------------------------------------------

#### Example:

Imagine you are judging a cake based on: - **Taste** - **Look** -
**Smell**

You might feel that **taste is the most important**, followed by
**look**, and **smell** is less important.

So you can assign: - Taste → Weight = 0.6  
- Look → Weight = 0.3  
- Smell → Weight = 0.1

Then, your **overall score of the cake** would be calculated as:

Score = (Taste Rating × 0.6) + (Look Rating × 0.3) + (Smell Rating × 0.1)

Thus, **weights tell the model which input is more important in
decision-making.**

------------------------------------------------------------------------

### In Deep Learning Neurons:

1.  Each neuron receives **multiple inputs (features)**.
2.  Each input is **multiplied by a weight**.
3.  The weighted inputs are **added up**.
4.  The result is passed through an **activation function** to decide
    the output.

------------------------------------------------------------------------

### Mathematical View:

Output = Activation(*w*<sub>1</sub> × *x*<sub>1</sub> + *w*<sub>2</sub> × *x*<sub>2</sub> + … + *w*<sub>*n*</sub> × *x*<sub>*n*</sub> + *b*)

Where:

-   *w*<sub>1</sub>, *w*<sub>2</sub>, …, *w*<sub>*n*</sub> = **weights**
-   *x*<sub>1</sub>, *x*<sub>2</sub>, …, *x*<sub>*n*</sub> = **inputs**
-   *b* = bias
-   **Activation function** = makes the output non-linear (like
    decision-making)

------------------------------------------------------------------------

### Why are weights important?

<table>
<thead>
<tr>
<th>Role</th>
<th>Explanation</th>
</tr>
</thead>
<tbody>
<tr>
<td>Control Importance</td>
<td>Higher weight → More important input</td>
</tr>
<tr>
<td>Learn from data</td>
<td>Model adjusts weights during training</td>
</tr>
<tr>
<td>Prediction accuracy</td>
<td>Good weights help the model predict better</td>
</tr>
</tbody>
</table>

------------------------------------------------------------------------

### Key points:

-   **Weights are not fixed.**
-   They are **learned automatically during training using optimization
    algorithms (like gradient descent)**.
-   **Incorrect weights → Wrong predictions.**
-   **Correct weights → Accurate predictions.**

------------------------------------------------------------------------

## How Does a Deep Learning Model Decide Weights?

------------------------------------------------------------------------

### Simple Answer:

A deep learning model **does not start with perfect weights**.  
It **starts with random guesses** for weights and **learns better
weights by looking at the errors it makes** during predictions.

This **learning process** is done using algorithms like **Gradient
Descent**.

------------------------------------------------------------------------

#### Step-by-Step Layman Explanation

#### Step 1: Start with random weights

-   Model assigns **random numbers (weights)** to inputs.
-   These are just guesses at the beginning.

#### Step 2: Make predictions using these weights

-   The model predicts an output using these guessed weights.

#### Step 3: Check how wrong the model is (Calculate error)

-   Model compares its prediction to the **actual correct answer**.
-   Calculates the **error (difference between predicted and actual)**.

#### Step 4: Adjust the weights to reduce the error

-   Using **Gradient Descent** (a math method), the model adjusts the
    weights slightly:
    -   If the prediction was too high, decrease the weights.
    -   If the prediction was too low, increase the weights.
-   This is done using the **Perceptron Learning Rule or
    backpropagation** in complex models.

#### Step 5: Repeat the process many times (Epochs)

-   The model keeps **repeating this process (over the entire
    dataset)**.
-   Over time, the weights adjust to values that help the model **make
    better and better predictions**.

------------------------------------------------------------------------

#### Mathematical View (Simplified)

$$
\large \text{New Weight} = \text{Old Weight} - \alpha \times \frac{\partial \text{Error}}{\partial \text{Weight}}
$$

Where:

-   *α* - Learning Rate (small positive number)

-   $\frac{\partial \text{Error}}{\partial \text{Weight}}$ - Gradient of
    Error with respect to Weight

------------------------------------------------------------------------

### Real-World Analogy

#### Learning to throw a basketball into a hoop:

1.  **First try (Random weight):** You throw blindly.
2.  **Check the error:** You see the ball missed the hoop.
3.  **Adjust your angle and force (Weight):** Based on how far you
    missed.
4.  **Try again:** Repeat until you start scoring baskets.

**Deep learning models do the same. They adjust their ‘throw’ (weight)
until the ‘ball’ (prediction) lands close to the ‘hoop’ (actual
label).**

------------------------------------------------------------------------

#### Summary Table

<table>
<colgroup>
<col style="width: 27%" />
<col style="width: 72%" />
</colgroup>
<thead>
<tr>
<th>Step</th>
<th>What happens?</th>
</tr>
</thead>
<tbody>
<tr>
<td>Initialize</td>
<td>Random weights assigned</td>
</tr>
<tr>
<td>Predict</td>
<td>Model makes predictions using current weights</td>
</tr>
<tr>
<td>Calculate Error</td>
<td>Compare predictions with actual output (Loss)</td>
</tr>
<tr>
<td>Update Weights</td>
<td>Use Gradient Descent to adjust weights to reduce error</td>
</tr>
<tr>
<td>Repeat</td>
<td>Do this over many passes (epochs)</td>
</tr>
</tbody>
</table>

------------------------------------------------------------------------
