<br>
<br>
<br>

![Glide Design](../assets/images/glide.png)

<br>
<br>
<br>

# Development Workflow

Complete project development workflow for **version control** of Glide projects.

This workflow deals with all stages of a project developmnt from start till launch. This workflow also includes process for properly supporting and maintaining the project after launch.

<br>
<br>

| #  | Topics |
|----|-------|
| 01 | [WPEngine Site](https://github.com/abubakar-me/glide-design/tree/master/glide-development-workflow#1%EF%B8%8F%E2%83%A3---wpengine-site) |
| 02 | [Local WP Site](https://github.com/abubakar-me/glide-design/tree/master/glide-development-workflow#2%EF%B8%8F%E2%83%A3---local-wp-site) |
| 03 | [Local Repository](https://github.com/abubakar-me/glide-design/tree/master/glide-development-workflow#3%EF%B8%8F%E2%83%A3---local-repository) |
| 04 | [Github Repository](https://github.com/abubakar-me/glide-design/tree/master/glide-development-workflow#4%EF%B8%8F%E2%83%A3---github-repository) |
| 05 | [Github Branches](https://github.com/abubakar-me/glide-design/tree/master/glide-development-workflow#5%EF%B8%8F%E2%83%A3---github-branches) |
| 06 | [First Release `1.0.0`](https://github.com/abubakar-me/glide-design/tree/master/glide-development-workflow#6%EF%B8%8F%E2%83%A3---first-release---100) |
| 07 | [Reviews & Tickets](https://github.com/abubakar-me/glide-design/tree/master/glide-development-workflow#7%EF%B8%8F%E2%83%A3---reviews--tickets) |
| 08 | [Second Release `1.0.1`](https://github.com/abubakar-me/glide-design/tree/master/glide-development-workflow#8%EF%B8%8F%E2%83%A3---second-release-101) |
| 09 | [Launch Release `2.0.0`](https://github.com/abubakar-me/glide-design/tree/master/glide-development-workflow#9%EF%B8%8F%E2%83%A3---launch-release-200) |
| 10 | [Launch](https://github.com/abubakar-me/glide-design/tree/master/glide-development-workflow#-launch) |
| 11 | [Support](https://github.com/abubakar-me/glide-design/tree/master/glide-development-workflow#1%EF%B8%8F%E2%83%A3---support) |
| 12 | [Launch](https://github.com/abubakar-me/glide-design/tree/master/glide-development-workflow#-launch) |
| 13 | [Support](https://github.com/abubakar-me/glide-design/tree/master/glide-development-workflow#1%EF%B8%8F%E2%83%A3---support) |
| 14 | [Support Release `2.0.1`](https://github.com/abubakar-me/glide-design/tree/master/glide-development-workflow#2%EF%B8%8F%E2%83%A3---support-release-201) |

<br>
<br>
<br>
<br>

![1](../assets/images/1.png)

## 1️⃣ - WPEngine Site

Start off with the correct setup in WP engine website hosting account.

All three environment types will be created right at the start of project.

Guidelines on how to name environments and WordPress users is available here in [Glide Nomenclature](https://github.com/) document.

> ✔️ Make sure to follow the nomenclature to ensure same naming scheme across all projects and environments.

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

> ✔️ Information on purpose of each environment and how to use it, is in [WP Engine Environments Workflow](https://github.com/) document.

<br>
<br>
<br>
<br>

![2](../assets/images/2.png)

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
<br>

![3](../assets/images/3.png)

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
<br>

![4](../assets/images/4.png)

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
<br>

![5](../assets/images/5.png)

## 5️⃣ - Github Branches

Documentation on how Glide Design uses various branch types for different purposes is here in [Github Branches Workflow](https://github.com/) document.

<br>

- Create `development branch` from `master branch`

- Create `developer branches` from `development branch`

<br>

**From this point onwards multiple developers can work on the same project at same time.**

> ✔️ Make sure to follow the [Glide Nomenclature](https://github.com/) for Github branches.

<br>
<br>
<br>
<br>

![6](../assets/images/6.png)

## 6️⃣ - First Release `1.0.0`

Development of the project is complete and its time to show off the hard work.

Let's put up the demo website for client and release our first theme version.

<br>

- Create pull request for lead developer

- Lead developer reviews the code

- Merge `developer branches` back into `developmeant branch`

- Create `release branch` from `development branch`

- Update version number in theme files and test code

- Merge `release branch` into `master branch`

- Automatic deployment pushes code to development environment on WP Engine

- Tag `master branch` with new version number `1.0.0`

- Merge `release branch` back into `development branch`

- Push database from Local WP to WP Engine

- Review `development environment`

- Copy `development environment` to `staging environment`

- Share `staging environment` with reviewers

<br>
<br>
<br>
<br>

![7](../assets/images/7.png)

## 7️⃣ - Reviews & Tickets

Staging website is reviewed and tickets are created in done done.

Follow the steps below to start working on done done tickets.

<br>

- Create `developer branches` from `development branch`

- Pull latest version of database (if required)

- Pull latest version of uploads folder (if required)

- Make the required updates and fixes from done done tickets

<br>
<br>
<br>
<br>

![8](../assets/images/8.png)

## 8️⃣ - Second Release `1.0.1`

Required updates and fixes are made to the code.

Let's put up new version of the project on `staging environment` to share with client.

Same process will be followed that was followed for initial demo release.

<br>

- Create pull request for lead developer when you are done with edits

- Lead developer reviews the code

- Merge `developer branches` back into `developmeant branch`

- Create `release branch` from `development branch`

- Update version number in theme files and test code

- Merge `release branch` into `master branch`

- Automatic deployment pushes code to development environment on wp engine

- Tag `master branch` with new version number `1.0.1`

- Merge `release branch` back into `development branch`

- Review `development environment`

8.  Copy `development environment` to `staging environment` (files only.

9.  Do content and image edits on `staging environment` (if required.

10. Share `staging environment` with reviewers

11. On approval copy `staging environment` down to `development environment`

<br>
<br>
<br>
<br>

![9](../assets/images/9.png)

## 9️⃣ - Launch Release `2.0.0`

When reviews and fixes are done and all done done tickets are cleared, it's time to prepare launch release.

<br>

- Create `release branch` from `development branch`

- Update version number in theme files and test code

- Merge `release branch` into `master branch`

- Automatic deployment pushes code to development environment on wp engine

- Tag `master branch` with new version number `2.0.0`

- Merge `release branch` back into `development branch`

- Review `development environment`

- Copy `development environment` to `staging environment` (files only)

- Do content and image edits on `staging environment` (if required)

- Share `staging environment` with reviewers

- On approval copy `staging environment` down to `development environment`

<br>
<br>
<br>
<br>

![10](../assets/images/10.png)

## 🔟 Launch

Everything is already reviewed and ready for launch.

<br>

- Copy approved `staging environment` to `production environment`

<br>

### 🚀 We are live

<br>
<br>
<br>
<br>

![11](../assets/images/11.png)

## 🅾️ - Hotfix

<br>

So right after launch we have to make an emergency fix to the code.

Follow the steps below to fix the issue quickly.

<br>

- Create team specific WordPress account if different team is going to work on tickets

- Install activity tracking plugin, if its not already installed

- Copy `production environment` to `staging environment`

- Copy `staging environment` to `development environment`

- You can skip the previous step if client has not made any file changes.

- Create `hotfix branch` from `master branch`

- Pull latest version of database to Local WP (if required)

- Pull latest version of uploads folder to Local WP (if required)

- Make the required updates and fixes

<br>
<br>
<br>
<br>

![12](../assets/images/11.png)

## 🅾️ - Hotfix Release 2.0.1

When ready to release the hot fix, follow these steps.

<br>

- Create pull request for lead developer when you are done with edits

- Lead developer reviews the code

- Merge `hotfix branch` back into `master branch`

- Automatic deployment pushes code to development environment on wp engine

- Tag `master branch` with new version number `2.0.1`

- Merge `hotfix branch` back into `development branch`

- Review `development environment`

- Copy `development environment` to `staging environment` (files only)

- Do content and image edits on `staging environment` (if required)

- Share `staging environment` with reviewers

- On approval copy approved `staging environment` to `production environment`

- Copy `staging environment` down to `development environment`

<br>
<br>
<br>
<br>

![13](../assets/images/11.png)

## 1️⃣ - Support

Months have passed and client came to Glide support to get some changes made on his website.

Follow the steps below to start working on support tickets.

<br>

- Create team specific WordPress account if different team is going to work on tickets

- Install activity tracking plugin, if its not already installed

- Copy `production environment` to `staging environment`

- Copy `staging environment` to `development environment`

- You can skip the previous step if client has not made any file changes.

- Create `developer branch` from `development branch`

- Pull latest version of database to Local WP (if required)

- Pull latest version of uploads folder to Local WP (if required)

- Make the required updates and fixes from support tickets

- Create pull request for lead developer when you are done with edits

- Lead developer reviews the code

- Merge `developer branch` back into `development branch`

<br>
<br>
<br>
<br>

![14](../assets/images/12.png)

## 2️⃣ - Support Release `2.0.2`

When ready to share the updates with client, follow these steps.

<br>

- Create `release branch` from `development branch`

- Update version number in theme files and test code

- Merge `release branch` into `master branch`

- Automatic deployment pushes code to development environment on wp engine

- Tag `master branch` with new version number `2.0.1`

- Merge `release branch` back into `development branch`

- Review `development environment`

- Copy `development environment` to `staging environment` (files only)

- Do content and image edits on `staging environment` (if required)

- Share `staging environment` with client

- On approval copy `staging environment` down to `development environment`

- Copy approved `staging environment` to `production environment` (files only)

- Do content and image edits on `staging environment` (if required)

- Review `production environment` and update client.

<br>
<br>
<br>
<br>

Noticed? we made content changes twice, Following are the reasons

If client has made any content changes on production website while you were working on support tickets. When you copy over `staging environment` to `production environment`. You will override his changes.

And in another scenario if you have not copied `production environment` completely to `staging environment` prior to working on support tickets, You will end up copying over older version of database to `production environment`.

<br>

Always follow the simple rule explained here in [WP Engine Environments Workflow](https://github.com/) document.

🔺 Code moves up 🔻 Data moves down

**A little bit of extra effort saves the headache.**

<br>

🔴 Its critical that all developers on all teams follow this workflow to ensure proper version control along with effective collaboration on code.

<br>
<br>

Happy Coding!

<br>

**Prepared by:**
Muhammad AbuBakar

<br>
<br>
