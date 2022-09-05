python version = 3.8.3

install requirements from requirements.txt

Files & Notebooks
------------------
* data_cleaning.ipynb:
    - solution for data preparation:
        - Trim and clean the text of special characters
	    - Using breaks, commas or spaces, attempt to separate the annotations into individual skills
* data_preparation.ipynb:
    - requires: resume_data.pkl created using data_cleaning.ipynb
    - data preparation, preprocessing for grouping the resumes
    - features used: skills, designation, degree
    - preprocessing steps: uniform lowercase, remove special characters, stopwords, lemmatize.
* class_model.ipynb:
    - requires: resume_data.pkl created using data_preparation.ipynb
    - groups and scores the resumes in the categories: testing, development and management.
    - Outputs a table of the index of the resume and the three values for testing, development and management.
    - uses latent dirichlet allocation for topic modelling and count vectorizer for vectorization.
    - Visualize groups using wordcloud.
* result.csv
    - output table of the index of the resume and the three values for testing, development and management.
* requirements.txt
    - python libraries requirement

Use model on test/holdout data:
-------------------------------
* run data_cleaning.ipynb, data_preparation
* save models as shown in section "save models" in class_model.ipynb
* Follow sample under section "Run on holdout data" in class_model.ipynb
