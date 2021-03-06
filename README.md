# Introduction
This repository contains an in depth analysis of the Stackoverflow 2017 survey results from a data science perspective. The three business questions to be answered are:
* Which are the most popular programming languages in different countries?
* What is the correlation between experience and salary for the most popular programming languages?
* What is the most popular occupation for the respondents?

The dataset used for this project can be found [here](https://insights.stackoverflow.com/survey)

Visit the [blog post](https://fertrevino.github.io/write_a_data_science_blog_post/) dedicated to the results obtained by this repository.

# Installation
You can download this repository with the following command:
```Shell
git clone git@github.com:fertrevino/write_a_data_science_blog_post.git
```

In order to start the Jupyter notebook, you can run:
```Shell
jupyter-notebook <your-path>/write_a_data_science_blog_pos/analysis_data_stackoverflow.ipynb
```

# Motivation
This project is part of the Udacity Nanodegree program.

# File(s) description
This repository contains an HTML and a Jupyter notebook version of the code:
* analysis_data_stackoverflow.ipynb
* analysis_data_stackoverflow.html

The original files from the Stackoverflow survey results:
* survey_results_schema.csv
* survey_results_public.csv
* stack-overflow-developer-survey-2017.zip

A folder with the images generated by the code:
* resources

# Results
## Which are the most popular programming languages in different countries?
![Alt text](resources/language_chart_Germany.png?raw=true "Most popular programing languages in Germany (2017)")
![Alt text](resources/language_chart_United_Kingdom.png?raw=true "Most popular programing languages in United Kingdom (2017)")
![Alt text](resources/language_chart_United_States.png?raw=true "Most popular programing languages in United States (2017)")

There seems to be a global boom in jobs requiring to develop code with JavaScript. An interesting observation is the increase in the number of respondents in the United States. The most popular programming language, JavaScript, has more than 5000 thousand mentions. That is more mentinos than those for JavaScript in Germany and the United Kingdom combined. This makes sense considering that Stackoverflow is a english speaking website and that the United States is the hub for software development.

We can observe that the 3 countries have a similar trend regarding the most popular programming languages. Javascript is unquestionably the most used language. If we analyze the top 6 most popular languages, we realize that the three countires have the same at the top. However, we can see a variation in the order in which these languages appear. For instance, SQL ranks third in Germany while it it is second in both the United States and the United Kingdom. Based on these results, it is reasonable to assume that trends in popular programming languages are global.

## What is the correlation between experience and salary for the most popular programming languages?
![Alt text](resources/mean_salary_popular_language_for_experience.png?raw=true "Salary as function of experience for popular programming languages (2017)")

Looking at the graph above, we can confirm that salary is correlated with experience. It is only correlated since the relation is not entirely linear. As we can see, some programmers with less experience have a higher salary than some more experienced colleagues. This can be due to new emerging frameworks and tools based on a particular language which are more in demand in the year 2017 and which younger developers are more familiar with. Assuming this is the case, it is understandable that trendy frameworks offer a high salary for less experienced developers if there is a shortage of people with those skills.

## What is the most popular occupation for the respondents?
![Alt text](resources/developer_types.png?raw=true "Most common developer types (2017)")

By far, web developer is the most common occupation in the survey. Surprisignly, desktop application developers won the second place while mobile developers got the third place. The fact that web developer is the most common occupation makes sense considering that JavaScript was the most popular programming language as seen in the resutls of question one.

An additional observation is that there are more database administrators than system administrators. This could be correlated with the popularity of SQL in the previous question.

An important remark here is data scientist. Despite being a new area, there are more respondents with this occupation than other older occupations such as graphics programming, grafic designer and quality assurance. Machine learning specialist is not so common in this survey. However, it is very probable that this will change in the next years.

# Aknowgledgements
The dataset used for this project has been obtained from Stackoverflow and it can be found [here](https://insights.stackoverflow.com/survey)



