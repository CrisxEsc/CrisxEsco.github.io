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

## Enhancement Strategy

Explain the algorithmic improvements or data structure changes you implemented. Examples include:

- Replacing inefficient algorithms with optimized variants
- Introducing appropriate data structures to reduce complexity
- Parallelizing or batching operations to improve throughput
- Adding instrumentation or profiling to validate performance gains

## Results & Evidence

| Metric | Before | After | Notes |
| --- | --- | --- | --- |
| Time Complexity | _e.g., O(n^2)_ | _e.g., O(n log n)_ | _Explain the change_ |
| Space Complexity | _Describe baseline_ | _Describe improvement_ | _Add references to code_ |
| Performance Benchmark | _Add numeric baseline_ | _Add improved result_ | _Link to benchmark script or output_ |

---
## Reflection

Through this enhancement, I strengthened my understanding of complexity and optimization. I measured query performance before and after, which helped me see the impact of using the right tools. I also practiced managing memory with care. The LRU cache taught me how to balance space and speed. When I saw users navigating smoothly between screens, I knew the changes were working. These enhancements supported outcomes around designing solutions with clear trade offs and using structured data effectively.
