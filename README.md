# Salary-Dataset-Project
Perform data analysis on the Salary Dataset
----------------------------------------------------------------

> Context

This Salary Dataset is Data that contains Job Salaries for Data Science jobs in various countries.

> Content

This dataset contains information as follows :
1. **work_year** : The year during which the salary was paid.
2. **experience_level** : The experience level in the job during the year with the following possible values:
    
     a. EN : Entry-level / Junior 
    
     b. MI : Mid-level / Intermediate
    
     c. SE : Senior-level / Expert
    
     d. EX : Executive-level / Director
3. **employment_type** : The type of employement for the role:

    a. PT (Part-time)

    b. FT (Full-time)

    c. CT (Contract)

    d. FL (Freelance)
4. **job_title** : The role worked in during the year.
5. **salary** : The total gross salary amount paid.
6. **salary_currency** : The currency of the salary paid as an ISO 4217 currency code.
7. **salary_in_usd** : The salary in USD (FX rate divided by avg. USD rate for the respective year via fxdata.foorilla.com).
8. **employee_residence** : Employee's primary country of residence in during the work year as an ISO 3166 country code.
9. **remote_ratio** : The overall amount of work done remotely, possible values are as follows:

    a. 0 - No remote work (less than 20%)

    b. 50 - Partially remote

    c. 100 - Fully remote (more than 80%)
10. **company_location** : The country of the employer's main office or contracting branch as an ISO 3166 country code.
11. **company_size** : The average number of people that worked for the company during the year:

    a. S : less than 50 employees (small)

    b. M : 50 to 250 employees (medium)

    c. L : more than 250 employees (large)

-- Taken from [kaggle.com by SAURABH SHAHANE](https://www.kaggle.com/datasets/saurabhshahane/data-science-jobs-salaries) --

-----------------------------------------------------------------------------------

I took this project from the study case assignment Mini Course Data Analytics Revou in the batch from July 25 to August 5, 2022

This Salary Dataset Project uses various tools, namely :
1. **Python with Google Colab** to *view data and perform data cleaning* before data is used,
2. **Google BigQuery** to *create queries from datasets* so that they are ready for further visualization, and
3. **GDS or Google Data Studio** to *perform Data Visualization*.

The following is a description of the file used :
1. The original dataset is on **salary_dataset.csv** file.
2. Cleaning data using python as in the **datacleaning_salary.py** file.
3. Same as using python regarding the data exploration steps, only the file extension is different, where the file **datacleaning_salary.ipynb** can be used for Jupyter Notebook.
4. The dataset that has been done Data Cleaning is in the **salary-dataset.csv** file.
5. SQL query file that will be used for data visualization is contained in the **query.sql** file.
6. The file with the Power Point extension (**ASSIGNMENT4.pptx**) contains the steps and the results of the work that has been done.
7. The file with the Portable Document Format (PDF) extension (**ASSIGNMENT4.pdf**) contains the steps and the results of the work same as the PPT file, that has been done.

The steps for Data Cleaning are as follows :
1. Change data type 
2. Remove duplicated data : from 607 data to 562 data, where there are 45 duplicate data, which is 7.41% of the total data.
3. Remove empty data 
4. Remove outliers : Delete data that has a value that exceeds the upper and lower limits (data outliers) in the ‘salary_in_usd' column, so that the total data becomes 552.
5. Remove unnecessary data

-- THANK YOU [@damalialutfiani](https://www.linkedin.com/in/damalialutfiani/) --
