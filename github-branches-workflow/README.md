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

- `Release branches` will be created from this branch to release new theme versions

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
<br>
<br>
<br>

![4](../assets/images/4.png)

## 4️⃣ - Hotfix Branch

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
<br>
<br>
<br>

![4](../assets/images/4.png)

## 4️⃣ - Golden Rule - 🔺 Code Moves Up 🔻 Data Moves Down

<br>

The `top` layer is `production environment` that is live website for public view.

The `middle` layer is `staging environment` that serves as bridge between other two.

The `bottom` layer is `development environment` where we are developing the website.

<br>
<br>

![Golden Rule](../assets/images/golden-rule.png)

<br>
<br>

The code will always move upwards from `development` to `staging` to `production environment`.

The database will always move downwards from `production` to `staging` to `development environment`.

Staging environment will always serve as bridge between the other two environments and all reviewing and testing will be done on staging environmnt.

**✅ Never move database upwards from staging to production to avoid mishaps.**

<br>
<br>

Happy Coding!

<br>

**Prepared by:**
Muhammad AbuBakar

<br>
<br>
