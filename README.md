# Twitter-Sentiment-Analysis-for-Apple-and-Google-Products
This project uses Natural Language Processing (NLP) and machine learning to classify tweets about Apple and Google products as positive, neutral, or negative. The goal was to determine whether machine learning could be used to automatically analyze customer sentiment from social media conversations.

## Project Summary

This project uses Natural Language Processing (NLP) and machine learning to classify tweets about Apple and Google products as positive, neutral, or negative. The goal was to determine whether machine learning could be used to automatically analyze customer sentiment from social media conversations.
Several classification models were developed and evaluated, including Logistic Regression, Decision Tree, Tuned Decision Tree, and Random Forest. Model performance was compared using Accuracy, Precision, Recall, and Macro F1-Score. Logistic Regression was selected as the final model because it provided the best balance across sentiment classes and achieved the highest Macro F1-Score.

## Project Workflow

### Business Understanding

The project addresses the challenge of understanding customer opinions from large volumes of social media data. Automatically identifying sentiment can help organizations monitor customer feedback and detect potential issues more efficiently.

### Data Understanding

The dataset contains tweets discussing Apple and Google products and includes human-assigned sentiment labels:

* Positive
* Neutral
* Negative

### Data Preparation

The data preparation process included:

* Removing missing values and duplicate records
* Cleaning tweet text
* Removing URLs and punctuation
* Tokenization and lemmatization
* TF-IDF feature extraction

### Modeling

The following models were evaluated:

* Dummy Classifier (Baseline)
* Logistic Regression
* Decision Tree
* Tuned Decision Tree
* Random Forest

### Evaluation

Models were evaluated using:

* Accuracy
* Precision
* Recall
* Macro F1-Score
* Confusion Matrices

Logistic Regression was selected as the final model because it achieved the strongest overall balance across sentiment classes.

## Repository Navigation

### Jupyter Notebook

Contains the complete analysis, including data preparation, modeling, evaluation, and final conclusions.

**File:** `Twitter_Sentiment_Analysis.ipynb`

### Presentation

Contains a non-technical summary of the project, key findings, and recommendations.

**File:** `Presentation PDF.pdf`

### README

Provides an overview of the project and instructions for navigating the repository.

**File:** `README.md`

## Results

| Model               | Accuracy | Macro F1-Score |
| ------------------- | -------- | -------------- |
| Dummy Classifier    | 0.603    | 0.251          |
| Logistic Regression | 0.631    | 0.556          |
| Decision Tree       | 0.600    | 0.478          |
| Tuned Decision Tree | 0.618    | 0.426          |
| Random Forest       | 0.672    | 0.515          |

Although Random Forest achieved the highest accuracy, Logistic Regression produced the highest Macro F1-Score and was therefore selected as the final model.

## Sources

### Dataset

CrowdFlower Twitter Sentiment Dataset

https://data.world/crowdflower/brands-and-product-emotions

## Running the Project

1. Download the dataset from the source above.
2. Place the dataset in the `data` folder.
3. Open the Jupyter Notebook.
4. Run all cells from top to bottom.
5. Review the visualizations, model outputs, and conclusions.

## Future Improvements

* Incorporate more recent Twitter data
* Address class imbalance using advanced resampling techniques
* Explore transformer-based NLP models such as BERT
* Develop a real-time sentiment monitoring dashboard

## Author

Chris Mau Karagu

