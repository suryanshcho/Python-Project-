Based on the project files and the repository structure, here is a professional **README.md** data for the "Zomato Restaurant Clustering and Sentiment Analysis" capstone project.

# Zomato Restaurant Clustering and Sentiment Analysis

## 📌 Project Overview
This project is an Unsupervised Machine Learning capstone designed to analyze Zomato restaurant data. It focuses on two core objectives:
1.  Restaurant Clustering:** Grouping restaurants into segments based on features like cost, cuisines, and timing to help customers find the best options in their locality.
2.  Sentiment Analysis:** Analyzing customer reviews to understand the sentiment (Positive, Negative, or Neutral) towards various restaurants and identifying industry critics.

## Problem Statement
Zomato is one of the largest food delivery and restaurant aggregator platforms. With thousands of restaurants, it becomes difficult for users to choose the right place. The goal is to:
* Cluster restaurants into meaningful segments.
* Analyze customer reviews to provide insights into restaurant performance.
* Help the company identify areas of improvement and help customers make informed decisions.

## Dataset Description
The project utilizes two primary datasets:
* **Zomato Restaurant Metadata:** Contains information like Restaurant Name, URL, Cost per person, Cuisines, and Timings.
* **Zomato Customer Reviews:** Contains Restaurant Name, Reviewer Name, Review Text, Rating, and Reviewer Metadata (Followers/Reviews).

## Technologies Used
* **Language:** Python
* **Libraries:** * Data Manipulation: `Pandas`, `Numpy`
    * Visualization: `Matplotlib`, `Seaborn`, `Plotly`
    * Machine Learning: `Scikit-learn`, `Scipy`
    * NLP: `NLTK`, `Spacy`, `Gensim` (for Text Preprocessing & Vectorization)

## Key Features & Workflow

### 1. Data Preprocessing & EDA
* Handled missing values and duplicates.
* Feature engineering: Extracted "Number of Cuisines" and "Operating Hours."
* Exploratory Data Analysis to find top-rated restaurants, most popular cuisines, and cost distributions.

### 2. Clustering (Unsupervised Learning)
**Algorithms:** K-Means Clustering, Hierarchical Clustering (Agglomerative).
**Evaluation:** Elbow Method and Silhouette Score to find the optimal number of clusters (typically 5 or 6).
**Insight:** Restaurants were clustered based on affordability and cuisine variety.

### 3. Sentiment Analysis (NLP)
**Preprocessing:** Tokenization, stop-word removal, lemmatization, and removing emojis/URLs.
**Vectorization:** TF-IDF and Count Vectorizer.
**Models:** Logistic Regression, Naive Bayes, Random Forest, and Support Vector Machines (SVM).
**Result:** Sentiment classification to distinguish between satisfied and dissatisfied customers.

## 📊 Key Findings
**Cluster Insights:** Identified budget-friendly "pocket-friendly" clusters vs. "premium" luxury dining clusters.
**Sentiment Trends:** Found that higher-cost restaurants don't always guarantee higher ratings; sentiment is often driven by service quality.
**Top Performers:** Identified specific restaurants and reviewers (critics) that have the highest influence on the platform.

## 📁 Repository Structure
```text
├── Data/                                  # Raw and Processed datasets
├── Notebooks/                             # Jupyter Notebooks (main project file)
├── Outputs/                               # Saved plots and model results
└── README.md                              # Project documentation
```

---

### How to Run
1. Clone this repository.
2. Install dependencies: `pip install -r requirements.txt`.
3. Open the `.ipynb` file in Jupyter Notebook or Google Colab.
4. Run all cells to see the analysis and model results.
