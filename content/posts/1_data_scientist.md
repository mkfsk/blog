+++
title = "Data science"
date = "2022-03-24"
categories = ["Data science"]
tags = [
    "data science", 
    "python",
]
+++


# What is data science?
---

Is data science worth changing my career? <!--more-->

<!---
![Pomeranian working on an iPad](https://source.unsplash.com/gySMaocSdqs/ "Pomeranian working on an iPad")
--->

{{<figure src="https://source.unsplash.com/gySMaocSdqs/" alt="Pomeranian working on an iPad" caption="Photo by [Conner Denessen](https://unsplash.com/@wanderingconner) on Unsplash">}}

Data science is a multidisciplinary approach to solving complex problems. Mathematics, technology, and business skills are tools that data scientists use to solve problems. 
The general cycle of solving problems is discovering, processing, analyzing, communicating. Since data science requires various professional knowledge, work is highly challenging.


# Why I want to be a data scientists?
---

I wanted to become a data scientist because my current job is meaningless to me. My current job is very repetitive and requires minimum thinking. I think robots will do a better job than I do. Also, I do not see any future in my career.

Moreover, I am passionate about technology and teach myself diverse subjects about them. I read and watched about Linux, python, networking, scripting, and more. Although I can only perform a simple task, I know enough to appreciate and fascinate by the technology people created. I have a desire to become like them and return to the community.


# How to become a data scientists?
---

I searched many websites and watched many videos about becoming a data scientist. Some provide similar and conflicting answers. I concluded that I should find the solution for myself. Most online information proposes becoming data scientists in order of knowledge/certification, degree, and job. Since my goal is to get a data scientist job, I start to collect information from jobs, degrees, and knowledge/certification orders.

I collected requirement data from Indeed and Glassdoor. Since data is similar and short, I manually copy and paste.
I created Python code to learn and practice while getting information.

Requirement counter:

```python
import pandas as pd
import collections

df = pd.read_csv("requirements.csv")

words = df["Requirements"].to_list()

comb_list = []

for i in words:
    i_comm = i.split(",") # str to list separated by comma
    for x in i_comm:
        x_low_clean = x.lower().strip() # lowercase and listed
        comb_list.append(x_low_clean) # add cleaned list to comb_list

combined_counts = collections.Counter(comb_list) # dict for counting hashable objects

for x in sorted(combined_counts.items(),key=lambda item: item[1]): # sorting dict
    print(x)
```

I have spent server hours creating this simple code. I enjoyed learning about python and creating code that is working. However, cleaning data was frustrating. Whitespaces, commas, and wording were obstacles before processing the data. I got most of the answers from online forums, which helped me understand the problem and view different angles to solve problems.

Output:
> 30 companies requirements are used  
> The result is show only mentioned more than 2

```python
('github', 2)
('numpy', 2)
('d3', 2)
('ggplot', 2)
('pandas', 2)
('spss', 2)
('excel', 2)
('modeling', 3)
('cloud computing', 3)
('nosql', 3)
('hive', 3)
('looker', 3)
('data mining', 4)
('hadoop', 4)
('a/b', 4)
('sas', 4)
('large datasets', 5)
('tableau', 8)
('ml', 8)
('r', 15)
('sql', 21)
('statistics', 22)
('python', 24)
```

**Important skills to know!**  
***Statistics***  is the most important skill mentioned in every single requirement  
Language: Python and R  
Visualization: Tableau, looker  
Database: SQL and NoSQL  
Other: ML, large datasets experience, cloud computing, processing and analytics

Keep in mind the result is not an absolute answer for requirements.  In the result, some data is "missing" because some company requirements state requires some skill and is not specific about which skill.

# Summary
---
Becoming a data scientist is **NOT** easy.
I must know:
- Statistics
- Programing language
- Data mine, clean, analyze
- Visualization
- Communication

I should be highly motivated and willing to learn everything! 

Thanks!