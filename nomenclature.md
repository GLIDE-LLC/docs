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


### 📙 Site Name      

- Project Name will be used here with proper spaces

- WP Engine allows 40 characters for this so it will not be an issue to have a proper and nice Site Name

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

### 📙 Environment Name

- Project name will be used here in lowercase and without spaces

- This will be lowercase version of the site same

- If site name is longer than 11 characters, try using only first word from the site name

- Even if that is not available use portion of second word from site name

- WP Engine allows only 14 characters, Use 11 characters for project name and last 3 characters to identify the environment type

- `prd` for `production environment`

- `stg` for `staging environment`

- `dev` for `development environment`

- Make sure all enviroments have same URL except for the 3 character identifier.

- With the help of this identifier in URL everyone will know on which specific environment he/she is and it also looks way more professional than having random names for these environments

<br>

#### 👉 For Example

- `glidedesignprd.wpengine.com` will be the url of `production environment`

- `glidedesignstg.wpengine.com` will be the url of `staging environment`

- `glidedesigndev.wpengine.com` will be the url of `development environment`

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

### 📙 SFTP Users

- Always add two sftp users to each of the WP Engine environments

- One will be used by **Glide Team** and the other will be used by **Client and its team**

- Username for Glide's SFTP account will be `glidesftp`

- Username for Client's SFTP account will be `clientsftp`

- When adding sftp user on any environment only write `glidesftp` or `clientsftp` in username input field

- `glidedesignprd-` prefix is automatically added by WP Engine

- So the added username will become `glidedesignprd-glidesftp` instead of just `glidesftp` that we entered

- With the help of this prefix, everyone will know what is the purpose of this sftp user and to whom it belongs

<br>

#### 👉 For Example

- Glide's sftp username for `production environment` will be `glidedesignprd-glidesftp`

- Glide's sftp username for `staging environment` will be `glidedesignstg-glidesftp`

- Glide's sftp username for `development environment` will be `glidedesigndev-glidesftp`

- Client's sftp username for `production environment` will be `glidedesignprd-clientsftp`

- Client's sftp username for `staging environment` will be `glidedesignstg-clientsftp`

- Client's sftp username for `development environment` will be `glidedesigndev-clientsftp`

<br>

> **Allowed**
> 
> ✔️ `glidesftp` <br>
> ✔️ `clientsftp`
>  
>  <br>
> 
> **Not Allowed**
> 
> ❌ `glidedesignsftp` <br>
> ❌ `glide-sftp` <br>
> ❌ `clientuser` <br>
> ❌ `client-sftp` 

<br>
<br>
<br>
<br>


## 1️⃣ - WordPress

Follow these guidelines for naming WordPress accounts for different uses.

<br>

- Add two WordPress admin users to only development environment

- One will be used by **Glide Team** and the other will be used by **Client and its team**

- Username for Glide's WordPress account will be `glideadmin`

- Username for Client's WordPress account will be `clientadmin`

- No need to create users on staging environment and production environment

- These environments will get their users when for first time development environment is copied over to them

<br>

#### 👉 Admin User for Glide's use

- username will always be glideadmin
- email will always be support@glidedesign.com

<br>

> **Allowed**
> 
> ✔️ `glideadmin`
>  
>  <br>
> 
> **Not Allowed**
> 
> ❌ `glidedesign` <br>
> ❌ `glide-admin` <br>
> ❌ `gadmin` <br>
> ❌ `glidedev` 
> 

<br>
<br>

#### 👉 Admin User for Client's Use

- username will always be clientadmin

- email will always be main point of contact for client hello@clientwebsite.com

- If client needs further admin users, he can create those by logging into this user or we can assist them.

<br>

> **Allowed**
> 
> ✔️ `clientadmin`
>  
>  <br>
> 
> **Not Allowed**
> 
> ❌ `clientname` <br>
> ❌ `client-admin` <br>
> ❌ `cadmin` <br>
> ❌ `client-name` 

<br>
<br>
<br>
<br>

## 1️⃣ - Github

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
