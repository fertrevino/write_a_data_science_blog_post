# Stackoverflow 2017 survey results analysis
Stackoverflow.com, a cornerstone in most software developers' work, has released its survey [results for the year 2017](https://insights.stackoverflow.com/survey). With more than 50k respondents from around the world, it is worth analyzing the results. Which insights can we gain? Continue reading and find out! 

![Alt text](resources/stack_overflow_image_logo.png?raw=true "Stackoverflow survery logo")

## Introduction
Software development is becoming more popular every year and an increasingly amout of people want to start a career in this field. Those already working in software development are commonly curious about the global trends in this technology sector. Therefore, an analysis of the survey results is interesting for these two population gruops.

What can we learn from the results? After analyzing the meta data, I concluded that the following questions can be answered programatically using Python and the Cross-Industry Standard Process for Data Mining (CRISP-DM).

1. What are the most popular programming languages in different countries? 
2. What is the correlation between programming language, experience and salary?
3. What is the most popular occupation for the respondents?

Check out the Github [repository](https://github.com/fertrevino/write_a_data_science_blog_post) containing all the code used for this analysis. Feel free to post your comments and questions in there! Let us begin with the answers.

## What are the most popular programming languages in different countries? 
As a person who has lived in different countries, I tend to compare the culture of one place with the culture of another. Trends in software development are not the exception. Therefore I wonder, are programming languages the same popular in different countries? Let us find out!

The survey results from Stackoverflow include the country of origin for the respondents as well as languages with which they are familiar. We can therefore choose a desired country, count how many developers have worked with each programming language available and rank the results. An important consideration for this is that a respondent may be experienced in more than one programming language. This has been taken care in the code used for processing the data.

Three countries are of my interest: Germany, the United Kingdom and the United States. I chose the first two countries because I lived in them and the United States because it is a leading country in innnovation in the software industry.

The respondents in Germany mentioned to be experienced in the following programming languages, ranked by number of mentions.

![Alt text](resources/language_chart_Germany.png?raw=true "Most popular programing languages in Germany (2017)")

As we can see, the 2 most popular programming languages are JavaScript and Java. Interestingly, both start with the same 4 letters despite being unrelated to each other. That is certainly a sympatic coincidence. One runs commonly in browser applications while ther other is a versatile and multipurpose programming language. 

Let us have a look at what respondents in the United Kingdom mentioned by looking at the image below.

![Alt text](resources/language_chart_United_Kingdom.png?raw=true "Most popular programing languages in United Kingdom (2017)")

It seems that Java is not the second most popular programming language but SQL is. Does this mean that there are more database administrators in the United Kingdom? Perhaps. The programming language used to analyze this data, Python, is within the top 5 for both the United Kingdom and Germany. Let us have a look at the results from respondents in the United States with the image below.

![Alt text](resources/language_chart_United_States.png?raw=true "Most popular programing languages in United States (2017)")

Surprisingly, JavaScript wins again! Who would have thought. There seems to be a global boom in jobs requiring to develop code using this langauge. Please notice the increase in respondents for the United States. The most popular programming language in this country has more than 5000 thousand mentions. That is more than the mentions for JavaScript in Germany and the United Kingdom combined. This makes sense considering that Stackoverflow is a website with content in English and because the United States is the hub for software development.

We can observe that the 3 countries have a similar trend regarding the most popular programming languages. Javascript is unquestionably the most used language. If we analyze the top 6 most popular languages, we realize that each country has the same programming languages at the top. However, we can see a small variation in the order in which these languages appear. For instance, SQL ranks third in Germany while it it is second in both the United States and the United Kingdom.

Based on the results of these questions, it is reasonable to assume that trends in popular programming languages are global.

## What is the correlation between programming language, experience and salary?
We have already seen that the popularity of programming languages is similar around the world. Another question worth investiating is knowing the relationship between programming language, experience, and salary.he 

It is expected, that experience is correlated with salary. The more experienced a developer is, the higher the salary. However, is this a linear relationship or is it a corrlation? Do all programming languages pay equally? Let us find out.

For this analysis, we have looked two additional pieces of data from the survey: years of experience coding and salary. We combined these two pieces of information with the programming language declared in the previous question, but this time for all countries. The results of this data processing are shown in the following chart.

![Alt text](resources/mean_salary_popular_language_for_experience.png?raw=true "Salary as function of experience for popular programming languages (2017)")

We can confirm with the graph above that salary is *correlated* with experience. It is only correlated since the relation is not entirely linear. As we can see, some programmers with less experience have a higher salary than some more experienced colleagues. This can be due to new emerging frameworks and tools based on a particular language which are more in demand in 2017 and younger developers are mor familiar with. Assuming this is the case, it is understandable that trendy frameworks offer a high salary for less experienced developers if there is a shortage of people with those skills.

Regarding the programming langauges we see again a correlation. From the popular languages, PHP tends to have the lowest salary regardless of the programming experience. On the other hand, we can see that Python tends to have the highest salary at any point across the years of experience. This would imply that Python developers, regardless of their experience, were in high demand in 2017. The rest of the programming languages (Java, SQL, JavaScript and C#) show a similar salary variation with respect to experience.

## What is the most popular occupation for the respondents?
Software development itself is a wide industry. There are game developers, embedded system programmers, smarthphone application developers and data scientists, just to name a few. Therefore, it is interesting to know what are the most popular occupations of the survey respondents.

To achieve these, the question regarding the *developer type* in the survey has been considered. The following bar plot show the results of this analysis.

![Alt text](resources/developer_types.png?raw=true "Most common developer types (2017)")

By far, web developer is the most common occupation in the survey. Surprisignly, desktop application developers won the second place while mobile developers got the third place. Who would have thought that mobile developers have not yet surpassed desktop develoopers? Awesome!

An additional observation is that there are more database administrators than system administrators. Would this me correlated with the popularity of SQL in the previous question? Maybe!

An important remark here is data scientist. Despite being a new area, there are more respondents with this occupation than other older occupations such as graphics programming, grafic designer and quality assurance. Surprising! Machine learning specialist is not so common in this survey. It is a sure bet to say that machine learning specialists occupations will be more common in the next years!

## Conclusions
Data science can help us understand collected data, which at first sight might seem astract and as a colleciton of values. An ordered and standarized analysis of the data, such as by following CRISP-DM, can throw meaningful insights to people interested in taking a decision. Such people can be a stakeholder in a company or an individual looking into choosing a career. Therefore, a proper understanding of the data collected, the background of the business and the necessary software techonlogy is essential in today's world. Without a doubt, data science is hardcoded deep into the society of the future.
