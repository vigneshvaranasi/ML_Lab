### **Why is Data Pre-processing Needed?**

Real-world data often contains noise, missing values, and inconsistent formats, making it unsuitable for machine learning. Pre-processing cleans and structures data, improving model accuracy and efficiency.

### **Steps in Data Pre-processing**

### **1. Getting the Dataset**

Data is collected and stored in formats like CSV, XLSX, or HTML for easy access in machine learning models.

### **2. Importing Libraries**

Essential libraries include:

- **NumPy** – For mathematical operations.
- **Matplotlib** – For data visualization.
- **Pandas** – For data manipulation and handling datasets.

### **3. Importing Datasets**

Using `read_csv()` in Pandas, datasets are loaded into memory. Features (independent variables) and target (dependent variables) are extracted using `.iloc[]`.

### **4. Handling Missing Data**

Missing values are replaced using statistical techniques like the mean, implemented with `Imputer` from Scikit-learn.

### **5. Encoding Categorical Data**

Categorical variables (e.g., Country, Gender) are converted into numerical values using `LabelEncoder` for ordinal data and `OneHotEncoder` for nominal data.

### **6. Splitting the Dataset**

Data is divided into training and test sets using `train_test_split()`, ensuring the model learns patterns and generalizes well.

### **7. Feature Scaling**

Feature values are standardized to ensure no variable dominates others, improving model stability and performance.

---
A **Perceptron** is an Artificial Neuron, which acts as the fundamental building block for **Artificial Neural Networks (ANNs)**. It was first introduced by **Frank Rosenblatt** in 1957 using an IBM 704 computer at **Cornell Aeronautical Laboratory**.

### **Working of a Perceptron**

A perceptron mimics biological neurons, where inputs are received as electrical signals, stored, and used to make decisions based on past experiences. It is a **Supervised Learning** algorithm, primarily used for **binary classification tasks** (classifying inputs as either **0 or 1**).

### **Perceptron Learning Rule**

- The perceptron starts with **random weights**.
- It iteratively **updates the weights** based on errors in classification.
- If a training example is **misclassified**, the weights are adjusted using the **Perceptron Training Rule**.
- This process continues until the perceptron correctly classifies all training examples.

## **Perceptron Algorithm**

### **Step 1: Initialize Weights**

- Assign small random values to the weights.
- Choose a **learning rate (α)** (typically a small value like **0.01** or **0.1**).

### **Step 2: Repeat for each epoch**

- Loop through all training examples multiple times.

### **Step 3: Compute the Weighted Sum**

**`sum_unit=w0⋅x0+w1⋅x1+...+wn⋅xn`**

- Here, `x0,x1,...,xn` are input features.
- `w0,w1,...,wn` ****are corresponding weights.

### **Step 4: Apply Activation Function**

- **`If sum_unit > threshold, set output 1 (fire).`**
- Otherwise, set output **0** (no fire).

### **Step 5: Update Weights**

If the predicted output **o** is incorrect, update the weights using:

**`wi=wi+α(t−o)xi`**

where,

- α = Learning rate
- t = Target Output
- o = Predicted Output

### **Step 6: Repeat Until Convergence**

- If no weight updates are required (all examples classified correctly), stop training.
- Otherwise, repeat the process until **global error = 0**.