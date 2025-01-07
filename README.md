# Twitter Sentiment Analysis of AI Topics in Databricks Cloud

This repository contains the code and resources for performing sentiment analysis on Twitter data related to AI topics using the Databricks cloud platform. The project demonstrates how to collect, preprocess, and analyze textual data to derive meaningful insights about public sentiment.

---

## Table of Contents
1. [Overview](#overview)
2. [Features](#features)
3. [Workflow](#workflow)
4. [Setup](#setup)
5. [Usage](#usage)
6. [Results](#results)
7. [Future Work](#future-work)
8. [Contributing](#contributing)
9. [License](#license)

---

## Overview

This project was run in Databricks using Spark to analyze recent news about "AI" for sentiment evaluation. The goal of this project is to practice traditional NLP techniques like:
- Tokenization
- Stopword Removal
- Count Vectorization (CV) and TF-IDF
- N-grams

Additionally, the project applied tools like **AWS S3**, **Athena**, and **QuickSight** to process and visualize big data effectively.

---

## Features
- **Integration with Databricks Cloud**: Seamlessly connects with Databricks for scalable data processing.
- **NLP Pipeline**: Implements traditional NLP techniques for text analysis.
- **Big Data Processing**: Utilizes AWS services (S3, Athena, QuickSight) for handling and visualizing large datasets.
- **Visualization Dashboard**: Includes insightful visualizations of the analysis results.

---

## Workflow

This project aims to practice NLP using Spark and process big data using Amazon Web Services. Below is the workflow diagram:

![Workflow](images/workflow.png)

---

## Setup

### Prerequisites
- Databricks account with access to a workspace.
- AWS credentials with permission to access S3 buckets.
- Python environment with the required libraries (listed in `requirements.txt`).

### Steps
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/Twitter-Sentiment-Analysis.git
   cd Twitter-Sentiment-Analysis
   ```

2. Set up your Databricks workspace:
   - Upload the notebook to Databricks.
   - Configure the AWS credentials in the notebook.

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Mount the S3 bucket:
   Use the provided script to mount your S3 bucket:
   ```python
   def mount_s3_bucket(access_key, secret_key, bucket_name, mount_folder):
       # Code provided in the Jupyter Notebook
   ```

---

## Usage

### Running the Notebook
1. Open the Jupyter Notebook in Databricks.
2. Run the data preprocessing cells to clean and tokenize Twitter data.
3. Train the sentiment analysis model.
4. Visualize results and export insights.

---

## Results

### Sentiment Breakdown
- **Positive Sentiments**: 70%
- **Neutral Sentiments**: 15%
- **Negative Sentiments**: 15%

### Accuracy
- **Correct Predictions**: 2,704
- **Total Predictions**: 2,973
- **Accuracy**: **90.95%**

### Visualizations
Below is a snapshot of the project’s dashboard, showcasing key metrics and insights:

![Dashboard](images/dashboard.png)

---

## Future Work
- Expand the analysis to other datasets and social media platforms.
- Incorporate advanced NLP techniques, such as Transformers (e.g., BERT, RoBERTa).
- Add a web-based dashboard for real-time sentiment tracking.

---

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your proposed changes.
