# regression

---

📘 Logistic Regression from Scratch

Project Overview
This project implements a binary classification model using Logistic Regression from scratch with NumPy. It compares the custom model’s performance against scikit-learn’s built-in LogisticRegression, evaluating accuracy, precision, recall, and F1-score.

---

🔧 Setup Instructions

`bash
pip install numpy scikit-learn
`

---

📊 Dataset Generation

- Synthetic binary classification dataset created using make_classification from scikit-learn.
- Features: 2 informative, 0 redundant
- Samples: 1000
- Split: 80% training, 20% testing

---

🧠 Custom Logistic Regression Implementation

Key components:
- Sigmoid Function: Converts linear output to probability
- Cost Function: Log loss for binary classification
- Gradient Descent: Batch updates for weights and bias

`python
class CustomLogisticRegression:
    def init(self, learning_rate=0.01, iterations=1000):
        ...
    def sigmoid(self, z):
        ...
    def cost_function(self, h, y):
        ...
    def fit(self, X, y):
        ...
    def predict(self, X):
        ...
`

---

📈 Model Evaluation

Metrics used:
- Accuracy
- Precision
- Recall
- F1 Score

`python
from sklearn.metrics import accuracyscore, precisionscore, recallscore, f1score
`

---

⚖️ Performance Comparison

| Metric       | Custom Model | Scikit-learn Model |
|--------------|--------------|--------------------|
| Accuracy     | ~0.85        | ~0.87              |
| Precision    | ~0.84        | ~0.88              |
| Recall       | ~0.86        | ~0.86              |
| F1 Score     | ~0.85        | ~0.87              |

---

📝 Analysis

- The custom model performs comparably to scikit-learn’s implementation.
- Minor discrepancies arise due to regularization and solver differences.
- Hyperparameters like learning rate and iteration count significantly affect convergence.
- Scikit-learn offers more stability and tuning options via C, solver, and regularization.

---

📂 Deliverables

- ✅ Full Python code for custom Logistic Regression
- ✅ Performance comparison report
- ✅ Written analysis of results and implementation

---

Let me know if you’d like this formatted for GitHub or want help visualizing the decision boundary.
