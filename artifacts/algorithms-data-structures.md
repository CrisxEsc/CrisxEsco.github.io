---
layout: default
title: Algorithms & Data Structures
permalink: /artifacts/algorithms-data-structures.html
---

{% include portfolio-nav.html %}

# Algorithms & Data Structures Enhancement

## Brief Overview

For this category, I continued working on the Event Tracker project. I wanted to improve its responsiveness and scalability. I focused on how the app retrieved and stored event data, especially when filtering or loading large lists. This made it the right fit for demonstrating algorithmic thinking and effective use of data structures.

I added indexes to the database to make searches faster. I also implemented an in memory cache using a Least Recently Used strategy, which stored recent queries so repeat searches could load instantly. These changes made the app more efficient and less dependent on network access. I also added offline caching with logic to sync changes when the device reconnects. That work required planning for conflicts and retry logic.

## Baseline Performance or Behavior

> _Summarize how the original implementation worked and any performance metrics, limitations, or complexity concerns you identified._

## Enhancement 

### Click here to see project
[![Event Tracking Application](https://img.shields.io/badge/GitHub-Event%20Tracking%20Application-181717?logo=github&logoColor=white&style=for-the-badge)](https://github.com/CrisxEsc/Event-Tracking-Application)


---
## Reflection

Through this enhancement, I strengthened my understanding of complexity and optimization. I measured query performance before and after, which helped me see the impact of using the right tools. I also practiced managing memory with care. The LRU cache taught me how to balance space and speed. When I saw users navigating smoothly between screens, I knew the changes were working. These enhancements supported outcomes around designing solutions with clear trade offs and using structured data effectively.
