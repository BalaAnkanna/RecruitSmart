## Project Overview
RecruitSmart is an AI-powered talent-to-role ranking system that helps recruiters automatically rank candidates based on their suitability for a job.

## Objective
- Automate resume screening
- Rank candidates based on skills and experience
- Reduce recruiter screening time

## Technologies Used
- Python
- Pandas
- NumPy
- Jupyter Notebook
- SQL (Upcoming)
- XGBoost (Upcoming)
- FastAPI (Upcoming)
- Power BI (Upcoming)

## Project Progress

### Day 1
- Read project blueprint
- Confirmed dataset sources
- Created GitHub repository
- Set up project folder structure

### Day 2
- Downloaded Kaggle datasets
- Loaded all datasets into Jupyter Notebook
- Inspected dataset structure
- Performed initial data audit
- Identified missing values

## Day 3 Progress
- Created the Applications bridge table.
- Handled missing experience values.
- Applied text preprocessing to job descriptions and requirements.
- Saved cleaned datasets for feature engineering.

## Day 4 Progress

- Created a SQLite database (`RecruitSmart.db`) for the project.
- Imported the Jobs, Candidates, Applications, PersonSkills, and Skills datasets into SQL tables.
- Verified that all tables were created successfully.
- Created the `JobCandidateView` SQL View by joining Jobs, Candidates, and Applications tables.
- Queried the SQL View to validate the relationships between jobs and candidates.
- Uploaded the Day 4 notebook (`Day4_ZiroProject.ipynb`) to the repository.

- ## Day 5 Progress

- Created SQL queries to count candidate skills from the PersonSkills table.
- Generated numerical experience scores using SQL CASE statements.
- Performed duplicate record checks for Candidates and Applications tables.
- Prepared SQL-based features for the RecruitSmart recommendation engine.
- Uploaded the Day 5 notebook (`Day5_ZiroProject.ipynb`) to the repository.

## Day 6 Progress

- Normalized experience levels using SQL CASE statements.
- Extracted certifications and technical tools from job requirements using SQL pattern matching.
- Analyzed job title frequencies to identify high-volume and niche job postings.
- Prepared additional SQL-based features for the RecruitSmart recommendation engine.
- Uploaded the Day 6 notebook (`Day6_ZiroProject.ipynb`) to the repository.

## Day 7 Progress

- Generated the `match_relevance_score` target variable for machine learning.
- Created a flattened feature matrix by joining Jobs, Candidates, and Applications tables.
- Merged target scores into the feature matrix.
- Exported the final modeling dataset (`flattened_feature_matrix.csv`).
- Validated the distribution of target scores across job postings.
- Uploaded the Day 7 notebook (`Day7_ZiroProject.ipynb`) to the repository.

## Day 8 Progress

- Performed exploratory data analysis (EDA) on job descriptions and requirements.
- Generated word frequency distributions after removing stop words.
- Processed salary ranges into average salary values and compared Python-related jobs with other roles.
- Validated the distribution of the generated `match_relevance_score` target variable.
- Uploaded the Day 8 notebook (`Day8_ZiroProject.ipynb`) to the repository.

## Day 9 Progress

- Completed Exploratory Data Analysis (EDA) on required experience levels.
- Visualized the distribution of experience categories.
- Performed outlier detection on the generated match relevance scores using the IQR method.
- Finalized and exported the feature set (`final_feature_set.csv`) for the NLP pipeline.
- Uploaded the Day 9 notebook to the repository.

## Day 10 Progress

- Initialized the spaCy NLP pipeline for Named Entity Recognition (NER).
- Built a TF-IDF vectorizer to convert job descriptions into numerical feature vectors.
- Generated a TF-IDF matrix with 17,880 job postings and 500 text features.
- Calculated cosine similarity scores to measure text similarity between job descriptions.
- Uploaded the Day 10 notebook (`Day10_ZiroProject.ipynb`) to the repository.

- ## Day 11 Progress

- Implemented HuggingFace Sentence-Transformers (all-MiniLM-L6-v2) for semantic text embeddings.
- Generated contextual embeddings for job descriptions and requirements.
- Calculated semantic similarity using cosine similarity.
- Compared BERT-based semantic similarity with the TF-IDF baseline.
- Exported generated embeddings (`bert_embeddings.csv`) for future machine learning tasks.
- Uploaded the Day 11 notebook (`Day11_ZiroProject.ipynb`) to the repository.
