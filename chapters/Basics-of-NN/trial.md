---
layout: default
title: MathJax Example
---

<!-- Load MathJax correctly -->
<script type="text/javascript">
window.MathJax = {
  tex: {
    inlineMath: [['\\(','\\)']],
    displayMath: [['$$','$$']]
  },
  svg: {
    fontCache: 'global'
  }
};
</script>
<script src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

## Weight Update Formula

$$
\large \text{New Weight} = \text{Old Weight} - \alpha \times \frac{\partial \text{Error}}{\partial \text{Weight}}
$$

Where:

- \( \alpha \): Learning Rate (small positive number)
- \( \frac{\partial \text{Error}}{\partial \text{Weight}} \): Gradient of Error with respect to Weight  

---

## Testing Inline Math inside Paragraph

The famous formula \( E = mc^2 \) is working here inside a normal text.

---

## Table Example with Math

| Component               | Explanation                               |
|-------------------------|-------------------------------------------|
| Inputs \( x_1, x_2, \ldots \) | Raw data                                |
| Weights \( w_1, w_2, \ldots \) | Importance of each input                |
| Bias \( b \)              | Adjustment to the output                 |



```python

```
