---
layout: post
title: "Topic Modelling for Healthcare News"
date: 2019-06-24 16:43:22 +1000
image: default-photo2.jpg
categories: project
---
### **Goal:** 
This project attempted to address the trend of previous healthcare news form different sources (bbc, cbc, etc ....) and to predict the future healthcare content.
<br>
data: 'the data set I have used is a list of over 50k healthcare tweets headlines published over a period of 2011 to 2015 and can be download from link below
<br>
[UCI Machine Learning Repository][UCI-Machine-Learning-Repository].

### **Data**
My raw data contains multiple text files which are related to one Twitter account of a new agency. Each line contains tweet basic information such as date, time and tweet.
<br>
They are explored by multiple bar charts. As you can see the vast majority of my data was well increase during first 3 and last 3 months of the years.
1. *Visualize by **Contribution***
    ![explore raw data]({{site.baseurl}}/assets/images/pro_caps_data.jpg){: .md-img.md-img-1}
2. *Visualize by **Months***
    ![explore raw data by months]({{site.baseurl}}/assets/images/pro_caps_data2.jpg){: .md-img.md-img-1} 
3. *Visualize by **Weekdays***
    ![explore raw data weekdays]({{site.baseurl}}/assets/images/pro_caps_data3.jpg){: .md-img.md-img-1}

I decided to leave these details and go further steps in my EDA process.

<br><br><br>
### **Exploratory Data Analysis (EDA)**
I applied some techniques here to gather more data from raw materials which will can be named, as web scraping.
<br>
There captured information are being processed by multiple techniques:
1. ***Web scraping** technique*
    ![EDA steps]({{site.baseurl}}/assets/images/pro_caps_eda.jpg){: .md-img.md-img-1}
2. ***Before** text pre-processing*
    ![EDA before cleaning]({{site.baseurl}}/assets/images/pro_caps_eda1.png){: .md-img.md-img-1}
3. ***After** text pre-processing*
    ![EDA after cleaning]({{site.baseurl}}/assets/images/pro_caps_eda2.png){: .md-img.md-img-1}
Then, I started to stored all raw data into database. While my captured content are stored in local multiple text files.

<br><br>
### **Model:**
I 
1. **Method 1**
   ![Model 1 with topic]({{site.baseurl}}/assets/images/pro_caps_model.jpg){: .md-img.md-img-1}
2. **Method 2**
   ![Model 1 with topic]({{site.baseurl}}/assets/images/pro_caps_model.jpg){: .md-img.md-img-1}

<br><br>
### **Deployment:** 
*Link: **[Online Demo][GCL]***
<br>
*Link: **[Localhost][local]***

[UCI-Machine-Learning-Repository]: https://archive.ics.uci.edu/ml/datasets/Health+News+in+Twitter
[GCL]: http://35.189.11.206:1306
[local]: localhost:5000