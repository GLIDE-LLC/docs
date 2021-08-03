<br>
<br>
<br>

![Glide Design](../assets/images/glide.png)

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

![1](../assets/images/1.png)

## 1️⃣ - WP Engine

Follow these guidelines for naming WP Engine environments.

> Guidelines on how to use different WP Engine environments in development Workflow is available here in [WP Engine Environments Workflow](https://github.com/) document.

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

- `glidedesignprd.wpengine.com` will become url of `production environment`
- `glidedesignstg.wpengine.com` will become url of `staging environment`
- `glidedesigndev.wpengine.com` will become url of `development environment`

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

![2](../assets/images/2.png)

## 2️⃣ - WordPress

Follow these guidelines for naming WordPress accounts for different uses.

<br>

- Add two WordPress admin users to only development environment

- One will be used by **Glide Team** and the other will be used by **Client and its team**

- Username for Glide's WordPress account will be `glideadmin`

- Username for Client's WordPress account will be `clientadmin`

- No need to create users on staging environment and production environment

- These environments will get their users when for first time development environment is copied over to them

<br>

### 📙 Admin Account for Glide's Use

- Username will be `glideadmin`

- Email will be `support@glidedesign.com`

- First name will be `Glide`

- First name will be `Admin`

<br>

#### 👉 For Example

- `glideadmin`

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

### 📙 Admin Account for Client's Use

- Username will be `clientadmin`

- Email will be main point of contact for client `hello@clientwebsite.com`

- First name will be `Client`

- First name will be `Admin`

- If client needs further admin users, he can create those by logging into this user or we can assist them

<br>

#### 👉 For Example

- `clientadmin`

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

### 📙 Admin Accounts for Specific Glide Team

When project is launched we will need separate admin accounts for different teams. So that different teams can work on the project if needed.

We will be able to version control theme code with help of Github repository. But in order for us to know who did what content or images updates on specific environment after project is launched, wwe will need team specific WordPress admin accounts.

We will also maintain WordPress activity log for this purpose.

Following are guidelines on how to setup and name those team spcific admin accounts.

<br>

- Username will be combination of two words.

- First word in username will be `glide`

- Second word in username will be `teamname`

- There will be no dash in these two words to maintain similar naming scheme with other username types

- Email will be team specific email `teamname@glidedesign.com`

- First name will be `Glide`

- Last name will be `Team Name`

<br>

#### 👉 For Example

- `glidedev` can be username for Glide development team

<br>

> **Allowed**
>
> ✔️ `glidedev`
>
>  <br>
>
> **Not Allowed**
>
> ❌ `glide-dev` <br>
> ❌ `dev-admin` <br>
> ❌ `devadmin` <br>
> ❌ `glide-team`

<br>
<br>
<br>
<br>

![3](../assets/images/3.png)

## 3️⃣ - Github

Follow these guidelines for naming Github repository and its branches.

Each project will have its dedicated repository and it will be properly versioned and tagged during life time of the project.

<br>

### 📙 Github Repository

- It will be named same as project name

- It will be in lowercase and will have dashes instead of spaces

<br>

#### 👉 For Example

- If project name is `Great Client` repository will be named as `great-client`

<br>

> **Allowed**
>
> ✔️ `great-client`
>
>  <br>
>
> **Not Allowed**
>
> ❌ `greatclient` <br>
> ❌ `client` <br>
> ❌ `great` <br>
> ❌ `glide-great-client`

<br>
<br>

### 📙 Github Branches

Five different branch types will be used for git workflow.

> Guidelines on how to use different branch types in development Workflow is available here in [Github Branches Workflow](https://github.com/) document.

<br>

#### 📘 Master Branch

- Main branch will be named `master`

<br>

#### 👉 For Example

- `master`

<br>

> **Allowed**
>
> ✔️ `master`
>
>  <br>
>
> **Not Allowed**
>
> ❌ `main` <br>
> ❌ `dev` <br>
> ❌ `clientname` <br>
> ❌ `masterbranch`

<br>
<br>
<br>

#### 📘 Development Branch

- Active development branch will be named `development`

<br>

#### 👉 For Example

- `development`

<br>

> **Allowed**
>
> ✔️ `development`
>
>  <br>
>
> **Not Allowed**
>
> ❌ `dev` <br>
> ❌ `under-development` <br>
> ❌ `develop` <br>
> ❌ `developmentbranch`

<br>
<br>
<br>

#### 📘 Developer Specific Branches

- Developer branches will be named as a combination of two words

- First word will be first name of developer

- Second word will be date on which he is creating the branch

- Dash will be used as a separator

- Initials will help us to quickly see who created the branch

- Date will help us in to quickly identify how latest or old the branch is

- Date will always be in day(number)-month(initials) format for easy scanning and identification

- If we have to create multiple developer branches in same day, we will add roman numbering to end of it for easy identification

<br>

#### 👉 For Example

- `travis-03jul`
- `travis-15aug`
- `travis-15augi`

<br>

> **Allowed**
>
> ✔️ `travis-03jul`
>
>  <br>
>
> **Not Allowed**
>
> ❌ `tm-03jul21` <br>
> ❌ `travis-03jul2021` <br>
> ❌ `mcashan-03-06-21` <br>
> ❌ `travis-03-06`

<br>
<br>
<br>


#### 📘 Release Branches

- Release branches will be named as a combination of two words

- First word will be `release`

- Second word will be version number

- Dash will be used as a separator

- Version number will be in `1.0.0` format

<br>

#### 👉 For Example

- `release-1.0.0`

<br>

> **Allowed**
>
> ✔️ `release-1.0.0`
>
>  <br>
>
> **Not Allowed**
>
> ❌ `release1.0.0` <br>
> ❌ `release-v1.0.0` <br>
> ❌ `1.0.0` <br>
> ❌ `version-1.0.0`

<br>
<br>
<br>

#### 📘 Hotfix Branches

- Hotfix branches will be named as a combination of two words

- First word will be `hotfix`

- Second word will be date on which branch is created

- Dash will be used as a separator

- Date will help us in to quickly identify how latest or old the branch is

- Date will always be in day(number)-month(initials) format for easy scanning and identification

- If we have to create multiple hotfix branches in same day, we will add roman numbering to end of it for easy identification

<br>

#### 👉 For Example

- `hotfix-03jul`
- `hotfix-15aug`
- `hotfix-15augi`

<br>

> **Allowed**
>
> ✔️ `hotfix-03jul`
>
>  <br>
>
> **Not Allowed**
>
> ❌ `hf-03jul` <br>
> ❌ `fix-03jul` <br>
> ❌ `hot-03-06-21` <br>
> ❌ `hotfix-03-06`

<br>
<br>
<br>
<br>

![4](../assets/images/4.png)

## 4️⃣ - Local WP

Follow these guidelines for naming Local WP install.

If you fetch the website using Local WP built in pull feature, it will automatically use same details as on WP Engine `development environment`.

But if you are adding the Local WP site manually you need to follow the guidelines given below.

<br>

### 📙 Local Environment

- Local WP site name will be same as project name

- Local WP site domain will be same as project name

- It will be in lowercase lowercase and will have dashes instead of spaces

- Local WP site path will be same as project name

- It will be in lowercase lowercase and will have dashes instead of spaces

<br>

#### 👉 For Example

- For project name `Great Client` Local WP site name will become `Great Client`
- For project name `Great Client` Local WP site domain will become `great-client.local`
- For project name `Great Client` Local WP site path will become `local-sites/great-client`

<br>

> **Allowed**
>
> ✔️ `Great Client` <br>
> ✔️ `great-client`
>
>  <br>
>
> **Not Allowed**
>
> ❌ `GreatClient` <br>
> ❌ `greatclient` <br>
> ❌ `client` <br>
> ❌ `great`

<br>
<br>
<br>

### 📙 WordPress Accounts

No need to create WordPress admin accounts in `local environment`.

These will be fetched from `development environment` when you fetch the webiste or when you replace the local database.

<br>
<br>
<br>
<br>

![5](../assets/images/5.png)

## 5️⃣ - WordPress Theme

Follow these guidelines for naming WordPress Theme and its components.

<br>

### 📙 Theme Name

- Theme Name will be same as project name

<br>

#### 👉 For Example

- If project name is `Great Client` Local WP site name will become `Great Client`

<br>

> **Allowed**
>
> ✔️ `Great Client`
>
>  <br>
>
> **Not Allowed**
>
> ❌ `GreatClient` <br>
> ❌ `greatclient` <br>
> ❌ `client` <br>
> ❌ `glidetheme`

<br>
<br>
<br>

### 📙 Theme Folder

- Theme folder will be same as project name

- It will be in lowercase lowercase and will have dashes instead of spaces

<br>

#### 👉 For Example

- If project name is `Great Client` theme folder name will become `great-client`

<br>

> **Allowed**
>
> ✔️ `great-client`
>
>  <br>
>
> **Not Allowed**
>
> ❌ `GreatClient` <br>
> ❌ `greatclient` <br>
> ❌ `client-great` <br>
> ❌ `glidetheme`

<br>
<br>
<br>

### 📙 Function's Prefix

- Function's prefix will be derived from project name

- If project name is long, take first or second word from project name whichever makes sense and is unique

- It will be in lowercase and it will be separated with underscore

- Add an underscore at end also to separate it from actual function name

- Never use dash for separation

<br>

#### 👉 For Example

- If project name is `Great Client` function's prefix will become `great_client_`

<br>

> **Allowed**
>
> ✔️ `great_client_` <br>
> ✔️ `great_` <br>
> ✔️ `client_`
>
>  <br>
>
> **Not Allowed**
>
> ❌ `GreatClient_` <br>
> ❌ `great-client_` <br>
> ❌ `client-great_` <br>
> ❌ `glidefunction_`

<br>
<br>
<br>

### 📙 Text Domain

- Text domain will be derived from project name

- If project name is long, take first or second word from project name whichever makes sense and is unique

- It will be in lowercase and it will be separated with underscore

- Add `_td` to end of it for easy recognition and separating it from general functions prefix

- Add an underscore at end also to separate it from actual function name

- Never use dash for separation

<br>

#### 👉 For Example

- If project name is `Great Client` text domain will become `great_client_td`

<br>

> **Allowed**
>
> ✔️ `great_client_td` <br>
> ✔️ `great_td` <br>
> ✔️ `client_td`
>
>  <br>
>
> **Not Allowed**
>
> ❌ `GreatClient_td` <br>
> ❌ `great-client_td` <br>
> ❌ `great_client_textdomain` <br>
> ❌ `text_domain`

<br>
<br>
<br>
<br>
