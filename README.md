<br>

# Development Workflow

Complete project development workflow for **version control** of Glide projects.

This workflow deals with all stages of a project developmnt from start till launch. This workflow also includes process for properly supporting and maintaining the project after launch.

<br>
<br>

![1](images/1.png)

## 💯 WPEngine Site

Start off with the correct setup in WP engine website hosting account.

Guidelines on how to name these environments and their respective users is available here in [Glide Nomenclature](https://github.com/) document.

Make sure to follow the nomenclature guidelines in order to ensure same naming scheme across all projects and environments.

Following is the list of tasks to be performed on WP Engine.

<br>

1.  Add wp engine website `production environment`

2.  Add its `staging environment`

3.  Add its `development environment`

4.  Add one sftp user to each of these environments

5.  Open wordpress admin of `development environment`

6.  Update site title and tagline with project name

7.  Add admin user for Glide's use

8.  Add admin user for Client's use

9.  Copy `development environment` to both `staging` and `production environments`

<br>

***From this point onwards developers need to work in development environment only.***

More information on purpose of each WP Engine environment and how to use them can be found here in [WP Engine Environments](https://github.com/) document.

<br>
<br>

![2](images/2.png)

## 🌋 Local WP Site

Use [Local WP](https://github.com/) for setting up local WordPress environment.

Local WP is supported by WP Engine and it fully integrates with their service.

<br>

1. Open Local WP

2. Connect Local WP with WP Engine Account

3. Pull `development environment` of your project into Local WP

<br>

If for any reason you can not pull the `development environment`, add a new site to Local WP.

Make sure to follow the Glide [naming scheme](https://github.com/) for this purpose.

<br>
<br>

![3](images/3.png)

## 💯 Local Repository

<br>

1. Open Local WP project folder and convert it into a local repository

2. Add .gitignore file

3. Add base theme to themes folder

<br>
<br>

![4](images/4.png)

## Github Repository

1. Create repository in github

2. Connect local and github repositories

3. Add action in github for continuous deployment

4. Connect WP Engine development environment and github

5. Update base theme with project name

6. Stage, commit and push the first change in master branch

<br>
<br>

![5](images/5.png)

## Github Branches
---

1. Create development branch from master branch

2. Create developer branches from development branch

3. Merge developer branches back into developmeant branch

4. Create release branch from development branch

5. Update version number in theme files and test code

<br>
<br>

![6](images/6.png)

## First Release - v1.0.0

1. Merge release branch into master branch

2. Automatic deployment pushes code to development environment on wp engine

3. Tag master branch with new version number

4. Merge release branch back into development branch

5. Push database from Local WP to WP Engine

6. Review development environment

7. Copy development environment to staging environment

8. Share staging environment with reviewers

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
