# Input 

In deep learning, **input is the raw data you provide to the model so that it can learn or make predictions**.

Inputs are usually represented as **numerical values**, but they can come from various sources like images, text, numbers, audio, or sensor data.

---

### Detailed Explanation:
A **neural network (deep learning model) is like a human brain that takes inputs and makes decisions**.

- For humans, inputs come from eyes, ears, skin, etc.
- For machines, inputs are numbers fed into the model.

In deep learning:
- Inputs are **organized into arrays or tensors (like tables of numbers)**.
- Each input can have **one or multiple features** (characteristics of the data).
- The model processes these inputs to **learn patterns, relationships, or make decisions**.

---

### Mathematical View:

<script type="text/javascript" async
    src="https://polyfill.io/v3/polyfill.min.js?features=es6">
</script>
<script type="text/javascript" async
    src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/3.2.0/es5/tex-mml-chtml.js">
</script>

$$
\large \text{Input} = [x_1, x_2, x_3, ..., x_n]
$$

Where:

- $x_1, x_2, x_3, ..., x_n$ are **input features**.

---

### Types of Inputs:

| Type         | Example                                |
|--------------|----------------------------------------|
| Numeric       | Age, salary, temperature              |
| Text          | Sentences, words, documents           |
| Image         | Pixels (converted to numbers)         |
| Audio         | Sound waves converted to numerical values |
| Video         | Series of image frames + audio        |

---

### Real-Life Examples:

| Real-Life Scenario            | Input for Deep Learning Model                            |
|-------------------------------|-----------------------------------------------------------|
| Predicting house price        | Size of the house, number of rooms, location, year built |
| Recognizing handwritten digits | Pixels of the image of the digit (0-9)                   |
| Language translation           | Sentence in English (converted to numbers via embeddings) |
| Voice assistant (like Alexa)   | Audio of spoken words (converted to numerical features)  |
| Predicting if a customer will buy | Age, income, browsing history, past purchases         |

---

### Example:

### Example 1: Cooking Recipe
- **Input:** Ingredients like flour, sugar, milk, etc.
- **Model:** Cook (processes the ingredients)
- **Output:** Cake or Bread

### Example 2: ATM Machine
- **Input:** You enter your **PIN and amount requested**.
- **Model:** ATM system (processes your request)
- **Output:** Cash or transaction declined.

### Example 3: Weather Prediction
- **Input:** Past temperature, humidity, wind speed.
- **Model:** Weather forecasting system.
- **Output:** Tomorrow's weather.

---

### Key Points:
- Input is **what you give to the model**.
- It can be **simple (like a number) or complex (like an image or text)**.
- The **quality and format of the input** directly affect the model's performance.
- **Deep learning models expect inputs as numerical arrays**, even if the original input is text, image, or audio.

---



```python
import numpy as np

# Step 1: Define the input features (as an array)
# Example: Predicting house price using [size, number_of_rooms, location_score]
inputs = np.array([2000, 3, 8])  # e.g., 2000 sq ft, 3 rooms, location score 8

# Step 2: Define the weights (importance of each input)
weights = np.array([0.5, 0.3, 0.2])  # these are randomly assigned for demonstration

# Step 3: Define bias
bias = 5  # extra adjustment added to the output

# Step 4: Calculate the weighted sum
weighted_sum = np.dot(inputs, weights) + bias

# Step 5: Apply activation function (ReLU used here as example)
def relu(x):
    return max(0, x)

output = relu(weighted_sum)

# Display the result
print(f"Input Features: {inputs}")
print(f"Weights: {weights}")
print(f"Weighted Sum (before activation): {weighted_sum}")
print(f"Output (after ReLU activation): {output}")
```

    Input Features: [2000    3    8]
    Weights: [0.5 0.3 0.2]
    Weighted Sum (before activation): 1007.5
    Output (after ReLU activation): 1007.5
    
