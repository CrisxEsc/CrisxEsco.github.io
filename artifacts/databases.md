---
layout: default
title: Databases
permalink: /artifacts/databases.html
---

{% include portfolio-nav.html %}
---
# Databases Enhancement

## Brief Overview

For the database category, I worked on the Animal Shelter Dashboard. This is a web application that uses MongoDB to manage shelter data. The original version ran multiple queries and processed data on the front end, which slowed things down. I chose this artifact because it gave me the chance to show how database design and query optimization can change the user experience.

I rewrote several data paths using aggregation pipelines. This let the database handle grouping and counting, which reduced the load on the application and made it faster. I added indexes to fields that appear in filters. I also applied stronger validation both in the client and server code to protect data quality and reduce user errors.
---
## Original Data Model

![Old_Dash](assets/OG_Dash.png) ![OG_Animal](assets/AAC.png)

---
## Enhancement Details
    git submodule add https://github.com/CrisxEsc/Animal-Shelter.git content/Animal-Shelter

![New_Dash](assets/New_Dash.png)  
![AAC](assets/OG_Animal.png)
---
## Reflection
This process helped me connect database principles to actual outcomes. I used explain plans to verify that indexes worked. I found that a well written aggregation can replace pages of front end logic. I also practiced creating validation rules to catch bad input early. One lesson I learned was to build validation where it is needed most. I made sure form inputs give clear guidance and that the database rejects anything outside the expected shape. These enhancements aligned with outcomes related to secure data handling, performance tuning, and building reliable data driven applications.
