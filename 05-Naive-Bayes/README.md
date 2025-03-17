### **Naive Bayes Classifier**

Naive Bayes is a **probabilistic classification** algorithm based on **Bayes' Theorem**. It is widely used in **Supervised Learning** for classification tasks. The algorithm assumes that features are **independent** of each other, making it a **"Naive"** assumption.

### **Bayes' Theorem**

Bayes’ theorem is a **mathematical formula** used to compute **conditional probabilities**. It is given by:

$$
P(A∣B)=P(B∣A)⋅P(A)/P(B)
$$

Where:

- P(A∣B) → Probability of event A occurring given that B is true (posterior probability).
- P(B∣A) → Probability of event B occurring given that A is true (likelihood).
- P(A) → Probability of event A occurring independently (prior probability).
- P(B) → Probability of event B occurring independently (evidence).

---

### **Working of Naive Bayes**

1. **Training Phase:**
    - Compute prior probabilities P(A) for each class
    - Compute likelihood P(B∣A) for each feature given the class.
    - Store these probabilities for later use.
2. **Prediction Phase:**
    - For a new input, compute P(A∣B) for each class.
    - Assign the class with the **highest probability**.

---

### **Why "Naive"?**

The algorithm assumes that **all features are independent** of each other, which is often not true in real-world scenarios. Despite this, it works well in many applications.

### **Gaussian Naive Bayes**

When dealing with **continuous data**, Naive Bayes assumes that the values follow a **Gaussian (Normal) distribution**.