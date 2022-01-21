# Thinkful Data Science Flex Course
# Supervised Learning Capstone Project: Predicting Popularity of Mashable News Articles

**Project Description**

- Developed supervised learning models to predict the popularity of Mashable news articles by using a large number of article properties as the features and a binary class split for the number of social media shares as the target outcome.
- Compared performance of four model types: logistic regression, decision tree, random forest, and kernel support vector machine.
-	Built models using Python, pandas, and scikit-learn in a Jupyter notebook.

**Source Data**

The dataset was obtained from [Kaggle](https://www.kaggle.com/yamqwe/predicting-number-of-shares-of-news-articles), but originally comes from this research project:
- Fernandes et al., 2015. A Proactive Intelligent Decision Support System for Predicting the Popularity of Online News [PDF](https://github.com/JosephMartin610/thinkful_data_science_flex_capstone_news_shares/blob/main/Fernandes_et_al_2015.pdf).
- The research article was consulted for information about the dataset.
- The dataset was created by retrieving content of all articles published on Mashable from January 7, 2013 to January 7, 2015.


- 

The data used for this project are a random subset of blogs, news, and tweet items (350,000 items) used to build a catalog of n-grams (sentence fragment of n words; n = 1:5) and their occurrence counts. The source blogs, news, and tweet data can be obtained [here](https://d396qusza40orc.cloudfront.net/dsscapstone/dataset/Coursera-SwiftKey.zip). The source data files and intermediate data files are too large to be stored on GitHub, so to make use of this, please repeat all steps in R.

**Jupyter Notebook**

The order in which to run the R scripts is as follows:
- read_corpora_scr.R (calls read_corpora.R)
- tknz_scr.R (calls rmv_pf.R and tokenize.R)
- make_ngrams_scr.R (calls make_ngrams_from_tokens.R)
- good_turing_disc_scr.R (calls simple_good_turing.R)
- merge_ns_ngrams_counts_for_model_gtd.R
- model_test_scr.R (calls pred_text_ngrams_kbo_gtd.R which calls model_ngrams_kbo_gtd.R)
- app.R to run Shiny app (calls pred_text_ngrams_kbo_gtd.R which calls model_ngrams_kbo_gtd.R)

**Presentation**

Results are described here: The capstone presentation is [here](https://htmlpreview.github.io/?https://github.com/JosephMartin610/coursera_data_science_capstone_bated_breath_word_generator/blob/main/word_generator_presentation-rpubs.html). It has information about model basis and performance.
