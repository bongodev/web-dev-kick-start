# HTML and CSS Learning Project: From Beginner to Advanced

## Table of Contents

1. [Introduction](#introduction)
2. [Getting Started](#getting-started)
3. [HTML Fundamentals](#html-fundamentals)
4. [Multimedia Elements](#multimedia-elements)
5. [Semantic HTML5](#semantic-html5)
6. [CSS Basics](#css-basics)
7. [Intermediate CSS](#intermediate-css)
8. [Advanced CSS Techniques](#advanced-css-techniques)
9. [Final Project](#final-project)
10. [Resources](#resources)

## Introduction

This comprehensive learning project will take you from a complete beginner to an advanced user of HTML and CSS. By the end of this course, you'll be able to create complex, responsive, and visually appealing web pages.

### What You'll Learn

- HTML markup from basic to advanced
- How to structure web content properly
- How to embed different types of media
- CSS styling techniques
- Layout strategies with flexbox and grid
- Advanced positioning and visual effects
- Modern responsive design practices

### How to Use This Project

Start from the beginning and work through each section sequentially. Complete all the exercises before moving on to ensure you've mastered each concept.

## Getting Started

### Setting Up Your Development Environment

1. **Text Editor**: Download Visual Studio Code (VS Code) or any text editor you prefer
2. **Browser**: Use Chrome or Firefox with developer tools enabled
3. **Create a Project Folder**: Set up a dedicated directory for your HTML and CSS files

### Creating Your First HTML File

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>My First Web Page</title>
  </head>
  <body>
    <h1>Hello, World!</h1>
    <p>This is my first web page.</p>
  </body>
</html>
```

**Exercise**: Create this file, save it as `index.html`, and open it in your browser.

## HTML Fundamentals

### Basic Structure

Every HTML document follows this basic structure:

- `<!DOCTYPE html>`: Declares the document type
- `<html>`: The root element
- `<head>`: Contains meta information
- `<body>`: Contains the visible content

### Text Elements

```html
<h1>Main Heading</h1>
<h2>Subheading</h2>
<h3>Sub-subheading</h3>
<p>This is a paragraph of text.</p>
<p>
  This is another paragraph with <strong>bold text</strong> and
  <em>italicized text</em>.
</p>
<blockquote>This is a blockquote.</blockquote>
```

**Exercise**: Create a page with different heading levels and paragraphs about your favorite hobby.

### Lists

```html
<!-- Ordered List -->
<ol>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
</ol>

<!-- Unordered List -->
<ul>
  <li>Apple</li>
  <li>Orange</li>
  <li>Banana</li>
</ul>

<!-- Definition List -->
<dl>
  <dt>HTML</dt>
  <dd>HyperText Markup Language</dd>
  <dt>CSS</dt>
  <dd>Cascading Style Sheets</dd>
</dl>
```

**Exercise**: Create a recipe page with an ingredient list and ordered instructions.

### Links

```html
<!-- Basic link -->
<a href="https://www.example.com">Visit Example Website</a>

<!-- Link to page section -->
<a href="#section1">Go to Section 1</a>

<!-- Link to local page -->
<a href="about.html">About Us</a>

<!-- Email link -->
<a href="mailto:example@example.com">Send Email</a>

<!-- Phone link -->
<a href="tel:+1234567890">Call Us</a>
```

**Exercise**: Create a simple navigation menu with links to different pages.

### Tables

```html
<table>
  <caption>
    Monthly Savings
  </caption>
  <thead>
    <tr>
      <th>Month</th>
      <th>Savings</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>January</td>
      <td>$100</td>
    </tr>
    <tr>
      <td>February</td>
      <td>$150</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td>Total</td>
      <td>$250</td>
    </tr>
  </tfoot>
</table>
```

**Exercise**: Create a table displaying a weekly schedule.

## Multimedia Elements

### Images

```html
<!-- Basic image -->
<img src="image.jpg" alt="Description of image" />

<!-- Image with dimensions -->
<img src="image.jpg" alt="Description of image" width="300" height="200" />

<!-- Image with title -->
<img src="image.jpg" alt="Description of image" title="This appears on hover" />

<!-- Responsive image -->
<img
  src="image.jpg"
  alt="Description of image"
  style="max-width:100%; height:auto;"
/>

<!-- Image with link -->
<a href="large-image.jpg">
  <img src="thumbnail.jpg" alt="Click to enlarge" />
</a>

<!-- Image map -->
<img
  src="workplace.jpg"
  alt="Workplace"
  usemap="#workmap"
  width="400"
  height="379"
/>
<map name="workmap">
  <area
    shape="rect"
    coords="34,44,270,350"
    alt="Computer"
    href="computer.htm"
  />
  <area shape="rect" coords="290,172,333,250" alt="Phone" href="phone.htm" />
  <area shape="circle" coords="337,300,44" alt="Coffee" href="coffee.htm" />
</map>
```

**Exercise**: Create a gallery page with at least 3 images, each with appropriate alt text.

### Video

```html
<!-- Basic video -->
<video src="movie.mp4" controls></video>

<!-- Video with multiple formats -->
<video controls width="320" height="240">
  <source src="movie.mp4" type="video/mp4" />
  <source src="movie.webm" type="video/webm" />
  Your browser does not support the video tag.
</video>

<!-- Video with poster image and autoplay -->
<video controls width="320" height="240" poster="poster.jpg" autoplay muted>
  <source src="movie.mp4" type="video/mp4" />
  Your browser does not support the video tag.
</video>

<!-- Responsive video container -->
<div
  style="position:relative; padding-bottom:56.25%; height:0; overflow:hidden;"
>
  <video
    style="position:absolute; top:0; left:0; width:100%; height:100%;"
    controls
  >
    <source src="movie.mp4" type="video/mp4" />
  </video>
</div>
```

**Exercise**: Embed a video on a page with custom controls and a fallback message.

### Audio

```html
<!-- Basic audio -->
<audio src="sound.mp3" controls></audio>

<!-- Audio with multiple formats -->
<audio controls>
  <source src="sound.ogg" type="audio/ogg" />
  <source src="sound.mp3" type="audio/mpeg" />
  Your browser does not support the audio element.
</audio>

<!-- Audio with autoplay and loop -->
<audio controls autoplay loop>
  <source src="background-music.mp3" type="audio/mpeg" />
</audio>
```

**Exercise**: Create an audio player for a podcast episode.

### iframes

```html
<!-- Basic iframe -->
<iframe src="https://www.example.com" width="600" height="400"></iframe>

<!-- YouTube video embed -->
<iframe
  width="560"
  height="315"
  src="https://www.youtube.com/embed/VIDEO_ID"
  title="YouTube video player"
  frameborder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
  allowfullscreen
></iframe>

<!-- Google Maps embed -->
<iframe
  src="https://www.google.com/maps/embed?pb=!1m18!1m12!..."
  width="600"
  height="450"
  style="border:0;"
  allowfullscreen=""
  loading="lazy"
></iframe>

<!-- Responsive iframe -->
<div
  style="position:relative; padding-bottom:56.25%; height:0; overflow:hidden;"
>
  <iframe
    style="position:absolute; top:0; left:0; width:100%; height:100%;"
    src="https://www.youtube.com/embed/VIDEO_ID"
    frameborder="0"
    allowfullscreen
  ></iframe>
</div>
```

**Exercise**: Create a page with an embedded map and YouTube video.

### Best Practices for Multimedia

- Always provide `alt` attributes for images
- Use responsive techniques for all media
- Compress images for faster loading
- Provide multiple formats for video and audio
- Be careful with autoplay features
- Consider accessibility for all media elements
- Use lazy loading for better performance: `<img loading="lazy" src="image.jpg" alt="Description">`

## Semantic HTML5

### Structural Elements

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Semantic HTML Example</title>
  </head>
  <body>
    <header>
      <h1>Website Title</h1>
      <nav>
        <ul>
          <li><a href="#home">Home</a></li>
          <li><a href="#about">About</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </nav>
    </header>

    <main>
      <section id="home">
        <h2>Home Section</h2>
        <p>Welcome to our website.</p>
      </section>

      <section id="about">
        <h2>About Section</h2>
        <article>
          <h3>Our Story</h3>
          <p>This is the story of our company.</p>
        </article>
        <article>
          <h3>Our Mission</h3>
          <p>This is our mission statement.</p>
        </article>
      </section>

      <aside>
        <h3>Related Information</h3>
        <p>Some additional information.</p>
      </aside>
    </main>

    <footer>
      <p>&copy; 2025 My Company</p>
    </footer>
  </body>
</html>
```

**Exercise**: Convert a non-semantic page to use proper semantic tags.

### Forms

```html
<form action="/submit-form" method="post">
  <fieldset>
    <legend>Personal Information</legend>

    <label for="name">Name:</label>
    <input type="text" id="name" name="name" required />

    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required />

    <label for="password">Password:</label>
    <input
      type="password"
      id="password"
      name="password"
      minlength="8"
      required
    />

    <label for="birthdate">Birth Date:</label>
    <input type="date" id="birthdate" name="birthdate" />
  </fieldset>

  <fieldset>
    <legend>Additional Information</legend>

    <label for="country">Country:</label>
    <select id="country" name="country">
      <option value="">--Please choose an option--</option>
      <option value="us">United States</option>
      <option value="ca">Canada</option>
      <option value="uk">United Kingdom</option>
    </select>

    <p>Preferred contact method:</p>
    <input type="radio" id="contact-email" name="contact" value="email" />
    <label for="contact-email">Email</label>

    <input type="radio" id="contact-phone" name="contact" value="phone" />
    <label for="contact-phone">Phone</label>

    <p>Interests:</p>
    <input
      type="checkbox"
      id="interest-tech"
      name="interests"
      value="technology"
    />
    <label for="interest-tech">Technology</label>

    <input
      type="checkbox"
      id="interest-sports"
      name="interests"
      value="sports"
    />
    <label for="interest-sports">Sports</label>

    <label for="message">Message:</label>
    <textarea id="message" name="message" rows="4" cols="30"></textarea>
  </fieldset>

  <button type="submit">Submit</button>
  <button type="reset">Reset</button>
</form>
```

**Exercise**: Create a registration form with various input types and validation.

### Advanced Form Elements

```html
<!-- Range slider -->
<label for="volume">Volume (between 0 and 100):</label>
<input type="range" id="volume" name="volume" min="0" max="100" step="1" />

<!-- Color picker -->
<label for="color">Choose a color:</label>
<input type="color" id="color" name="color" />

<!-- Date and time -->
<label for="meeting-time">Meeting time:</label>
<input type="datetime-local" id="meeting-time" name="meeting-time" />

<!-- File upload -->
<label for="profile-pic">Upload profile picture:</label>
<input type="file" id="profile-pic" name="profile-pic" accept="image/*" />

<!-- Progress bar -->
<label for="download">Download progress:</label>
<progress id="download" value="32" max="100">32%</progress>

<!-- Meter -->
<label for="disk-usage">Disk usage:</label>
<meter id="disk-usage" value="0.7" min="0" max="1">70%</meter>

<!-- Datalist for suggestions -->
<label for="browser">Choose your browser:</label>
<input list="browsers" id="browser" name="browser" />
<datalist id="browsers">
  <option value="Chrome"></option>
  <option value="Firefox"></option>
  <option value="Safari"></option>
  <option value="Edge"></option>
</datalist>
```

**Exercise**: Create an advanced form with range sliders, color pickers, and other HTML5 input types.

## CSS Basics

### Linking CSS

```html
<!-- External CSS -->
<link rel="stylesheet" href="styles.css" />

<!-- Internal CSS -->
<style>
  body {
    font-family: Arial, sans-serif;
  }
</style>

<!-- Inline CSS -->
<p style="color: blue; font-size: 16px;">This is a paragraph.</p>
```

### Selectors

```css
/* Element selector */
p {
  color: navy;
}

/* Class selector */
.highlight {
  background-color: yellow;
}

/* ID selector */
#header {
  background-color: black;
  color: white;
}

/* Descendant selector */
article p {
  font-style: italic;
}

/* Child selector */
ul > li {
  list-style-type: square;
}

/* Adjacent sibling selector */
h2 + p {
  font-weight: bold;
}

/* Attribute selector */
input[type='text'] {
  border: 1px solid gray;
}

/* Pseudo-class */
a:hover {
  text-decoration: none;
}

/* Pseudo-element */
p::first-letter {
  font-size: 2em;
}
```

**Exercise**: Create a CSS file with different types of selectors to style a simple HTML page.

### Colors and Typography

```css
/* Colors */
.box1 {
  color: red; /* Named color */
  background-color: #f0f0f0; /* Hex color */
}

.box2 {
  color: rgb(0, 128, 255); /* RGB color */
  background-color: rgba(0, 128, 255, 0.5); /* RGB with alpha */
}

.box3 {
  color: hsl(120, 100%, 50%); /* HSL color */
  background-color: hsla(120, 100%, 50%, 0.3); /* HSL with alpha */
}

/* Typography */
body {
  font-family: 'Helvetica', Arial, sans-serif;
  font-size: 16px;
  line-height: 1.5;
}

h1 {
  font-family: 'Georgia', serif;
  font-weight: bold;
  font-size: 2.5em;
  text-transform: uppercase;
  letter-spacing: 2px;
}

p {
  text-align: justify;
  text-indent: 2em;
  word-spacing: 2px;
}

.fancy-text {
  font-style: italic;
  text-decoration: underline;
  text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.3);
}
```

**Exercise**: Create a typography stylesheet for a blog, using different font properties.

### Box Model

```css
.box {
  /* Content width and height */
  width: 300px;
  height: 200px;

  /* Padding (inner space) */
  padding-top: 10px;
  padding-right: 20px;
  padding-bottom: 10px;
  padding-left: 20px;
  /* Or shorthand: */
  padding: 10px 20px; /* top/bottom right/left */

  /* Border */
  border-width: 2px;
  border-style: solid;
  border-color: black;
  /* Or shorthand: */
  border: 2px solid black;

  /* Border radius */
  border-radius: 10px;

  /* Margin (outer space) */
  margin-top: 20px;
  margin-right: 10px;
  margin-bottom: 20px;
  margin-left: 10px;
  /* Or shorthand: */
  margin: 20px 10px; /* top/bottom right/left */

  /* Box sizing */
  box-sizing: border-box; /* Width/height includes padding and border */
}
```

**Exercise**: Create different boxes with various border styles, padding, and margins.

### Styling Form Elements

```css
/* Base form styling */
form {
  max-width: 500px;
  margin: 0 auto;
  padding: 20px;
  background-color: #f5f5f5;
  border-radius: 8px;
}

/* Label styling */
label {
  display: block;
  margin-bottom: 5px;
  font-weight: bold;
}

/* Input fields */
input[type='text'],
input[type='email'],
input[type='password'],
select,
textarea {
  width: 100%;
  padding: 10px;
  margin-bottom: 15px;
  border: 1px solid #ddd;
  border-radius: 4px;
  box-sizing: border-box;
}

/* Focus state */
input:focus,
select:focus,
textarea:focus {
  border-color: #4a90e2;
  outline: none;
  box-shadow: 0 0 5px rgba(74, 144, 226, 0.5);
}

/* Button styling */
button,
input[type='submit'],
input[type='reset'] {
  background-color: #4a90e2;
  color: white;
  padding: 10px 15px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  font-size: 16px;
}

button:hover,
input[type='submit']:hover,
input[type='reset']:hover {
  background-color: #357abd;
}

/* Checkbox and radio styling */
input[type='checkbox'],
input[type='radio'] {
  margin-right: 10px;
}

/* Fieldset styling */
fieldset {
  margin-bottom: 20px;
  padding: 15px;
  border: 1px solid #ddd;
  border-radius: 4px;
}

legend {
  padding: 0 10px;
  font-weight: bold;
}
```

**Exercise**: Style the form you created in the HTML forms exercise.

## Intermediate CSS

### Flexbox

```css
/* Basic flex container */
.flex-container {
  display: flex;
  /* Main axis direction */
  flex-direction: row; /* row, row-reverse, column, column-reverse */

  /* Wrapping behavior */
  flex-wrap: wrap; /* nowrap, wrap, wrap-reverse */

  /* Shorthand for direction and wrap */
  flex-flow: row wrap;

  /* Main axis alignment */
  justify-content: space-between; /* flex-start, flex-end, center, space-around, space-evenly */

  /* Cross axis alignment */
  align-items: center; /* flex-start, flex-end, center, stretch, baseline */

  /* Multi-line alignment */
  align-content: space-between; /* flex-start, flex-end, center, space-around, space-between, stretch */
}

/* Flex items */
.flex-item {
  /* Order (default is 0) */
  order: 2;

  /* Flex grow factor (default is 0) */
  flex-grow: 1;

  /* Flex shrink factor (default is 1) */
  flex-shrink: 0;

  /* Default size */
  flex-basis: 200px;

  /* Shorthand for grow, shrink, and basis */
  flex: 1 0 200px;

  /* Self alignment (overrides container's align-items) */
  align-self: flex-start; /* auto, flex-start, flex-end, center, baseline, stretch */
}
```

**Exercise**: Create a responsive navigation bar using flexbox.

### CSS Grid

```css
/* Basic grid container */
.grid-container {
  display: grid;

  /* Define columns */
  grid-template-columns: 1fr 2fr 1fr; /* Three columns with 1:2:1 ratio */

  /* Define rows */
  grid-template-rows: 100px auto 100px; /* Fixed height header/footer, auto content */

  /* Gap between cells */
  column-gap: 20px;
  row-gap: 10px;
  /* Or shorthand: */
  gap: 10px 20px; /* row-gap column-gap */

  /* Named areas */
  grid-template-areas:
    'header header header'
    'sidebar content content'
    'footer footer footer';

  /* Alignment of all items */
  justify-items: center; /* start, end, center, stretch */
  align-items: center; /* start, end, center, stretch */

  /* Alignment of the grid within its container */
  justify-content: space-between; /* start, end, center, stretch, space-around, space-between, space-evenly */
  align-content: space-between; /* start, end, center, stretch, space-around, space-between, space-evenly */
}

/* Grid items */
.grid-item {
  /* Placement by lines */
  grid-column-start: 1;
  grid-column-end: 3; /* or span 2 */
  /* Shorthand: */
  grid-column: 1 / 3; /* or 1 / span 2 */

  grid-row-start: 1;
  grid-row-end: 3; /* or span 2 */
  /* Shorthand: */
  grid-row: 1 / 3; /* or 1 / span 2 */

  /* Placement by area name */
  grid-area: header;

  /* Self alignment (overrides container's alignment) */
  justify-self: end; /* start, end, center, stretch */
  align-self: start; /* start, end, center, stretch */
}

/* Complex grid layout example */
.complex-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-template-rows: auto;
  grid-template-areas:
    'header header header header'
    'sidebar main main main'
    'sidebar main main main'
    'footer footer footer footer';
}

.header {
  grid-area: header;
}
.sidebar {
  grid-area: sidebar;
}
.main {
  grid-area: main;
}
.footer {
  grid-area: footer;
}
```

**Exercise**: Create a responsive grid layout for a portfolio page.

### CSS Positioning

```css
/* Static positioning (default) */
.static {
  position: static;
}

/* Relative positioning */
.relative {
  position: relative;
  top: 20px;
  left: 20px;
}

/* Absolute positioning */
.absolute {
  position: absolute;
  top: 20px;
  right: 20px;
  bottom: 20px;
  left: 20px;
}

/* Fixed positioning */
.fixed {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  background-color: white;
  z-index: 100;
}

/* Sticky positioning */
.sticky {
  position: sticky;
  top: 20px; /* Sticks when scrolled to this position */
}
```

**Exercise**: Create a webpage with a fixed header, a sidebar, and a sticky call-to-action button.

### Media Styling

```css
/* Basic image styling */
img {
  max-width: 100%;
  height: auto;
  border-radius: 8px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.3);
}

/* Image filters */
.filtered-image {
  filter: grayscale(50%) brightness(110%) contrast(120%);
  transition: filter 0.3s ease;
}

.filtered-image:hover {
  filter: grayscale(0%) brightness(100%) contrast(100%);
}

/* Video container */
.video-container {
  position: relative;
  padding-bottom: 56.25%; /* 16:9 aspect ratio */
  height: 0;
  overflow: hidden;
}

.video-container iframe,
.video-container video {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  border: none;
}

/* Audio player styling */
audio {
  width: 100%;
  margin: 10px 0;
}

/* iframe styling */
iframe {
  border: 2px solid #ddd;
  border-radius: 4px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
}

/* Background images */
.hero {
  background-image: url('hero.jpg');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  height: 400px;
}

/* Multiple background images */
.complex-bg {
  background-image: url('overlay.png'), linear-gradient(
      rgba(0, 0, 0, 0.5),
      rgba(0, 0, 0, 0.5)
    ), url('background.jpg');
  background-size: auto, cover, cover;
  background-position: center, center, center;
  height: 500px;
}

/* Image gallery with CSS Grid */
.gallery {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
  gap: 16px;
}

.gallery img {
  width: 100%;
  height: 200px;
  object-fit: cover;
  transition: transform 0.3s ease;
}

.gallery img:hover {
  transform: scale(1.05);
}
```

**Exercise**: Create a responsive media gallery with image filtering effects.

## Advanced CSS Techniques

### Z-index and Stacking Context

```css
/* Basic z-index */
.layer1 {
  position: relative; /* z-index only works on positioned elements */
  z-index: 1; /* Higher value appears on top */
}

.layer2 {
  position: relative;
  z-index: 2; /* This will appear above layer1 */
}

/* Creating a stacking context */
.stacking-context {
  position: relative;
  z-index: 10;
  /* The following also create stacking contexts: */
  /* opacity: 0.99; */
  /* transform: translateZ(0); */
  /* will-change: transform; */
  /* filter: blur(0); */
}

/* Children of a stacking context are confined to that context */
.stacking-context .child {
  position: relative;
  z-index: 1000; /* High value, but still contained within parent */
}

.outside-element {
  position: relative;
  z-index: 5; /* Lower than stacking-context, but will appear above its children */
}
```

**Exercise**: Create a layered interface with overlapping elements using z-index.

### Responsive Design

```css
/* Mobile-first approach */
.container {
  width: 100%;
  padding: 15px;
}

/* Responsive typography */
html {
  font-size: 16px; /* Base font size */
}

h1 {
  font-size: 1.5rem; /* 24px on default settings */
}

/* Media queries */
/* Small devices (landscape phones) */
@media (min-width: 576px) {
  .container {
    max-width: 540px;
    margin: 0 auto;
  }

  h1 {
    font-size: 2rem; /* 32px on default settings */
  }
}

/* Medium devices (tablets) */
@media (min-width: 768px) {
  .container {
    max-width: 720px;
  }
}

/* Large devices (desktops) */
@media (min-width: 992px) {
  .container {
    max-width: 960px;
  }
}

/* Extra large devices */
@media (min-width: 1200px) {
  .container {
    max-width: 1140px;
  }
}

/* Print styles */
@media print {
  .no-print {
    display: none;
  }

  body {
    font-size: 12pt;
    line-height: 1.5;
    color: #000;
    background: #fff;
  }

  a {
    text-decoration: underline;
    color: #000;
  }

  a[href]:after {
    content: ' (' attr(href) ')';
  }
}

/* Responsive images */
.responsive-img {
  max-width: 100%;
  height: auto;
}

/* Using viewport units */
.viewport-element {
  width: 50vw; /* 50% of viewport width */
  height: 50vh; /* 50% of viewport height */
  padding: 2vmin; /* 2% of viewport's smaller dimension */
}

/* Using calc() */
.sidebar {
  width: calc(100% - 80px);
}

@media (min-width: 768px) {
  .sidebar {
    width: calc(30% - 20px);
  }

  .main-content {
    width: calc(70% - 20px);
  }
}
```

**Exercise**: Create a fully responsive webpage that adapts to different screen sizes.

### CSS Animations and Transitions

```css
/* Basic transition */
.button {
    background-color: blue;
    color:
```
