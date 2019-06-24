---
layout: post
title: Predict DA/DS job market in Australia
date: 2019-06-20 10:23:52 +1000
image: default-photo3.jpg
categories: ideas project
---
### **Goal:** 
The main purpose of this project is about to obtain unstructured data from website and to determine the important factors which impacted salaries by applying machine learning tools

<br><br>
### **Data**
I used some tools and python framework, ***Selenium & Scrapy***, to gather data from [Seek.com.au][Sk]. 
The most reason I decided to go with both tools because. 
In other words, Selenium helps me to collect job url, the scrapy helps me to collect the expected data.
These pictures belows show the process:
1. *Collect **Job Url***
    ![explore raw data](/assets/images/pro_p4_data.jpg){: .md-img.md-img-1}
2. *Collect **Job Details***
    ![explore raw data](/assets/images/pro_p4_data1.jpg){: .md-img.md-img-1}
<br>
Job's information will be: ***title, role, location, description and salary***
<br>

<br><br><br>
### **Exploratory Data Analysis (EDA)**
After carefully cleaning the data, I can rely on 310 relevant job advertisements, where all contain the significant salary info. I decided to scrapt more job search (next 2-3 days) and to impute some missing salaries value by having an effect on the median salary
These pictures belows show the process:
1. *Impute **Wages column***
    ![explore raw data](/assets/images/pro_p4_data2.jpg){: .md-img.md-img-1}
2. *Visualize **Job Title***
    ![explore raw data](/assets/images/pro_p4_eda1.jpg){: .md-img.md-img-1}
3. *Visualize **Job Title** per **Location***
    ![explore raw data](/assets/images/pro_p4_eda3.jpg){: .md-img.md-img-1}
4. *Visualize **Job Wages** per **Location***
    ![explore raw data](/assets/images/pro_p4_eda6.jpg){: .md-img.md-img-1}
5. *Visualize **Contract Type***
    ![explore raw data](/assets/images/pro_p4_eda7.jpg){: .md-img.md-img-1}
6. *Visualize**Salary** per industries*
    ![explore raw data](/assets/images/pro_p4_eda5.jpg){: .md-img.md-img-1}

<br><br>
### **Model:**
Beforehand, I started to identify my baseline which is ***68.83%***. Then, I did some models to compare and select the best one which is ***BaggingClassifier*** because of 

![explore raw data](/assets/images/pro_p4_model1.jpg){: .md-img.md-img-1}

<br><br>
### **Natural Language Processing (NLP):** 
I then decided to move forward to NLP part which is mainly focused on ***Job Description***. By applying some basic techniques, I stopped at selecting most 6 common topics.
1. *Visualize **Topic Model***
    ![explore raw data](/assets/images/pro_p4_nlp1.jpg){: .md-img.md-img-1}
2. *Visualize **Topic Model** with KMeans*
    ![explore raw data](/assets/images/pro_p4_nlp2.jpg){: .md-img.md-img-1}

[Sk]: https://seek.com.au
[GCL]: 35.189.11.206:1306