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

- ## Day 12 Progress

- Implemented GroupKFold cross-validation grouped by `job_id`.
- Trained a baseline Random Forest Regressor to predict `match_relevance_score`.
- Evaluated model performance using Mean Absolute Error (MAE).
- Analyzed feature importance for the engineered feature set.
- Uploaded the Day 12 notebook (`Day12_ZiroProject.ipynb`) to the repository.

- ## Day 13 Progress

- Implemented an XGBoost baseline model for predicting the engineered match relevance score.
- Performed hyperparameter tuning using different learning rates and tree depths.
- Evaluated model performance using Mean Absolute Error (MAE).
- Analyzed feature importance generated by the XGBoost model.
- Uploaded the Day 13 notebook (`Day13_ZiroProject.ipynb`) to the repository.

- ## Day 14 Progress

- Evaluated the recommendation pipeline using ranking-based metrics.
- Calculated Precision@5 and Precision@10 for top-ranked candidates.
- Performed an adapted NDCG@5 and NDCG@10 evaluation using engineered relevance scores.
- Visualized Precision@K results and summarized overall model performance.
- Uploaded the Day 14 notebook (`Day14_ZiroProject.ipynb`) to the repository.

- Day 15 Progress
Connected the RecruitSmart datasets to Power BI Desktop.
Imported the cleaned job and feature datasets for dashboard development.
Created KPI cards to display Total Jobs, Total Candidates, Average Skills, and Average Match Score.
Designed recruiter-focused visualizations including Department, Employment Type, Experience Level, Salary Distribution, and Top Matching Job Titles.
Uploaded the Day 15 Power BI dashboard and related project files to the repository.

- Day 16 Progress
Enhanced the RecruitSmart dashboard by adding an Average Time-to-Shortlist KPI.
Created interactive slicers for Experience Level and Skill Cluster filtering.
Built a Match Score Distribution visualization for recruiter analysis.
Verified dashboard interactivity and ensured filters updated all visuals correctly.
Uploaded the Day 16 notebook (Day16_ZiroProject.ipynb) to the repository.

- Day 17 Progress
Reviewed and validated the RecruitSmart Power BI dashboard for consistency.
Verified KPI values, charts, and slicers against the processed datasets and model outputs.
Confirmed the dashboard was ready for project documentation and portfolio inclusion.
Finalized the dashboard for presentation and deployment preparation.
Uploaded the finalized dashboard files and documentation updates to the repository.

- Day 18 Progress
Developed the initial FastAPI application structure for the RecruitSmart project.
Created a Pydantic model to validate incoming JSON resume data.
Built a preprocessing class to standardize resume information before prediction.
Implemented the /predict endpoint to return candidate match ranking results.
Uploaded the Day 18 notebook (Day18_API.ipynb) to the repository.
