<br>
<br>
<br>

![Glide Design](images/glide.png)

<br>
<br>
<br>

# Glide Nomenclature

Proper naming scheme to be followed by **all teams and project managers** for Glide projects.

This nomenclature deals with all pieces of Glide's WordPress projects from local environment to remote. This nomenclature also includes naming scheme for WordPress theme and its files and functions.

<br>
<br>
<br>
<br>

![1](images/1.png)

## 1️⃣ - WP Engine

Follow these guidelines for naming WP Engine environments.

<br>

### 📑 Site Name

- Project Name will be used here with proper spaces.

- Wp Engine allows 40 characters for this so it will not be an issue to have a proper and nice Site Name

- Make Sure project name is never more than 3 words, ideally it should be combination of 2 words

<br>

#### 👉 For Example
- Glide Design

<br>

> **Allowed**
> 
> ✔️ Glide Design
>  
>  <br>
> 
> **Not Allowed**
> 
> ❌ G Design <br>
> ❌ Glide <br>
> ❌ GlideDesign <br>
> ❌ Glide Design Company LLC 

<br>
<br>

### ▶️ Environment Name

- Project name will be used here in lowercase and without spaces.

- This will be lowercase version of the Site Name.

- If site name is longer than 11 characters. Try using only first word from the site name. Even if that is not available use portion of second word from site name.

- WP Engine allows only 14 characters for this. We will use 11 characters for project name and last 3 characters to identify the environment type.

- `prd` for `production environment`

- `stg` for `staging environment`

- `dev` for `development environment`

- Make sure all enviroments have same URL except for the 3 character identifier.

- With the help of this identifier in URL everyone will know on which specific environment he/she is and it also looks way more professional than having random names for these environments.

<br>

#### 👉 For Example
- `glidedesignprd.wpengine.com` will be the url for `production environment`

- `glidedesignstg.wpengine.com` will be the url for `staging environment`

- `glidedesigndev.wpengine.com` will be the url for `development environment`

<br>

> **Allowed**
> 
> ✔️ `glidedesignprd.wpengine.com`
>  
>  <br>
> 
> **Not Allowed**
> 
> ❌ `glidedesign.wpengine.com` <br>
> ❌ `gdesignprd.wpengine.com` <br>
> ❌ `glidedesignpro.wpengine.com` <br>
> ❌ `glidellc.wpengine.com` 

<br>
<br>

## SFTP Users

- When adding sftp users for each of the environments make sure to use the identifier as the username.

- For Example, when adding sftp user on production environment only write glidesftp in username input field.

- Once you add the username wp engine will automatically prefix it with environment name.

### For example
- sftp username for production environment will become glidedesignprd-glidesftp
- sftp username for staging environment will become glidedesignstg-glidesftp
- sftp username for development environment will become glidedesigndev-glidesftp

---
## WordPress
---

- There will always be two wp admin accounts added to dev environment.

- Which will automatically get copied over to staging and production environment when site will go live for first time.

- One will be used by Glide Team and the other will be used by Client and its Team.

## Admin User for Glide's use

- username will always be glideadmin

### Not allowed
- glidedesign
- glide-admin
- gadmin

- email will always be support@glidedesign.com

## Admin User for Client's Use

- username will always be clientadmin

### Not allowed
- clientname
- client-admin
- cadmin

- email will always be their main point of contact.

- If client needs further admin users, he can create those by logging into this user or we can assist them.

---
## GitHub
---

- Each project will have its dedicated repository and it will be properly versioned and tagged.

## Repositoy Name

- It will be same as project name except it will be in lowercase and will have dashes instead of spaces.

- If project name is Great Client repository will be named as great-client

## Branches

- master branch as default will always be named "master"

- active development branch will always be named "development"

- hotfix branches will be named as "hf-03jul21" where hf stands for hotfix and the date helps us quickly see how old the branch is.
if we have to create multiple hotfix branches in same day, we will add roman numbering to end of it for easy identification for example "hf-03jul21" , "hf-03jul21i" and "hf-03jul21ii"

- developer branches will be named as "tm-03jul21" where tm stands for Travis McAshan and the date helps us quickly see how old the branch is.
if we have to create multiple developer branches in same day, we will add roman numbering to end of it for easy identification for example "tm-03jul21" , "tm-03jul21i" and "tm-03jul21ii"

- release branches will be named as "release-v1.0.0"

---
## Local WP
---

## Local Environment

- Local environment url will be same as project name except it will be in lowercase and will have dashes instead of spaces.

- If project name is Great Client Local environment url will be named as great-client.local

## Admin Users

- Same admin users as live will be fetched into local install on first sync

---
## WordPress Theme
---

## Theme Name

- Theme Name will be same as project name.

- If project name is Great Client theme name will be Great Client.

## Theme Folder

- Theme folder will be same as project name except it will be in lowercase and will have dashes instead of spaces.

- If project name is Great Client theme folder will be great-client
