# Gender-College-and-Earnings
Data visualization in R

**Please find my findings and full work of this data [Swintabel@io](https://swintabel.github.io/Gender-College-and-Earnings/GCE.html)**

#### MOTIVATION

The relevance of employment is really earnings. Simple macro economics says that, higher incomes reflect in higher consumption and higher demand leading to high overall motivation for increased production which facilitates development. This is the reasons why employment is a sensitive topic in relation to developemnt and the more reason I want to dedicate this project to exploring an interesting topic of the relationship that exists amongst earnings, gender and college courses. 

Some researchers say that the low earnings of graduates are as a result of poor choices of college courses, there are others who have also said that gender is major determining factor of earnings.

In this project, I will be exploring the relationship that exists amongst college majors, an individual's gender and earnings with a dataset generated from some college graduates between 2010 and 2012. The dataset I would be using can be found at [kaggle](https://www.kaggle.com/samaxtech/college-earnings-by-major).


#### DATASET

The dataset I would be using for this project is called  recent-grad.csv. As mentioned above, I retrieved it from Kaggle. According to another [kernel](https://www.kaggle.com/suugaku/dataquest-visualizing-earnings-by-college-major), the data was initially collected and aggregated by the [AMERICAN COMMUNITY SURVEY (ACS)](https://www.census.gov/programs-surveys/acs/data/pums.html). The current version of the data I will be using was extracted from the original data by [fiftythirtytwo](https://github.com/fivethirtyeight/data/tree/master/college-majors).

There are detailed discriptions of the dataset parameters at [fiftythirtytwo](https://github.com/fivethirtyeight/data/tree/master/college-majors)


![](https://github.com/Swintabel/Gender-College-and-Earnings/blob/master/desc.jpg.JPG?raw=true)


#### ORIGINAL PROBLEM AND QUESTIONS OF INQUIRY 

The original reason for this version of the dataset was the story; [The Economic Guide To Picking A College Major](https://fivethirtyeight.com/features/the-economic-guide-to-picking-a-college-major/). The major points made by this story was the fact that some Engineering and science courses are the courses that pay on the job market. However, majority of students offer courses that are not as rewarding in terms of earnings and jobs like Psychology and other social sciences. Likewise, some reseachers also say that the jobs that primarily employ men tend to pay more than the jobs that primarily employ women; Also, One year after graduation, a pay gap exists between women and men who majored in the same field (Christianne & Catherine, 2012, pp.2). Many college majors that lead to high-paying roles in tech and engineering are male dominated, while majors that lead to lower-paying roles in social sciences and liberal arts tend to be female-dominated, placing men in higher-paying career pathways, on average (Andrew & Jyotsna, 2017,pp.2).

These conclusions by these researchers have propelled me to explore this dataset to have a view into the relationships that exist amongst college courses, gender and earnings. In particular, I am curious to find some answers to the following questions:

1. What relationship exists between gender share of a college course and potential earnings?

2. What relationship exists between college courses and earnings?

3. What relationship exists between gender and college courses?

4. How much does gender and college course together determine earnings?


#### **SCOPE OF SOLUTION**

To help me find solutions to my above stated questions, I would be using GGPLOT2 for visualization.

I may not need certain variables in the dataset and hence, they would be silent variables in my analysis.  

I will first explore a one-to-one relatioships between my variables of interest and then look out for any interractions therein.

For every visualization i would explain the story told and see if it supports previous research on the topic and then, what i can make of the story.

In the concluding part of my visualization, i will put together my findings and recommend other projects worth exploring in this data.

Lastly, since my focus here is visualization, I would not be showing any preliminary data cleaning that i would be doing.



### **VISUALIZATION OF DATA**

#### **GENDER AND EARNINGS**

There are no questions when it comes to the importance of education for both men and women. In fact an old adage has said that, 'if you educate a man, you educate one person; But if you educate a woman, you educate a whole nation'. It is no wonder therefore that the girl-child education mantra seem never to die out.

However, the issue of the big pay gaps that exist between men and women of equal qualifications is a problem that hunts most women looking to further their education. Is it worth it? Will it change my standard of living any significantly? In africa where jobs are hard to find in the first place, these questions lead most women to give up on education even at the basic level.

As stated by a similar study, among federal financial aid recipients who attended public and private nonprofit four-year colleges, are no longer enrolled, and are working, average women's earnings 10 years after they first enrolled are lower than average men's earnings six years after first enrolling.(Antoinette Flores, 2016)

From the diagram below, it is seen that as the percentage of women majoring in a particular course increases, the median earning of year round employees also fall. That is, there is a negative relationship between earnings and the share of women in a college course.

More like, if women want the earnings of a particular profession to fall, all they have to do is to enroll more into the corresponding college course and enter the job market!

It is also noticed from the diagram that, as the share of women drops, the occurences of outrageous salaries also become more ubiquitous.

![](https://github.com/Swintabel/Gender-College-and-Earnings/blob/master/Rplot1.jpeg?raw=true)

#### **COLLEGE MAJORS AND EARNING**

The dream of most parents around the world is to see their children get good education and eventually, it becomes the dream of most teenagers after high school to enter into college and read their dream courses.

However, most young people graduate from college to the hard reality that,'not all glitters are gold'. While some careers seem very rewarding, others are not so much rewarding. This is not to downplay the essence of education but to emphasize the need to critically examine what career path to take when choosing a college course.

According to some researchers, women tend to enroll in graduate fields with lower economic returns than those chosen by men. In 2014, women enrolling in graduate school were significantly overrepresented in lower-earning fields-including public administration, health sciences, and education fields-encompassing roughly 75 percent or more of all enrollments. In contrast, women were significantly underrepresented in higher-earning fields, such as engineering, math, business, and computer sciences.(Antoinette Flores, 2016)

Hence, it is worth inquiring from the data;
**What relationship exists between college courses and earnings?** 

![](https://github.com/Swintabel/Gender-College-and-Earnings/blob/master/Rplot2.jpeg?raw=true)

From the figure above, it is noticed that the major with the highest median earnings is Engineering and the lowest is Psychology and Social work. Computers & Mathematics as well as Business also do pay well and they are followed by Social Science, Biology and Law. The likes of Arts, Humanities& liberal Arts and Education find themselves on the lower side.

This leads to the question of whether or not it is simply an issue of demand and supply. What if certain courses pay more because there very few people with these qualifications.

Thus, **What relationship exists between gender and college courses?**



#### **COLLEGE MAJORS AND GENDER**

From the initial infromation given by the above diagram, the courses that pay most are engineering, Computer Science and Mathematics. These courses are mostly known to be 'Men Courses'. According to an article published by the Harvard Business Review, Jobs that are unconsciously coded male have more prestige and pay than jobs that are coded female (Sarah Green Carmichael, 2017).

At this stage, I would like to know what the data say about 'Male courses' and 'Female courses'

![](https://github.com/Swintabel/Gender-College-and-Earnings/blob/master/Rplot3.jpeg?raw=true)

**IS IT A QUESTION OF DEMAND AND SUPPLY?**

From the diagram, the most noticable bar is that of the number of women in Psychology & Social Work compared to men. So then, can we say it is a matter of gender? There is also an equally competitive argument of total number of people majoring this course. The graph make it clear that they are generally higher that any other major. So it could be because of high labor supply exceeding demand for this type of labour.

However, let's consider a major like interdisciplinary. It appears to have the lowest number of people with such a qualification but also has more than 50% of the people being females.Even with these few majors, it is the forth lowest in terms of earnings from 'figure 2'. Is it a matter of skills relevance to the world?

I would say health is a very relevant field and therefore should pay better based on its merits. However, it pays just as low as Industrial Arts & Industrial Services as shown in 'figure 2'. Interestingly, it is almost totally dominated by women. Is it a matter of relevance to industries?

Engineering although does not have a very high number of majors, it is not very low in numbers either. This is same for Computers and Mathematics but they pay very high and they account for the outrageous pays seen in 'Figure 1'. Interestingly, they are highly male dominated.

![](https://github.com/Swintabel/Gender-College-and-Earnings/blob/master/Rplot4.jpeg?raw=true)

It is also worth noting from 'figure 4' that this data set has more women that men counts. This re-emphisize how male-dominated engineering and computers & Mathematics are.

**How much does gender and college course together determine earnings?**

#### **GENDER, COLLEGE MAJOR AND EARNINGS**

When it comes to the interaction of the three variables, the interesting trend here is that, for any two majors with compratively equal number of majors, if the women exceed the men in one than the other, then the median pay becomes lesser. For instance, 'interdisciplinary and Education', 'Biology & Life sciences compared to Computers and Mathematics'.'engineering compared to Law & Policy'.

![](https://github.com/Swintabel/Gender-College-and-Earnings/blob/master/Rplot5.jpeg?raw=true)

### **STATISTICAL ANALYSIS OF DATA**

To conduct a simple statistical analysis of the dataset, i will use a multivariate linear regression model. In this model, the log of Median earnings is the dependent variable and the log of 'Total'(total number of majors), major category and the proportion of women are the independent variables. For Major category, 'Psychology & Social Work' will be the reference major category for interpretation of parameter estimates.

#### **HYPOTHESIS**

1. + Status quo: The proportion of women has no impact on earnings for any given major.
   + Alternatively: The proportion of women has a negative impact on earnings for any given major.
   
2. + Status quo: The Total number of people majoring in any major category has no impact on earnings.
   + Alternatively:The Total number of people majoring in any major category has an impact on earnings.
   
3. + Status quo: The major category has no impact on earnings.
   + Alternatively:The major category has an impact on earnings.

The table below displays the findings from the model.

![](https://github.com/Swintabel/Gender-College-and-Earnings/blob/master/regression%20analysis.JPG?raw=true)


#### **INTERPRETATION OF RESULTS**

##### PROPORTION OF WOMEN

The model shows that, a 1% increase in the **proportion of women** in any major is **associated with a 35% reduction** in the median **earnings** of year round employees within the specified field. This estimate is **highly significant** even at a level of significance less than 0.001. Therefore, we reject the status-co that the proportion of women has no impact on earnings and **fail to reject** that the proportion of women has a negative impact on earnings for any given major. 

##### TOTAL NUMBER OF MAJORS

The model shows that a 1% increase in the total number of people majoring in any course is associated with a 0.01% fall in the median earnings of year round employees in the respective field. This estimate is significant at 5%. Therefore we can **only reject the status quo** at a level of **significance of 5%** and conclude that total majors has a negative effect on earnings at the said level of significance but otherwise at any lesser level of significance.

##### MAJOR CATEGORY

The results show that all other major categories are associated with earnings that are **higher than that of 'Psychology & Social Work'**. The highest of them is **engineering** which is associated with earnings that are 44% higher than that of 'Psychology & Social Work'. Other majors with significantly higher earnings compared to 'Psychology & Social Work' are:**'Business' , 'Computers & Mathematics', 'Health', 'Law & Public Policy', and 'Physical Sciences'.**

**The model explains about 65% of the changes that occur in earnings**

#### **CONCLUSION**

The gender share(proportion of women) of any major has a significantly negative impact on the earnings associated with the field. In addition, the total number of people majoring in any field is also negatively associated with the earnings in that field though not as significant as gender share. Lastly, of all the major categories, Engineering pays the highest and Psychology & Social Work pays the lowest; all other major categories also pay higher than psychology & social work.

Thus, though college education can have an overall positive impact on anyone whether male or female, the impact is unequal and with other factors such as number of people in the choice of major or the even the choice of major in itself can further reduce the expected benefit in monetary terms.

However, this is not to downplay the possible non monetary benefits that comes along with higher education especially for women.


#### **RECOMMENDATIONS**

The issue of labour market gender inequality has been with for long and there is the need to keep exploring data to find answers to these situations that come in different folds(unemployment amongst women, lay-offs and matters like this). In the near future a project in line with more recent data and also in the context of Africa and Ghana to be precise would be worth exploring.

Let's keep sensitizing the world and someday, it would hear us.

 
