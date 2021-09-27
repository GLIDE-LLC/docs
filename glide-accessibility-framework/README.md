<br>
<br>
<br>

![Glide Design](../assets/images/glide.png)

<br>
<br>
<br>

# Glide Accessibility Framework

<br>

Complete framework for ensuring **Accessibility** of Glide projects.

This framework includes guidelines according to `WCAG 2.0` & `WCAG 2.1` `Level A`. These rules must be followed to make Glide projects accessible.

This document breaks it down to the responsibility level, making it easier for everyone to implement overall accessibility framework.

<br>
<br>

| #  | Topics |
|----|-------|
| 01 | [Responsibilities of Designers](https://github.com/abubakar-me/glide-design/tree/master/glide-accessibility-framework#1%EF%B8%8F%E2%83%A3---responsibilities-of-designers) |
| 02 | [Responsibilities of Designers](https://github.com/abubakar-me/glide-design/tree/master/glide-accessibility-framework#2%EF%B8%8F%E2%83%A3---responsibilities-of-developers) |
| 03 | [Responsibilities of Content Editors](https://github.com/abubakar-me/glide-design/tree/master/glide-accessibility-framework#3%EF%B8%8F%E2%83%A3---responsibilities-of-content-editors) |

<br>
<br>
<br>
<br>

![1](../assets/images/1.png)

## 1️⃣ - Responsibilities of Designers

> ✔️ This is live website, this is only meant for public view

<br>

### 📙 Headings

- Break up content into hierarchical logical chunks

- Add heading at the start of all areas of content

<br>

### 📙 Links

- Ensure the link text describes the destination

- Link text should not be empty

- Do not use ambigous link names

- Ensure text links are clearly distinguished

- Distinguish links by either undelining them or by use of icons

- Do not rely solely on color to identify links

- If only color is used to distinghuish links, provide high contrast of at least `3:1` ratio

<br>

### 📙 Color & Contrast

- Do not use only color to convey important information

- Do not use only shapes and designs to convey important information

- Ensure `foreground` vs. `background` contrast ratio is at least `4.5:1`

<br>

### 📙 Page Layout

- Avoid complex page layouts

- Use labels, controls, status indicators, and other UI elements for easy accessibility

- If a UI element is designed or named in a specific way, ensure that it is used consistently

- Avoid horizontal scrolling of elements

- Add a descriptive page title for every page

- Ensure that the target size for elements is large enough to easily activate with a finger or mouse pointer

<br>

### 📙 Forms

- Provide visible form labels

- Display labels in close proximity to the form elements

- Group related form elements and provide description

- Clearly identify required form elements

- Properly design form errors

- Do not use only color to identify errors

<br>

### 📙 Tables

- Add table headers to tabular content

<br>
<br>
<br>
<br>

![2](../assets/images/2.png)

## 2️⃣ - Responsibilities of Developers

<br>

> ✔️ This is staging website to review changes and updates

<br>

### 📙 HTML Validity

- Use complete start and end tags for elements

- Nest elements according to their specifications

- Do not add duplicate attributes to elements

- Use unique IDs for elements

- Pass W3C HTML validation test

<br>

### 📙 HTML Structure

- Add language tag on every page

- Use proper HTML markup for different content types

- Use only one `<h1>` per page 

- Hierarchically order heading tags `<h1>` `<h2>` `<h3>`

- Do not use tables for positional layout

- Use `<ul>` and `<ol>` list tags for content lists

- Use logical tabbing order for the page elements

- Make page contents understandable without stylesheets

<br>

### 📙 Page Title

- Add descriptive & unique meta title on every page

- Use `<page name> - <site name>` format for page title

<br>

### 📙 Forms

- Add labels for all input fields

- Group related form inputs with `<fieldset>` tag

- Add description for fieldsets with `<legend>` tag

- Clearly identify required fields

- Provide examples of correct input

- All form elements should be keyboard accessible

- Do not use CAPTCHA that relies on visual identification

<br>

### 📙 Form Errors

- Add error messages for all input fields

- Describe the specific input errors

- Do not use only color to identify errors

- Use `ARIA` to connect the input field and the error message

- Add aria-invalid=false attribute to the input field with error

- Add `aria-describedby="[id of element with error message]"` attribute to the input field with error

- Add `role="alert"` attribute to the element with the error message

<br>

### 📙 Tables

- Use proper table markup for tabular content

- Add scope attributes in tables `<th scope="row/col">`

- Use colgroup and rowgroup scope for table headers

<br>

### 📙 Images

- Use CSS methods for displaying decorative images

- Use image tag only for displaying meaningful content images

- Provide a method to add alt text to `<img>` tags

- Decorative images should have `"null"` as alt text

- For on screen description of an image use `<figcaption>` tag

<br>

### 📙 Links

- Use `<button>` tag for elements that perform a function

- Use `<a>` tag for elements that load new page

- Add taget attribute to links for description purpose

- Use progressive enhancement for opening links in new window

- Add tab index to clickable `<div>` or wrap it with `<a>` tag

<br>

### 📙 Navigation

- Use unordered list markup for menu items

- Use unordered lists within unordered lists for heirarchical meunus

- Add link to skip navigation and go to content directly

- Link should only be visible to screen readers

- Link should appear on keyboard focus

<br>

### 📙 Keyboard

- Ensure that the page is keyboard accessible

- Ensure that the interactive elements are accessible through keyboard

- Ensure that the HTML content in the DOM is in logical order

- Add visible focus indicator to all keyboard accessible elements

- Avoid unexpected actions when an element gets keyboard focus

- Avoid unexpected actions when an element gets changed
  
<br>

### 📙 Zoomability

- Ensure that users can enlarge browser text upto `200%` without breaking the page functionality

<br>

### 📙 Errors

- Properly style and mark error messages
  
<br>

### 📙 Dynamic Content

- If an element shows new content, ensure that the content follows the activating element in the DOM

- Ensure the content changes and status messages are conveyed to assistive technology

- Provide ability to pause slideshows and carousels
  
<br>

### 📙 ARIA

- Prefer use of standard HTML elements over custom `ARIA` elements

- Correctly apply `ARIA` attributes on the right elements

- No `ARIA` is better than bad `ARIA`
  
<br>

### 📙 Audio / Video

- Provide Audio / Video media controls

- Provide method to add titles

- Provide method to add descriptions and transcripts

<br>
<br>
<br>
<br>

![3](../assets/images/3.png)

## 3️⃣ - Responsibilities of Content Editors

<br>

> ✔️ This is development website to develop new code, this is meant for developers only

<br>

### 📙 Images

- Provide meaningful alt text for all images

- Provide captions for images if required
  
<br>

### 📙 Links

- Provide descriptive text for <a> tags

- Provide descriptive titles for links
  
<br>
	
### 📙 Audio / Video

- Provide a descriptive title attribute for audio / video

- Provide audio descriptions, transcripts for audio / video

- Provide captioning for audio / video
  
<br>

### 📙 PDF

- In addition to PDFs, also provide HTML, Word, and EPUB3 versions

- Ensure that PDFs are properly tagged
  
<br>

### 📙 Machine Readability

- Use web technologies that are compatible with screen readers

- Use HTML markup for any text content, don't use images

- Use MathML for math content

- Use Highcharts for graphs and charts

- Use Able Player as a media player for video and audio content

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
