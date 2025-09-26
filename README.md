# SentiCook

## Contents of the Repository

This repository contains scripts for sentiment analysis of recipe reviews using VADER sentiment analysis and machine learning models to examine the relationship between review text sentiment, star ratings, and upvotes. 

## Software and Platform

**Software:** Google Colab and Jupyter Notebooks

**Add-on packages:**
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- scipy
- vaderSentiment
- nltk

**Platform:** Windows and Mac

## Map of the Documentation

```
SentiCook/
├── DATA/
│   ├── original_data/
│   │   └── Recipe Reviews and User Feedback Dataset.csv
│   ├── final_data/
│   │   └── cleaned_recipe_reviews.csv
│   └── DataAppendix.pdf
├── SCRIPTS/
│   ├── 1_cleaning.ipynb
│   ├── 2_exploratory_plots.ipynb
│   └── 3_model.ipynb
├── OUTPUT/
│   ├── exploratory/
│   │   ├── f_distribution of star bins.jpg
│   │   ├── f_distribution of stars (original scale).jpg
│   │   ├── f_distribution of upvotes.jpg
│   │   ├── t_categorical summaries.jpg
│   │   ├── t_descriptive statistics.jpg
│   │   ├── t_helpful rate summary.jpg
│   │   ├── t_sentiment bin distribution.jpg
│   │   ├── t_star bin distribution.jpg
│   │   ├── t_star count and percentages.jpg
│   │   ├── t_thumbs up:down summary.jpg
│   │   └── t_total and net thumb votes.jpg
│   └── model visualizations/
│       ├── f_distribution of thumbs up count-alignment.jpg
│       ├── f_mean thumbs up count-alignment.jpg
│       ├── f_model1 ROC.jpg
│       ├── f_model1 confusion matrix.jpg
│       ├── f_model2 ROC.jpg
│       ├── f_model2 classification report.jpg
│       ├── f_model2 confusion matrix.jpg
│       ├── f_model3 ROC.jpg
│       ├── f_model3 confusion matrix.jpg
│       ├── t_AUC values for each class.jpg
│       ├── t_model1 classification report.jpg
│       ├── t_model3 classification report.jpg
│       ├── t_sentiment vs star bin.jpg
│       ├── t_summary of thumbs up for alignment.jpg
│       └── t_upvotes summary.jpg
├── LICENSE
└── README.md
```

## Instructions for Reproducing the Results

1. **Clone the repository:**
   ```bash
   git clone https://github.com/srujanay18/SentiCook.git
   cd SentiCook
   ```

2. **Install required packages:**
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn scipy vaderSentiment nltk
   ```

3. **Run the notebooks in order:**

   **Step 1: Data Cleaning**
   - Open `SCRIPTS/1_cleaning.ipynb` in Jupyter Notebook or upload to Google Colab
   - Execute all cells in order
   - This will clean the raw dataset and output `DATA/final_data/cleaned_recipe_reviews.csv`

   **Step 2: Exploratory Analysis**
   - Open `SCRIPTS/2_exploratory_plots.ipynb` in Jupyter Notebook or upload to Google Colab
   - Execute all cells in order
   - This will generate descriptive statistics and visualizations in `OUTPUT/exploratory/`

   **Step 3: Machine Learning Models**
   - Open `SCRIPTS/3_model.ipynb` in Jupyter Notebook or upload to Google Colab
   - Execute all cells in order
   - This will train sentiment analysis models and generate performance visualizations in `OUTPUT/model visualizations/`

**Note:** If using Google Colab, upload the dataset file `Recipe Reviews and User Feedback Dataset.csv` to the `/content/` directory before running the notebooks.
