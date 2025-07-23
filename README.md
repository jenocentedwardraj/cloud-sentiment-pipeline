# 🧠 Cloud ML Pipeline for Market Sentiment Classification (PySpark + GCP)

**Author:** Jenocent Edwardraj  
**Timeline:** June – July 2025  
**Tech Stack:** `PySpark` · `Google Cloud Platform (GCS, Dataproc)` · `TF-IDF` · `Logistic Regression` · `Naive Bayes` · `NLP` · `MLlib`  
**Status:** ✅ Completed | 📈 Deployed on Cloud Dataproc

---

## 🚀 Overview

This project builds a full-scale **cloud-native machine learning pipeline** to classify **customer sentiment from unstructured market feedback**. It simulates a real-world scenario of analyzing product reviews, support messages, or user feedback to uncover actionable insights for business teams.

The pipeline was implemented and tested in two environments:
- **Google Colab**: Localized pipeline development and testing on small datasets.
- **Google Cloud Dataproc**: Scalable deployment and execution on a 1M-row synthetic dataset using distributed computing.

---

## 🎯 Problem Statement

Classify sentiment (Positive, Neutral, Negative) based on customer feedback text and additional metadata including:
- **Feedback Text**
- **Response Time**
- **Customer Segment**
- **Interaction Channel**
- **Feedback Length**

---

## 🛠️ Tools & Technologies

| Category         | Stack                                                                 |
|------------------|-----------------------------------------------------------------------|
| Programming      | Python, PySpark                                                       |
| ML / NLP         | TF-IDF, Logistic Regression, Naive Bayes, CountVectorizer             |
| Distributed Infra| Google Cloud Dataproc (Spark Cluster), GCS (Google Cloud Storage)     |
| Dev Environment  | JupyterLab, Google Colab                                              |

---

## 📊 Pipeline Stages

1. **Data Ingestion** from GCS into Spark DataFrame  
2. **EDA** + Null handling + Feature Engineering  
3. **Text Vectorization** using CountVectorizer and TF-IDF  
4. **Label Encoding** using StringIndexer  
5. **Model Training** on:
   - Logistic Regression
   - Naive Bayes
6. **Evaluation** with:
   - Accuracy
   - F1 Score
7. **Deployment** on full dataset using multi-node GCP Dataproc cluster

---

## 📈 Results

| Model              | Dataset      | Accuracy | F1 Score |
|-------------------|--------------|----------|----------|
| Logistic Regression | Small (5%)   | 0.5113   | 0.3460   |
| Naive Bayes         | Small (5%)   | 0.5113   | 0.3460   |
| Logistic Regression | Full (100%)  | 0.5000   | 0.3333   |
| Naive Bayes         | Full (100%)  | 0.5000   | 0.3333   |

> Performance was equivalent across both models. Future work includes adding tree-based classifiers and deep learning-based NLP approaches.

---

## 💡 Key Skills Demonstrated

- **Cloud-Native ML Deployment**: Adapted PySpark pipelines across platforms (Colab → Dataproc)  
- **Distributed Computing**: Handled 1M-row data pipeline on GCP Spark cluster  
- **NLP & Feature Engineering**: Built tokenization + TF-IDF pipelines in PySpark  
- **End-to-End MLOps Thinking**: Preprocessing → Modeling → Evaluation → Cloud Scaling

---

## 📁 Repository Structure

```
├── sentiment_analysis_starter_code_colab.ipynb     # Local Colab version for small data
├── sentiment_analysis_starter_code_gcp.ipynb       # GCP Dataproc-compatible notebook
├── sentiment_small_dataset.csv                     # 5% sample (design/test)
├── sentiment_big_dataset.csv                       # 1M-row full dataset
├── Big Data Analytics in Business Project.pdf       # Final project writeup
└── README.md                                       # ← You're here
```

---

## 📍 Professional Context

This project simulates a production-grade ML pipeline for market sentiment classification, built using PySpark and deployed on Google Cloud Dataproc for scalable execution. It reflects the kind of end-to-end architecture used in real-world data workflows—ingesting unstructured feedback data, engineering NLP features, training classification models, and evaluating performance across cloud environments.

Originally scoped through Arizona State University’s applied analytics curriculum, the project was executed independently from design through deployment, aligning closely with use cases in product analytics, customer experience, and investor sentiment analysis.

---

## 📬 Contact

Feel free to reach out if you'd like to discuss:
- How this project can be extended with better models (e.g., GBTs, LLMs)
- NLP applications in product or financial analytics
- Cloud-native MLOps or scalable pipeline development

📧 jenocent.work@gmail.com  
🔗 [GitHub](https://github.com/jenocentedwardraj)



---

## 📍 Professional Context

This project was completed as part of the “**Big Data & AI in Business**” course at Arizona State University. It reflects real-world data science workflows and is featured on my resume across multiple roles — from **quantitative finance** to **product analytics** to **compliance analytics**.

---

## 📬 Contact

If you'd like to discuss the pipeline, request enhancements, or learn how I adapt this approach to other domains (e.g., credit risk modeling or trend forecasting), feel free to connect:

📧 jenocent.work@gmail.com  
🔗 [GitHub Profile](https://github.com/jenocentedwardraj)
