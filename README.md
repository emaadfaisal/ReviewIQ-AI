ReviewIQ AI
ReviewIQ AI is an AI-powered customer review intelligence platform. It uses Natural Language Processing and machine learning to analyze customer reviews, classify sentiment, identify recurring complaints, and provide useful business insights.

Project Type
Track A: Application Development

Problem
Businesses may receive thousands of customer reviews across e-commerce websites, surveys, and online platforms. Reading and analyzing these reviews manually is slow and difficult.

Ratings can show general satisfaction, but they do not always explain whether customers are discussing product quality, delivery, pricing, packaging, or customer service.

ReviewIQ AI aims to automatically process customer reviews and help businesses understand customer feedback.

Target Users
E-commerce businesses
Online product sellers
Customer experience teams
Product managers
Marketing teams
Current Features
The first deliverable includes:

Dataset acquisition from Hugging Face
Stratified sampling
Missing-value analysis
Duplicate review removal
Text preprocessing
Sentiment-label creation
Exploratory data analysis
TF-IDF feature extraction
Train, validation, and test preparation
Dataset
The project uses the SetFit Amazon Reviews Multi English dataset from Hugging Face.

The original dataset contains:

200,000 training reviews
5,000 validation reviews
5,000 testing reviews
A smaller working sample was selected:

30,000 training reviews
3,000 validation reviews
3,000 testing reviews
After cleaning and cross-split duplicate removal, the final dataset contains:

29,960 training reviews
2,992 validation reviews
2,990 testing reviews
35,942 total reviews
Sentiment Classes
The original five rating labels were converted into three sentiment classes:

Labels 0 and 1: Negative
Label 2: Neutral
Labels 3 and 4: Positive
Data Preprocessing
The preprocessing pipeline:

Checks missing review text and labels
Removes duplicate customer reviews
Converts review text to lowercase
Removes HTML tags and URLs
Removes unnecessary characters
Removes extra spaces
Calculates review word count
Removes repeated text across dataset splits
Converts review text into TF-IDF features
TF-IDF Results
The final feature matrix shapes are:

Training: (29,960, 10,000)
Validation: (2,992, 10,000)
Testing: (2,990, 10,000)
Technologies
Python
Google Colab
Hugging Face Datasets
Pandas
Scikit-learn
Matplotlib
Seaborn
LaTeX
Overleaf
Repository Structure
notebooks/: Google Colab notebook
data_scripts/: Dataset acquisition and preprocessing code
figures/: Exploratory data analysis charts
report/: Deliverable 1 LaTeX source and PDF
Future Work
The next stages will include:

Sentiment-classification model training
Model comparison and evaluation
Aspect detection
Recurring complaint identification
Business recommendations
Web application development
Author
Emaad Faisal
