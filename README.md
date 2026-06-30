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
