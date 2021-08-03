<br>
<br>
<br>

![Glide Design](../assets/images/glide.png)

<br>
<br>
<br>

# WP Engine Environments Workflow

<br>

WP Engine environemts workflow for **version control** of Glide projects. 

This document explains what is the purpose of each environment type and why and how to use it in development workflow.

This document deals with all rules that we have to be followed when working with different types of environments in WP Engine account.


<br>
<br>
<br>
<br>

![1](../assets/images/1.png)

## 1️⃣ - Production Environment

<br>

> ✔️ This is live website, this is only meant for public view

<br>

- This will always have 100% final, tested and approved code and data

- Never ever make an edit to code on live website

<br>
<br>
<br>
<br>

![2](../assets/images/2.png)

## 1️⃣ - Staging Environment

<br>

> ✔️ This is staging website to review changes and updates, this is meant for reviewers and content editors

<br>

- Staging environment will serve as bridge between development environment and production environment

- Whenever we need to do new set of updates we can copy data from production environment

- When updates are done, Code will be pushed from development environment into staging environment

- When this is ready to go live we can push code to production environment

- Staging data will never get pushed upwards to production environment, only if we are going live for first time

<br>
<br>
<br>
<br>

![3](../assets/images/3.png)

## 2️⃣ - Development Environment

<br>

> ✔️ This is development website to develop new code, this is meant for developers only

<br>

- Whenever we need to do new set of updates we can copy data from staging environment

- When this is ready we can push code to staging environment.

- Development data will never get pushed upwards to staging environment, only if we are going live for first time

<br>



<br>
<br>

Happy Coding!

<br>

**Prepared by:**
Muhammad AbuBakar

<br>
<br>
