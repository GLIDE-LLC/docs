<br>
<br>
<br>

![Glide Design](../assets/images/glide.png)

<br>
<br>
<br>

# Glide Performance Framework

<br>

Complete framework for ensuring **Performance Optimization** of Glide projects.

This framework includes guidelines according to `WCAG 2.0` & `WCAG 2.1` - `Level A`. These rules must be followed to make Glide projects accessible.

This document breaks it down to the responsibility level, making it easier for everyone involved in a project to achieve accessibility compliance.

<br>

#### Rule for Success

⚠️ Its important that we start discussing performance with our clients at start of projects. This is not something to consider while project is already in review phase.

<br>
<br>

| #  | Topics |
|----|-------|
| 01 | [Responsibilities of Project Manager](https://github.com/abubakar-me/glide-design/blob/master/glide-performance-framework/README.md#1%EF%B8%8F%E2%83%A3---responsibilities-of-project-manager) |
| 02 | [Defining the Performance Budget](https://github.com/abubakar-me/glide-design/blob/master/glide-performance-framework/README.md#2%EF%B8%8F%E2%83%A3---defining-the-performance-budget) |
| 03 | [Responsibilities of Designer](https://github.com/abubakar-me/glide-design/blob/master/glide-performance-framework/README.md#3%EF%B8%8F%E2%83%A3---responsibilities-of-designer) |
| 04 | [Responsibilities of Developer](https://github.com/abubakar-me/glide-design/blob/master/glide-performance-framework/README.md#4%EF%B8%8F%E2%83%A3---responsibilities-of-developer) |
|    | [&nbsp; &nbsp; &nbsp; &nbsp;Setting up best environment for performance](https://github.com/abubakar-me/glide-design/blob/master/glide-performance-framework/README.md#-setting-up-best-environment-for-performance) |
|    | [&nbsp; &nbsp; &nbsp; &nbsp;Coding best theme for performance](https://github.com/abubakar-me/glide-design/blob/master/glide-performance-framework/README.md#-coding-best-theme-for-performance) |
| 05 | [Responsibilities of Content Editor](https://github.com/abubakar-me/glide-design/blob/master/glide-performance-framework/README.md#5%EF%B8%8F%E2%83%A3---responsibilities-of-content-editor) |
| 06 | [Performance Tools & Resources](https://github.com/abubakar-me/glide-design/blob/master/glide-performance-framework/README.md#6%EF%B8%8F%E2%83%A3---performance-tools--resources) |


<br>
<br>
<br>
<br>

![1](../assets/images/1.png)

## 1️⃣ - Responsibilities of Project Manager

<br>

> ✔️ Project managers should follow this process and convey everything clearly to client.

<br>

👉 Guide client on performance and performance budget


	 ▪️  Performance is an important part of the user experience and it affects business metrics

	 ▪️  Performance should be one of the first things a team considers in planning a website

	 ▪️  Start the journey by setting a performance budget

	 ▪️  A performance budget is a set of limits imposed on metrics that affect site performance

	 ▪️  This could be the total size of a page, the time it takes to load on a mobile network, or even the number of HTTP requests that are sent

	 ▪️  Defining a budget helps get the web performance conversation started

	 ▪️  It serves as a point of reference for making decisions about design, technology, and adding features


<br>

👉 Guide client on benefits and need for performance and performance budget


	 ▪️  Increased conversion rates, page views, reduced bounce rates and even better search engine rankings

	 ▪️  Shopzilla reduced page load times from 7 seconds to 2 seconds and saw a 12% increase in conversion rate

	 ▪️  If Amazon increased page load time by +100ms they lose 1% of sales

	 ▪️  (+100ms = 1 marketing pixel / third party script)

	 ▪️  If Google increased page load by +500 ms they get 25% fewer searches

	 ▪️  52% of online shoppers claim that quick page loads are important for their loyalty to a site


<br>

👉 Agree upon a performance level with the client

<br>

👉 Set clear expectations and performance goals with client

<br>

👉 Convey performance goals to the design and development team

<br>
<br>
<br>
<br>

![2](../assets/images/2.png)

## 2️⃣ - Defining the Performance Budget

<br>

> ✔️ This is a collective team effort which will most likely be lead by development team.

<br>

### 📙 Analysis

- Review Google Analytics data

- Review Search Console data

- Create list of important pages

- Perform priliminary analysis

- Perform competitive analysis

<br>

### 📕 Devise Budgets

- Devise budget for timing milestones

- Devise budget for quantity-based metrics

- Devise budget for rule-based metrics

- Devise budget for core web vitals

<br>

### 📗 Devise Rules

- Devise rules for images

- Devise rules for fonts

- Devise rules for videos

- Devise rules for scripts

- Devise rules for animations and effects

<br>
<br>
<br>
<br>

![3](../assets/images/3.png)

## 3️⃣ - Responsibilities of Designer

<br>

👉 Review performance budget and rules

<br>

👉 Adhere to performance budget while designing different pages of the website

<br>

👉 Adhere to image rules set in performance budget

<br>

👉 Adhere to font rules set in performance budget

<br>

👉 Adhere to video rules set in performance budget

<br>
<br>
<br>
<br>

![4](../assets/images/4.png)

## 4️⃣ - Responsibilities of Developer

<br>

> ✔️ Developer should follow these guidelines to ensure performance optimization.

<br>
<br>

### 👉 Setting up best environment for performance

<br>

### 📙 Server

- Keep the server response time short

- Use HTTP/2

- Enable keep-alive

- Use Latest PHP Version

<br>

### 📕 Redirects

- Avoid multiple page redirects

<br>

### 📗 WordPress

- Keep WordPress updated

- Don’t upload videos directly to WordPress

- Split comments into pages

- Use excerpts on homepage and archive pages

- Split long posts into pages

- Fix SSL errors

- Turn off pingbacks and trackbacks, if not using

- Disable hotlinking and leeching of content

- Disable WordPress embeds

<br>

### 📘 Plugins

- Remove high resource plugins

- Remove unused, outdated, and otherwise unnecessary plugins

- Only use optimized and reliable plugins

<br>

### 📙 Database

- Cleanup WordPress database

- Reduce database calls

- Limit post revisions

- Perform routine database maintenance


		Optimize Database Tables
		Remove Post Revisions
		Remove Auto-draft Posts
		Clear Trash Posts
		Remove Unused Posts Metadata
		Clear Unapproved Comments
		Remove Spam Comments
		Clear Trash Comments
		Remove Unused Comments Metadata
		Remove Pingbacks
		Remove Trackbacks


<br>

### 📕 WP Rocket

- Install cache plugin

- Configure cache plugin

<br>

### 📗 Cache

- Use efficient cache policy on static assets

- Add expiry headers

<br>

### 📘 CDN

- Use a content delivery network

<br>
<br>

### 👉 Coding best theme for performance

<br>

### 📙 Requests

- Keep request counts low and transfer sizes small

- Avoid enormous network payloads

- Avoid chaining critical requests

- Preload key requests

<br>

### 📕 HTML

- Enable gzip compression

- Avoid an excessive DOM size

<br>

### 📗 CSS

- Minify CSS

- Remove unused CSS

- Avoid large layout shifts

- Eliminate render-blocking CSS

- Avoid CSS import

- Combine images using CSS sprites

- Inline small CSS

- Add critical path CSS

<br>

### 📘 Javascript

<br>

- Minify JavaScript

- Remove unused JavaScript

- Remove duplicate modules in JavaScript bundles

- Avoid serving legacy JavaScript to modern browsers

- Avoid document.write()

- Reduce time spent parsing, compiling, and executing JS

- Avoid long main-thread tasks

- Minimizes main-thread work

- Use passive listeners to improve scrolling performance

- Preload Largest Contentful Paint element

- Eliminate render-blocking Javascript

- Inline small Javascript

- Use asynchronous scripts

- Defer parse Javascript

- Delay Javascript execution

- Instrument your app with the User Timing API

<br>

### 📙 Images

- Properly size images

- Defer offscreen images

- Efficiently encode images

- Serve images in next-gen formats

- Add explicit width and height to images

- Preload Largest Contentful Paint image

- Install WordPress image optimization plugin

- Enable lazy load for images (if needed)

- Enable lazy load for iframes and videos (if needed)

<br>

### 📕 Animations

- Avoid non-composited animations

- Use video formats for animated content

<br>

### 📗 Fonts

- Preload fonts

- Use font display API

- Ensure that there are no flashes of invisible text

- Ensure that all text remains visible during webfont load

<br>

### 📘 Third Party

- Minimize third-party usage

- Lazy load third-party resources with facades

- Preconnect to required origins

<br>
<br>
<br>
<br>

![5](../assets/images/5.png)

## 5️⃣ - Responsibilities of Content Editor

<br>

> ✔️ Content editors should follow these guidelines when working with content.

<br>

### 📙 General

- Avoid using too many plugins

- Dont use custom fonts for styling

<br>

### 📕 Images

- Always use webp images

- Optimize images before uploading

- Always use properly sized images

<br>

### 📗 Videos

- Optimize videos before uploading

- Host video content to third party services

- Don’t upload videos directly to WordPress

<br>

### 📘 Content

- Avoid creating very lengthy pages

- Split long posts into pages (if possible)

<br>

### 📙 Testing

- Test page size after adding content and images

- Adhere to page size rules set in performance budget

- Adhere to image rules set in performance budget

<br>
<br>
<br>
<br>

![6](../assets/images/6.png)

## 6️⃣ - Performance Tools & Resources

> ✔️ Useful resources for everyone on team.

<br>

### 📙 Performance Testing Tools

- [Page Speed](https://developers.google.com/speed/pagespeed/insights/) <br>
Google Page Speed Insights Test

- [Lighthouse](https://chrome.google.com/webstore/detail/lighthouse/blipmdconlkpinefehnmjammfjpmpbjk?hl=en) <br>
Google Lighthouse - Chrome Extension

- [GT Metrix](https://gtmetrix.com/) <br>
GT Metrix Website Speed Test

- [Pingdom](https://tools.pingdom.com/) <br>
Pingdom Website Speed Test

- [Web Page Test](https://www.webpagetest.org/) <br>
Web Page Performance & Optimization Test

<br>

### 📕 Learn Performance Optimization

- [Web Dev](https://web.dev/)  <br>
Learn performance optimization techniques

- [WPO Stats](https://wpostats.com/) <br>
Performance case studies and experiements

<br>

### 📗 Budget Calculators

- [Budget Calculator 1](https://www.performancebudget.io/) <br>
Interactive performance budget calculator

- [Budget Calculator 2](https://perf-budget-calculator.firebaseapp.com/) <br>
Interactive performance budget calculator

<br>

### 📘 Budget Monitoring Services

- [Speed Curve](https://www.speedcurve.com/) <br>
Performance budget monitoring service

- [Calibre](https://calibreapp.com/) <br>
Performance budget monitoring service

<br>

### 📙 Image / Video Tools

- [TinyPNG](https://tinypng.com/) <br>
WebP Image Compressor

- [Cloud Convert](https://cloudconvert.com/webp-converter) <br>
WebP Image Converter

- [Free Convert](https://www.freeconvert.com/video-compressor) <br>
Video Compressor

<br>
<br>
<br>
<br>

⚠️ Its critical that all project team members follow these guidelines according to their role to ensure performance optimization.

<br>
<br>
<br>

Happy Performance!

<br>

**Prepared by:**
Muhammad AbuBakar

<br>
<br>
