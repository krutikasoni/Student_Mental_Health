# 🧠 Predicting Mental Performance of Students Using Academic Data

This project explores the relationship between academic and mental performance using a custom-defined mental score. It leverages machine learning to predict whether a student is mentally "healthy" or "unhealthy" based on various academic and lifestyle factors.


## 🎯 Objective

- Predict a student's mental performance based on academic and personal indicators.
- Identify at-risk students to enable early intervention strategies.
- Use clustering and feature importance analysis to generate actionable insights for schools and policymakers.


## 📊 Dataset & Feature Engineering

- Aggregated academic performance data with custom-calculated **Mental_Score**
- Weighted formula included:  
  - Parental involvement, extracurricular activity, sleep hours, motivation level, family income, peer influence, parental education level
- Binary classification created:
  - **Healthy**: Mental score > 5.46  
  - **Unhealthy**: ≤ 5.46


## 🧪 Models & Performance

| Model               | Accuracy | AUC-ROC | F1-Score |
|--------------------|----------|---------|----------|
| Logistic Regression| 0.999    | 0.999   | 0.999    |
| Neural Network      | 0.998    | 0.999   | 0.998    |
| XGBoost             | 0.968    | 0.995   | 0.968    |
| Random Forest       | 0.930    | 0.985   | 0.930    |
| Naive Bayes         | 0.898    | 0.964   | 0.898    |
| KNN                 | 0.813    | 0.886   | 0.813    |

- **Best Model**: Logistic Regression (but also evaluated XGBoost and Neural Net)
- Addressed class imbalance using **upsampling**
- Risks of false positives and false negatives analyzed for real-world deployment


## 🔍 Clustering & Insights

- Cluster A: Low-engagement students, moderate attendance
- Cluster B: High academic performers with low extracurricular participation (may lack balance)
- Cluster C: Well-rounded students with high scores, balanced lifestyle

### Key Feature Importance (from XGBoost):
- Extracurricular Activities (most impactful)
- School Type
- Study Hours and Attendance


## 💡 Business & Social Implications

- **For Schools**: Invest in extracurriculars, improve attendance incentives, offer mentorship
- **For Policymakers**: Promote holistic well-being—not just test scores
- **For EdTech Investors**: Opportunity to support mental wellness tools using ML/NLP


## 🛠 Tools & Technologies

- Python (pandas, scikit-learn, XGBoost, Keras)
- Jupyter Notebook
- Confusion Matrix & AUC for evaluation
- Clustering for profiling (K-Means)


## 📈 Future Enhancements

- Add temporal data & underrepresented attributes (e.g., perceived academic pressure)
- Collaborate with psychologists to validate metrics
- Use NLP for text-based self-reported stress analysis
- Improve robustness & generalizability with more diverse datasets


## ✅ Outcome

This project presents a replicable, data-driven framework to identify students at mental risk, highlighting the power of integrating academic data with mental health indicators for proactive, student-centered interventions.
