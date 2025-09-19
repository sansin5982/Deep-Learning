# Weight

In deep learning, **weights are numbers that represent the importance of each input to a neuron**.  
They **control how much influence an input has on the output of a neuron**.

---

#### Example:
Imagine you are judging a cake based on:
- **Taste**
- **Look**
- **Smell**

You might feel that **taste is the most important**, followed by **look**, and **smell** is less important.

So you can assign:
- Taste → Weight = 0.6  
- Look → Weight = 0.3  
- Smell → Weight = 0.1  

Then, your **overall score of the cake** would be calculated as:
$$
\text{Score} = (\text{Taste Rating} \times 0.6) + (\text{Look Rating} \times 0.3) + (\text{Smell Rating} \times 0.1)
$$

Thus, **weights tell the model which input is more important in decision-making.**

---

### In Deep Learning Neurons:
1. Each neuron receives **multiple inputs (features)**.
2. Each input is **multiplied by a weight**.
3. The weighted inputs are **added up**.
4. The result is passed through an **activation function** to decide the output.

---

### Mathematical View:

<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async
  src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
</script>

$$
\text{Output} = \text{Activation}(w_1 \times x_1 + w_2 \times x_2 + \ldots + w_n \times x_n + b)
$$

Where:

- $w_1, w_2, \ldots, w_n$ = **weights**
- $x_1, x_2, \ldots, x_n$ = **inputs**
- $ b$ = bias
- **Activation function** = makes the output non-linear (like decision-making)

---

### Why are weights important?

| Role                  | Explanation                                  |
|-----------------------|----------------------------------------------|
| Control Importance     | Higher weight → More important input        |
| Learn from data        | Model adjusts weights during training       |
| Prediction accuracy    | Good weights help the model predict better  |

---

###  Key points:
- **Weights are not fixed.**
- They are **learned automatically during training using optimization algorithms (like gradient descent)**.
- **Incorrect weights → Wrong predictions.**
- **Correct weights → Accurate predictions.**

---


<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async
  src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
</script>



## How Does a Deep Learning Model Decide Weights? 

---

### Simple Answer:
A deep learning model **does not start with perfect weights**.  
It **starts with random guesses** for weights and **learns better weights by looking at the errors it makes** during predictions.

This **learning process** is done using algorithms like **Gradient Descent**.

---

#### Step-by-Step Layman Explanation

#### Step 1: Start with random weights
- Model assigns **random numbers (weights)** to inputs.
- These are just guesses at the beginning.

#### Step 2: Make predictions using these weights
- The model predicts an output using these guessed weights.

#### Step 3: Check how wrong the model is (Calculate error)
- Model compares its prediction to the **actual correct answer**.
- Calculates the **error (difference between predicted and actual)**.

#### Step 4: Adjust the weights to reduce the error
- Using **Gradient Descent** (a math method), the model adjusts the weights slightly:
   - If the prediction was too high, decrease the weights.
   - If the prediction was too low, increase the weights.
- This is done using the **Perceptron Learning Rule or backpropagation** in complex models.

#### Step 5: Repeat the process many times (Epochs)
- The model keeps **repeating this process (over the entire dataset)**.
- Over time, the weights adjust to values that help the model **make better and better predictions**.

---

#### Mathematical View (Simplified)

$$
\large \text{New Weight} = \text{Old Weight} - \alpha \times \frac{\partial \text{Error}}{\partial \text{Weight}}
$$

Where:  

- $\alpha$: Learning Rate (small positive number)  
- $\frac{\partial \text{Error}}{\partial \text{Weight}}$: Gradient of Error with respect to Weight  

---

### Real-World Analogy

#### Learning to throw a basketball into a hoop:
1. **First try (Random weight):** You throw blindly.
2. **Check the error:** You see the ball missed the hoop.
3. **Adjust your angle and force (Weight):** Based on how far you missed.
4. **Try again:** Repeat until you start scoring baskets.

**Deep learning models do the same. They adjust their 'throw' (weight) until the 'ball' (prediction) lands close to the 'hoop' (actual label).**

---

#### Summary Table

| Step                | What happens?                                          |
|---------------------|--------------------------------------------------------|
| Initialize           | Random weights assigned                               |
| Predict              | Model makes predictions using current weights         |
| Calculate Error      | Compare predictions with actual output (Loss)         |
| Update Weights       | Use Gradient Descent to adjust weights to reduce error |
| Repeat               | Do this over many passes (epochs)                     |

---



```python

```
