<br>

# Development Workflow

Complete project development workflow for **version control** of Glide projects.

This workflow deals with all stages of a project developmnt from start till launch. This workflow also includes process for properly supporting and maintaining the project after launch.

<br>
<br>
<br>

![1](images/1.png)

## 1️⃣ - WPEngine Site

Start off with the correct setup in WP engine website hosting account.

Guidelines on how to name these environments and their respective users is available here in [Glide Nomenclature](https://github.com/) document.

> ✔️ Make sure to follow the nomenclature guidelines in order to ensure same naming scheme across all projects and environments.

<br>

Following is the list of tasks to be performed on WP Engine.


-  Add wp engine website `production environment`

-  Add its `staging environment`

-  Add its `development environment`

-  Add one sftp user to each of these environments

-  Open wordpress admin of `development environment`

-  Update site title and tagline with project name

-  Add admin user for Glide's use

-  Add admin user for Client's use

-  Copy `development environment` to both `staging` and `production environments`

<br>

**From this point onwards developers need to work in development environment only.**

> ✔️ More information on purpose of each environment and how to use them is here in [WP Engine Environments](https://github.com/) document.

<br>
<br>
<br>

![2](images/2.png)

## 2️⃣ - Local WP Site

Use [Local WP](https://github.com/) for setting up local WordPress environment.

Local WP is supported by WP Engine and it fully integrates with their service.

<br>

- Open Local WP

- Connect Local WP with WP Engine Account

- Pull `development environment` of your project into Local WP

<br>

If for any reason you can not pull the `development environment`, add a new site to Local WP.

> ✔️ Make sure to follow the [Glide Nomenclature](https://github.com/) for Local WP.

<br>
<br>
<br>

![3](images/3.png)

## 3️⃣ - Local Repository

Use [Github Desktop](https://github.com/) for easy GUI based git workflow.

<br>

- Open Local WP project folder and convert it into a local repository

- Add `.gitignore` file

- Add base theme to WordPress themes folder

<br>

> ✔️Use latest version of [Glide Base Theme](https://github.com/) from Github

<br>
<br>
<br>

![4](images/4.png)

## 4️⃣ - Github Repository

Use [Glide Design](https://github.com/) github account and user for setting up remote repository.

<br>

- Create repository in Github

- Connect local and Github repositories

- Add action in Github for continuous deployment

- Connect WP Engine development environment and Github

- Update base theme with project name

- Stage, commit and push the first change in `master branch`

<br>

> ✔️ Make sure to follow the [Glide Nomenclature](https://github.com/) for Github repository.

<br>
<br>
<br>

![5](images/5.png)

## Github Branches

Documentation on how Glide Design uses various branch types for different purposes is here in [Github Branches](https://github.com/) document.

<br>

- Create `development branch` from `master branch`

- Create `developer branches` from `development branch`

<br>

**From this point onwards multiple developers can work on the same project at same time.**

> ✔️ Make sure to follow the [Glide Nomenclature](https://github.com/) for Github branches.

<br>
<br>
<br>

![6](images/6.png)

## First Release - v1.0.0

So the development of the project is complete and its time to show off the hard work. 

Let's put up the demo website for client and release our first theme version.

<br>

- Merge `developer branches` back into `developmeant branch`

- Create `release branch` from `development branch`

- Update version number in theme files and test code

- Merge `release branch` into `master branch`

- Automatic deployment pushes code to development environment on WP Engine

- Tag `master branch` with new version number

- Merge `release branch` back into `development branch`

- Push database from Local WP to WP Engine

- Review `development environment`

- Copy `development environment` to `staging environment`

- Share `staging environment` with reviewers

<br>
<br>
<br>

![7](images/7.png)

## Reviews & Tickets

1. Create developer branches from development branch

2. Pull latest version of database (if required.

3. Pull latest version of uploads folder (if required.

4. Merge developer branches back into developmeant branch

<br>
<br>

![8](images/8.png)

## Second Release v1.0.1

1.  Create release branch from development branch

2.  Update version number in theme files and test code

3.  Merge release branch into master branch

4.  Automatic deployment pushes code to development environment on wp engine

5.  Tag master branch with new version number

6.  Merge release branch back into development branch

7.  Review development environment

8.  Copy development environment to staging environment (files only.

9.  Do content and image edits on staging environment (if required.

10. Share staging environment with reviewers

11. On approval copy staging environment down to development environment

<br>
<br>

![9](images/9.png)

## Launch Release v2.0.0

1.  Create release branch from development branch

2.  Update version number in theme files and test code

3.  Merge release branch into master branch

4.  Automatic deployment pushes code to development environment on wp engine

5.  Tag master branch with new version number

6.  Merge release branch back into development branch

7.  Review development environment

8.  Copy development environment to staging environment (files only.

9.  Do content and image edits on staging environment (if required.

10. Share staging environment with reviewers

11. On approval copy staging environment down to development environment

<br>
<br>

![10](images/10.png)

## Launch

1.  Copy approved staging environment to production environment

<br>
<br>

![11](images/11.png)

## Support

1.  Copy production environment to staging environment

2.  Copy staging environment to development environment

3.  Create developer branch from development branch

4.  Pull latest version of database to Local WP (if required.

5.  Pull latest version of uploads folder to Local WP (if required.

6.  Merge developer branches back into development branch

<br>
<br>

![12](images/12.png)

## Support Release v2.0.1

1.  Create release branch from development branch

2.  Update version number in theme files and test code

3.  Merge release branch into master branch

4.  Automatic deployment pushes code to development environment on wp engine

5.  Tag master branch with new version number

6.  Merge release branch back into development branch

7.  Review development environment

8.  Copy development environment to staging environment (files only.

9.  Do content and image edits on staging environment (if required.

10. Share staging environment with reviewers

11. On approval copy staging environment down to development environment

12. Copy approved staging environment to production environment
