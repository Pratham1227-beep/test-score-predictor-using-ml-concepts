# 📚 Test Score Predictor using Linear Regression

A simple, interactive **Streamlit application** that predicts a student's test score based on the number of hours they studied. The prediction uses **Linear Regression** computed via the **Normal Equation**. Users can also input actual scores to evaluate prediction accuracy and track progress through a built-in history log.

---

## 🚀 Features

- 📈 **Linear Regression-Based Prediction**  
  Predict scores using a pre-trained model built on sample data.

- 🧑‍🎓 **Student-Specific Inputs**  
  Enter student name, hours studied, and optional actual test score.

- 🧾 **Prediction History Tracking**  
  Stores all predictions during a Streamlit session via `st.session_state`.

- 📥 **CSV Export**  
  Download all predictions for later review.

- 📉 **Interactive Regression Plot**  
  Visualizes:
  - Training data  
  - Regression line  
  - User predictions  

---

## 🧩 Technologies Used

- Python  
- Streamlit  
- NumPy  
- Pandas  
- Matplotlib

---

## 📦 Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/test-score-predictor.git
   cd test-score-predictor
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the application**
   ```bash
   streamlit run app.py
   ```

---

## 🧠 How the Model Works

The model is trained on this dataset:

| Hours | Score |
|-------|--------|
| 1     | 50     |
| 2     | 60     |
| 3     | 65     |
| 4     | 70     |
| 5     | 80     |

The Normal Equation is used:

\[
\theta = (X^T X)^{-1} X^T y
\]

Prediction formula:

\[
\text{Predicted Score} = \theta_0 + \theta_1 \cdot (\text{Hours Studied})
\]

Predictions are capped at **100** for realism.

---

## 📂 Project Structure

```
|── Test Score Predictor.py                 # Streamlit app
│── requirements.txt       # Dependencies
│── README.md              # Documentation
```

---

## 🖼️ What You’ll See

- Input panel for name, hours, and optional actual score  
- Predicted score with error calculation  
- Scrollable prediction history table  
- Regression chart showing all predictions  

---

## 🤝 Contributing

Contributions are welcome!  
Feel free to open issues or submit pull requests.

---
