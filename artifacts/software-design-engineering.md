---
layout: default
title: Software Design & Engineering
permalink: /artifacts/software-design-engineering.html
---

{% include portfolio-nav.html %}

# Software Design & Engineering Enhancement


## Brief Overview

My enhancement in software design focused on the Event Tracker mobile application. This app allows users to log and view events, and it began with a simple structure that lacked flexibility. I selected this artifact because it presented a real opportunity to apply modern architecture principles and create a cleaner, more reliable system. I redesigned the app using a Model View ViewModel structure and separated core logic into reusable components. This helped me deliver better maintainability and performance.

I implemented input validation across the app to prevent crashes caused by empty or malformed entries. I also used secure storage for sensitive data, relying on Android's encryption tools to protect user information. These decisions required careful design and testing. I demonstrated skills in architecture design, defensive programming, and platform specific security.

## Original Implementation Snapshot

![Old DB](https://raw.githubusercontent.com/CrisxEsc/CrisxEsco.github.io/29e8544466e15bf201cabccac339b1c532072473/assets/Old_DB.png)


## Enhancement 

### Click here to see project
[![Event Tracking Application](https://img.shields.io/badge/GitHub-Event%20Tracking%20Application-181717?logo=github&logoColor=white&style=for-the-badge)](https://github.com/CrisxEsc/Event-Tracking-Application)


![App screenshot](https://raw.githubusercontent.com/CrisxEsc/CrisxEsco.github.io/91f342bb0643a1a1fa5ca038f32b93e75c2d3129/assets/App.png)


---
## Reflection

During the enhancement process, I learned how planning upfront can save time later. I drew diagrams and mapped data flows before touching code. Converting from a monolithic design to a layered model challenged me to manage dependencies and keep the UI responsive. I wrote unit tests to confirm that logic stayed intact during the refactor. I learned how to keep the interface simple while introducing more structure underneath. These efforts met outcomes around designing maintainable solutions, applying secure practices, and using industry tools to deliver real value.

