# 🧠 Customer Churn Prediction using Deep Learning

This project aims to predict customer churn using a deep learning model built with TensorFlow and Keras. The dataset contains customer information from a telecom company, and the goal is to predict whether a customer will exit or stay based on various attributes.

---

## 📁 Dataset

- **File Used:** `Churn_Modelling.csv`
- **Target Variable:** `Exited`
- **Features:** Includes customer demographics, account information, and transaction details.

---

## 🛠️ Workflow

### 1. Data Preprocessing
- Loaded dataset using Pandas.
- Dropped irrelevant columns: `RowNumber`, `CustomerId`, and `Surname`.
- Applied one-hot encoding on categorical columns: `Geography`, `Gender`.
- Performed train-test split (80/20).
- Standardized features using `StandardScaler`.

### 2. Model Building
- Built a Neural Network using `Keras Sequential API`:
  - **Input Layer:** 11 neurons
  - **Hidden Layers:** 2 layers, 11 neurons each, ReLU activation
  - **Output Layer:** 1 neuron, Sigmoid activation (for binary classification)
- Compiled model with:
  - Loss: `binary_crossentropy`
  - Optimizer: `Adam`
  - Metric: `accuracy`

### 3. Model Training
- Trained the model for **100 epochs** with `validation_split=0.2`.

### 4. Evaluation
- Made predictions on the test set.
- Converted predicted probabilities to binary values using a 0.5 threshold.
- Evaluated performance using:
  - `Accuracy Score`
  - Learning curve visualization (loss & accuracy)

---

## 📊 Results

- The deep learning model was able to effectively learn patterns in the data.
- Accuracy score achieved after training.
- Visualization shows model performance over epochs.

---

## 📌 Tools & Libraries

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- TensorFlow, Keras

---

## 📈 Future Improvements

- Hyperparameter tuning
- Cross-validation
- Try other deep learning architectures (e.g., CNN, LSTM for sequential features)

---

## 🤝 Contributing

Feel free to fork the repo and submit pull requests for improvements!

