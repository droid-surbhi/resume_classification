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
    
