# Salary Prediction project
# Description of the project
This project examines job posting salaries based on existing dataset, and make prediction for salaries of new job postings. An estimation of salary range across different industries offers job seekers guidance in their application for their desired jobs; the HR department can use these prediction in their construction of business processes for the job posting.
# Datasets
train_features.csv - Each observation represents an individual's job posting; each column represents unqiue information about this applicant and the job applied to. This dataset is meant to be used in training models.

test_features.csv - Each observation represents an individual's job posting; each column represents unqiue information about this applicant and the job applied to. This dataset is meant to be used for evaluating models trained on train_features.csv.

train_salaries.csv - Each observation represents an individual's salary corresponding to their job posting in train_features.csv.

Features:

* jobId - the id of the job posting (unique)
* companyId - the id of the company posting the job (unique)
* jobType - the type of the job (e.g. CEO, CFO, senior, etc)
* degree - the highest degree obtained by the applicant (e.g. DOCTORAL, MASTERS, BACHELOR, etc)
* major - the major of this applicant in college (e.g. business, math, etc)
* industry - the industry this job belongs to (e.g. oil, finance, tech, etc)
* yearsExperience - years of experience required
* milesFromMetropolis - distance away from the metropolis in miles
* salary - the salary of the job posting

# Feature Summary
# jobType
<img src='Salary prediction project/images/salary_by_degree.png'>
Higher level jobs have high average salary.

# Degree
<img src='Salary prediction project/images/salary_by_degree.png'>
The educational background is directly propotion to the average salary.

# Major
<img src="Salary prediction project/images/salary_by_major.png">
More technical majors tend to have higher average salary.

# Industry
<img src='Salary prediction project/images/salary_by_industry.png'>
Industries like oil and finance have higher average salary, which makes sense since these industries are known to pay well even at an entry level position.

# Salary
<img src='Salary prediction project/images/salary_distribution.png'>
Salary is approximately normally distributed. Basically all but a few salary are under 200k/year.

# Feature correlation
<img src='Salary prediction project/images/correlation_matrix_heatmap.png'>
Job type, degree, major, industry, and years of experience all have positive correlation with salary. Distance from the metropolis has negative correlation with salary. Degree, major and job type have relatively strong positive correlation with each other.

# Training Models
Three models are Tested:

* Linear Regression ---> MSE=384.5
* Random Forest ---> MSE=388.7
* Grandient Boosting ---> MSE=361.4

The best model with lowest mean square error is the Gradient Boosting Regressor.
<img src='Salary prediction project/images/model_evaluations.png'>


# Solution
The predicted salaries for job postings based on the Gradient Boosting model on the training set:
<img src='Salary prediction project/images/predicted_solution.png'>




