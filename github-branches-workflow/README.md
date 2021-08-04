<br>
<br>
<br>

![Glide Design](../assets/images/glide.png)

<br>
<br>
<br>

# Github Branches Workflow

<br>

Github branches workflow for **version control** of Glide projects. 

This document explains what is the purpose of each branch type and why and how to use it in development workflow.

This document also deals with all rules that have to be followed when working with different types of branches in Github.

<br>
<br>

| #  | Topics |
|----|-------|
| 01 | [Master Branch](https://github.com/abubakar-me/glide-design/tree/master/github-branches-workflow#1%EF%B8%8F%E2%83%A3---master-branch) |
| 02 | [Development Branch](https://github.com/abubakar-me/glide-design/tree/master/github-branches-workflow#2%EF%B8%8F%E2%83%A3---development-branch) |
| 03 | [Developer Branch](https://github.com/abubakar-me/glide-design/tree/master/github-branches-workflow#3%EF%B8%8F%E2%83%A3---developer-branch) |
| 04 | [Release Branch](https://github.com/abubakar-me/glide-design/tree/master/github-branches-workflow#4%EF%B8%8F%E2%83%A3---release-branch) |
| 05 | [Hotfix Branch](https://github.com/abubakar-me/glide-design/tree/master/github-branches-workflow#5%EF%B8%8F%E2%83%A3---hotfix-branch) |
| 06 | [Big Picture](https://github.com/abubakar-me/glide-design/tree/master/github-branches-workflow#6%EF%B8%8F%E2%83%A3---big-picture) |

<br>
<br>
<br>
<br>

![1](../assets/images/1.png)

## 1️⃣ - Master Branch

<br>

> ✔️ `Master branch` will always have final code

<br>

- This is main branch of the project repository

- Whenever this is updated, that is tagged as a new version release

- On update code is automatically deployed to `development environment`

- In emergency situation only `hotfix branches` will be created from this branch to make emergency code edits

<br>

![Master Branch](../assets/images/master-branch.png)

<br>
<br>
<br>
<br>

![2](../assets/images/2.png)

## 2️⃣ - Development Branch

<br>

> ✔️ `Development branch` will always have latest code

<br>

- This is active development branch of the project repository

- All developers will create there own `developer branches` from this branch for any type of code edits

- This will branch out of `master branch` after initial project setup

- `Release branches` will be created from this branch to release new theme versions

<br>

![Development Branch](../assets/images/development-branch.png)

<br>
<br>
<br>
<br>

![3](../assets/images/3.png)

## 3️⃣ - Developer Branch

<br>

> ✔️ `Developer branch` will always belong to only one developer

<br>

- This is developer specific branch

- This will branch out of `development branch`

- And merge back into `development branch` when that developer is done with edits

- `Developer branch` will get deleted once that is no longer required

<br>

#### 👉 For Example 

We have 5 new tickets, developer will create a `developer branch` and work on those 5 tickets in his branch. And when he is done, he will merge back into `development branch`.

<br>

![Developer Branch](../assets/images/developer-branch.png)

<br>
<br>
<br>
<br>

![4](../assets/images/4.png)

## 4️⃣ - Release Branch

<br>

> ✔️ `Release branch` will always be attached to a new version release

<br>

- This will branch out of `development branch`

- And after testing and version update it will merge into `master branch`

- `Master branch` will be tagged with a new version number upon merge

- `Release branch` will merge back into `development branch` so that the `development branch`can stay as latest working copy

- `Release branch` will be kept for additional record

<br>

#### 👉 For Example 

We are ready for a new version release, we will create a `release branch` and update version number in this branch. Next, we will merge `release branch` into `master branch` and tag it with new version number. And lastly we will merge `release branch` into `development branch` to keep it as latest working copy.

<br>

![Release](../assets/images/release-branch.png)

<br>
<br>
<br>
<br>

![5](../assets/images/5.png)

## 5️⃣ - Hotfix Branch

<br>

> ✔️ `Hotfix branch` will always be attached to an emergency code edit

<br>

- This will branch out of `master branch` on an emergency basis

- And after fixing and testing it will merge back into `master branch`

- `Master branch` will be tagged with a new version number upon merge

- `Hotfix branch` will merge back into `development branch` so that the `development branch`can stay as latest working copy

- `Hotfix branch` will get deleted once that is no longer required

<br>

#### 👉 For Example 

We have an emergency situation and we need to make quick fix, we will create a `hotfix branch` and update code in this branch. Next, we will merge `hotfix branch` into `master branch` and tag it with new version number. And lastly we will merge `hotfix branch` into `development branch` to keep it as latest working copy.

<br>

![Hotfix Branch](../assets/images/hotfix-branch.png)

<br>
<br>
<br>
<br>

![6](../assets/images/6.png)

## 6️⃣ - Big Picture

<br>

Lets put up everything in one big picture to visualize how the workflow wroks.

<br>
<br>

![Github Branches](../assets/images/github-branches.png)

<br>
<br>

⚠️ Its critical that all developers on all teams follow these guidelines rules to ensure effective version control of Glide projects.

<br>
<br>
<br>

Happy Coding!

<br>

**Prepared by:**
Muhammad AbuBakar

<br>
<br>
