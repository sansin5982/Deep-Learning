# Neuron

An **artificial neuron** is a **mathematical function that mimics the behavior of a biological neuron** in our brain.  
It **receives multiple inputs, processes them using weights, adds bias, and passes them through an activation function to produce an output**.

It is the **core building block of any neural network**.

---

## Structure of an Artificial Neuron

1. **Inputs:**  
   - Data (features), e.g., Age, Income, etc.

2. **Weights:**  
   - Importance given to each input.

3. **Summation:**  
   - Weighted sum of inputs:  
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async
  src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
</script>

   $
   z = \sum (w_i \times x_i) + b
   $

4. **Activation Function:**  
   - Applies a function to add non-linearity (like decision-making).
   - Examples: Sigmoid, ReLU, Tanh.

5. **Output:**  
   - Result after applying activation function.

---

## Mathematical Formula

$
\text{Output} = Activation\left(\sum_{i=1}^{n} (w_i \times x_i) + b\right)
$

Where:
- $w_i$ = weight
- $x_i$ = input
- $b$ = bias
- Activation() = function like Sigmoid, ReLU

---

## Analogy:
Imagine you are a **teacher grading students** based on:
- Homework (weight = 0.4)
- Exam (weight = 0.6)

You add the scores with different importance:
$
\text{Final Grade} = (\text{Homework} \times 0.4) + (\text{Exam} \times 0.6)
$

If the **result is above a threshold**, you decide **Pass**; else, **Fail**.

This is what a neuron does!

---

## Key Concepts in Artificial Neuron

| Component             | Role                                       |
|-----------------------|--------------------------------------------|
| Inputs $(x_1, x_2, ...$)   | Raw data                                |
| Weights ($w_1, w_2, ...$) | Importance of each input                |
| Bias ($b$)            | Adjustment to the output                   |
| Summation               | Weighted sum of inputs and bias            |
| Activation Function     | Adds non-linearity (like decision-making)  |
| Output                  | Final result                               |

---

## Why do we use **Activation Functions** in Neurons?
- **Without activation function:** The neuron would behave like a simple linear equation (a straight line).
- **With activation function:** Neuron can model **non-linear relationships**.
- This makes the model **powerful enough to solve complex problems like image or speech recognition**.

---

## Visual Representation of an Artificial Neuron
<img src="hidden.png" alt="Drawing" style="width: 400px;"/>

---

### Key Takeaways:
- **Neuron is the smallest unit in an Artificial Neural Network.**
- It **transforms inputs into meaningful outputs using weights, bias, and activation function.**
- Multiple neurons connected together form layers that can solve **very complex tasks like face recognition, language translation, etc.**

---
