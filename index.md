## Stackoverflow 2017 survey results analysis

Stackoverflow.com, a cornerstone in most software developers' work, has released its survey [results for the year 2017](https://insights.stackoverflow.com/survey). With more than 50k respondents from around the world, it is worth analyzing the results. Which insights can we gain? Continue reading and find out! 

![Alt text](resources/stack_overflow_image_logo.png?raw=true "Stackoverflow survery logo")

### Introduction
Software development is becoming more popular every year. More and more people are interested in starting a career in this field. Others who are already working in this field, are curious about the global trends in this technology sector. Hence the Stackoverflow survey results are of interest for newcomers and expereinced programmers.

What can we learn? After a meta analysis of the results, I have concluded that the following questions can be answered by analyzing the data programatically. Check out the Github [repository](https://github.com/fertrevino/write_a_data_science_blog_post) containing all the code used for this analysis.

In this post, we will answer the following questions using the Cross-Industry Standard Process for Data Mining (CRISP-DM).

1. What are the most popular programming languages in different countries? 
2. What is the correlation between programming language, experience and salary?
3. What is the most popular occupation for the respondents?

We can observe that the 3 countries have a similar trend regarding the most popular programming languages. Javascript is unquestionably the most used language. If we analyze the top 6 most popular languages, we realize that each country has the same programming languages at the top. However, we can see a small variation in the order in which these languages appear. For instance, SQL ranks third in Germany while it it is second in both the United States and the United Kingdom.

Based on the results of these questions, it is reasonable to assume that trends in popular programming languages are global.

### What are the most popular programming languages in different countries? 
As a person who has lived in different countries, I tend to compare the culture of one place with another. Work culture and trends are no the exception for this. Therefore I wonder, are the programming language the same popular in different countries? Let us find out!

The survey results from Stackoverflow include the country of origin for the respondents as well as languages with which they are familiar. We can therefore choose a desired country, count how many developers have worked with each programming language available and rank the results. An important consideration for this is, that a respondent may be experienced in more than one programming language, which has been taken care for this data processing.

There are 3 countries which interest me: Germany, United States and the United Kingdom. The reason for choosing Germany and the United Kingdom is because I have lived in those countries, while the United States is a suitable option since it is a country with leading innnovation in the software industry.

The following three images show the results for these countries.

![Alt text](resources/language_chart_Germany.png?raw=true "Most popular programing languages in Germany (2017)")

![Alt text](resources/language_chart_United_Kingdom.png?raw=true "Most popular programing languages in United Kingdom (2017)")

![Alt text](resources/language_chart_United_States.png?raw=true "Most popular programing languages in United States (2017)")


### What is the correlation between programming language, experience and salary?
We have already seen that the popularity of programming languages is similar around the world. Another question worth investiating is knowing the relationship between programming language, experience, and salary.

It is expected, that experience is correlated with salary. The more experienced a developer is, the higher the salary. However, is this a linear relationship or is it a corrlation? Do all programming languages pay equally? Let us find out.

For this analysis, we have looked two additional pieces of data from the survey: years of experience coding and salary. We combined these two pieces of information with the programming language declared in the previous question, but this time for all countries. The results of this data processing are shown in the following chart.


![Alt text](resources/mean_salary_popular_language_for_experience.png?raw=true "Salary as function of experience for popular programming languages (2017)")

We can confirm with the graph above that salary is *correlated* with experience. It is only correlated since the relation is not entirely linear. As we can see, some programmers with less experience have a higher salary than some more experienced colleagues. This can be due to new emerging frameworks and tools based on a particular language which are more in demand in 2017 and younger developers are mor familiar with. Assuming this is the case, it is understandable that trendy frameworks offer a high salary for less experienced developers if there is a shortage of people with those skills.

Regarding the programming langauges we see again a correlation. From the popular languages, PHP tends to have the lowest salary regardless of the programming experience. On the other hand, we can see that Python tends to have the highest salary at any point across the years of experience. This would imply that Python developers, regardless of their experience, were in high demand in 2017. The rest of the programming languages (Java, SQL, JavaScript and C#) show a similar salary variation with respect to experience.


### What is the most popular occupation for the respondents?
Software development itself is a wide industry. There are game developers, embedded system programmers, smarthphone application developers and data scientists, just to name a few. Therefore, it is interesting to know what are the most popular occupations of the survey respondents.

To achieve these, the question regarding the *developer type* in the survey has been considered. The following bar plot show the results of this analysis.

![Alt text](resources/developer_types.png?raw=true "Most common developer types (2017)")

By far, web developer is the most common occupation in the survey. Surprisignly, desktop application developers won the second place while mobile developers got the third place. Who would have thought that mobile developers have not yet surpassed desktop develoopers? Awesome!

An additional observation is that there are more database administrators than system administrators. Would this me correlated with the popularity of SQL in the previous question? Maybe!

An important remark here is data scientist. Despite being a new area, there are more respondents with this occupation than other older occupations such as graphics programming, grafic designer and quality assurance. Surprising! Machine learning specialist is not so common in this survey. It is a sure bet to say that machine learning specialists occupations will be more common in the next years!


### Conclusions



```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/fertrevino/github_page/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
