
# 🧠 Mental Health in Tech: A Multi-Year Analysis

## 📌 Introduction

The tech sector has long been linked to heavy workloads, fast-paced work settings, and burnout risks.  Using survey data from the Open Sourcing Mental Illness (OSMI) initiative, this study examines the mental health conditions of tech workers from 2017 to 2021.  The objective is not only to forecast the probability of mental health diagnoses among workers, but also to pinpoint important personal and professional elements that affect wellbeing.

 In order to create a risk indicator and a diagnostic model, this research uses clustering and predictive modeling techniques.  A multi-year trend analysis is also conducted to look at changes in mental health support and attitudes, especially in reaction to COVID-19, which drastically changed work culture and stressors around the world.

## 📊 Datasets

- OSMI Mental Health in Tech Survey (2017–2021)

## 🛠 System Design

1. **Data Preprocessing**
2. **Exploratory Data Analysis (EDA)**
3. **Feature Selection**
4. **Predictive Modeling**
5. **Risk Indicator Modeling (Clustering)**
6. **Trend Analysis – Pre vs. Post COVID**
7. **Chatbot - Mental health Recommendation and Risk Indication**

## 🔧 Preprocessing

- Dropped columns with >50% missing values
- Imputed remaining missing data
- Handled categorical inconsistencies
- Treated numerical outliers
- Encoded data for modeling

## 🔍 Predicting Mental Health Diagnosis

This binary classification task predicts whether an employee has been diagnosed with a mental health condition.

**Models Evaluated:**

1. K-Nearest Neighbors (Best performer: 86.34% Accuracy)
2. Logistic Regression
3. Decision Tree
4. Random Forest
5. AdaBoost
6. Gradient Boosting
7. XGBoost

**Evaluation:**

- Train/Test Split: 70/30
- Metrics: Accuracy, F1 Score, Precision, Recall, ROC AUC
- K-Fold Cross Validation applied

## 📈 Risk Indicator (Clustering)

Clustering methods were used to group employees by mental health risk levels (Low, Medium, High).

**Clustering Models:**

- K-Means
- K-Means++

**Evaluation Metrics:**

- Silhouette Score
- Calinski-Harabasz Index
- SSE

## 💡 Key Inferences

### Influential Factors:
- Willingness to discuss mental health at work
- Employer support and resources
- Personal history of mental illness
- Age, gender, and tech industry status

### Pre/Post COVID Trends:
- More formal discussions and support post-COVID
- Increased mental health awareness
- Greater work-from-home related stress factors

### Chatbot - Mental Health Recommendations and Risk Indication

This intelligent, locally deployed chatbot was created to respond to inquiries around mental health at work using data from the OSMI Mental Health in Tech Survey (2017–2021).  It finds and returns the most semantically relevant answers by converting the user's question and the EDA summary into vectors using a sentence embedding model (MiniLM-L6-v2).  FAISS is used in the construction of the vector storage, allowing for quick and effective similarity search.  The chatbot delivers one or two concise, useful insights after retrieving the most relevant portions from the summary in response to a user's query.It offers broad, encouraging advice in the event that no pertinent match is discovered.  With the help of Streamlit, the chatbot can be implemented as an interactive web application or operated via a terminal interface, maintaining chat history and enabling ongoing multi-question discussion.  All things considered, it turns a static data analysis into a conversational, approachable tool for promoting mental health in the tech industry.

## 📌 Conclusion

In addition to forecasting mental health diagnoses, this initiative identifies workplace trends that exacerbate mental health issues.  Tech companies can use the information to put preventative mental health strategies into practice. In line with this, the chatbot uses information from the OSMI survey to react to inquiries regarding workplace mental health.  To find pertinent answers, it makes use of FAISS and sentence embeddings.  In the end, it offers prompt, helpful responses and raises awareness of mental health issues through an engaging, dialogue-style experience.


Contributors:
Sai Varun Nimmagadda,
Shaheen Chirakula,
Vishnu Vikas Nallamalli.
---
