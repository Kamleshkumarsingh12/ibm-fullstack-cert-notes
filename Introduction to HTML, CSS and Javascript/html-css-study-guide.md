# HTML & CSS Complete Study Guide

This document is a comprehensive guide to **HTML (HyperText Markup Language)** and **CSS (Cascading Style Sheets)**.  
It is designed as a one-stop reference for beginners and intermediate learners.

---

## 📌 Table of Contents
1. [Introduction](#introduction)
2. [HTML Basics](#html-basics)
   - [Structure of an HTML Document](#structure-of-an-html-document)
   - [HTML Elements & Tags](#html-elements--tags)
   - [Attributes](#attributes)
   - [Headings & Paragraphs](#headings--paragraphs)
   - [Formatting Text](#formatting-text)
   - [Lists](#lists)
   - [Links](#links)
   - [Images](#images)
   - [Tables](#tables)
   - [Forms](#forms)
   - [Semantic HTML](#semantic-html)
   - [Multimedia](#multimedia)
   - [HTML5 Features](#html5-features)
3. [CSS Basics](#css-basics)
   - [What is CSS?](#what-is-css)
   - [Ways to Add CSS](#ways-to-add-css)
   - [Selectors](#selectors)
   - [Colors](#colors)
   - [Units](#units)
   - [Box Model](#box-model)
   - [Positioning](#positioning)
   - [Flexbox](#flexbox)
   - [Grid](#grid)
   - [Typography](#typography)
   - [Backgrounds](#backgrounds)
   - [Borders & Shadows](#borders--shadows)
   - [Transitions & Animations](#transitions--animations)
   - [Responsive Design & Media Queries](#responsive-design--media-queries)
4. [Best Practices](#best-practices)
5. [Interview Questions](#interview-questions)
6. [Resources](#resources)

---

## Introduction
- **HTML**: The standard markup language for structuring web pages.
- **CSS**: Stylesheet language used to control layout and presentation.

Together they form the **foundation of web development**.

---

## HTML Basics

### Structure of an HTML Document
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>
<body>
  <h1>Hello World</h1>
</body>
</html>

HTML Elements & Tags
Elements are defined by tags.
Example: <p>Paragraph</p>

Attributes
Provide extra information about elements.
Example: <img src="image.jpg" alt="Description">

Headings & Paragraphs
Headings: <h1> to <h6>
Paragraph: <p>

Formatting Text
<b>, <strong> → Bold text
<i>, <em> → Italic text
<u> → Underline
<mark> → Highlight
<sup> <sub> → Superscript / Subscript

Lists
Ordered List: <ol><li>Item</li></ol>
Unordered List: <ul><li>Item</li></ul>
Description List: <dl><dt>Term</dt><dd>Definition</dd></dl>

Links
html
Copy code
<a href="https://example.com" target="_blank">Visit</a>
target="_blank" → Opens in new tab

Images
html

<img src="image.jpg" alt="Description" width="300" height="200">
Tables
html

<table border="1">
  <tr>
    <th>Name</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>John</td>
    <td>25</td>
  </tr>
</table>
-------------------------------------------------------------------
Forms
<form action="/submit" method="POST">
  <input type="text" name="username" placeholder="Enter name">
  <input type="password" name="password">
  <input type="submit" value="Submit">
</form>
Semantic HTML
<header>, <footer>, <article>, <section>, <nav>, <aside>
------------------------------------------------------------------
Multimedia
Images: <img>
Audio: <audio controls><source src="song.mp3"></audio>
Video: <video controls><source src="movie.mp4"></video>
------------------------------------------------------------------
 HTML5 Features
New input types: email, date, number, range
<canvas> for graphics
<svg> for vector graphics
<video> & <audio> for media
----------------------------------------------------------------------
CSS Basics
What is CSS?
CSS controls the style of HTML elements (colors, layout, fonts).
Ways to Add CSS
Inline: <p style="color:red;">
Internal: <style> p { color: red; } </style>
External: <link rel="stylesheet" href="style.css">

Selectors
Element: p { }
Class: .classname { }
ID: #idname { }
Universal: * { }
Grouping: h1, h2 { }
Descendant: div p { }

Pseudo-classes: a:hover, :first-child

Colors
Names (red)
HEX (#ff0000)
RGB (rgb(255,0,0))
RGBA (rgba(255,0,0,0.5))
HSL (hsl(0,100%,50%))

Units
Absolute: px
Relative: %, em, rem, vh, vw
Box Model
Each element has:
content
padding
borde
margin

Positioning
static, relative, absolute, fixed, sticky

Flexbox
Container: display: flex;

Main properties:
justify-content
align-items
flex-direction
flex-wrap
Grid

display: grid;
grid-template-columns: repeat(3, 1fr);
grid-gap: 10px;

Typography
font-family, font-size, font-weight
line-height, letter-spacing
text-align

Backgrounds
background-color
background-image: url("img.jpg")
background-size: cover

Borders & Shadows
border: 1px solid black;
border-radius: 10px;
box-shadow: 2px 2px 5px gray;
text-shadow: 1px 1px 3px black;

Transitions & Animations
css
div {
  transition: all 0.3s ease;
}
div:hover {
  transform: scale(1.2);
}
css
@keyframes slide {
  from { left: 0; }
  to { left: 100px; }
}
Responsive Design & Media Queries
css
@media (max-width: 600px) {
  body {
    background: lightblue;
  }
}

-----------------------------------------------------------------
Best Practices-
Always use semantic HTML for SEO & accessibility.
Keep CSS in external files for maintainability.
Use classes instead of IDs for styling.
Optimize images for performance.
Use relative units (em, rem) for responsiveness.

-----------------------------------------------------------------
Interview Questions
Difference between inline, inline-block, and block elements.
Difference between absolute, relative, fixed, and sticky positioning.
Explain the CSS box model.
What are pseudo-classes and pseudo-elements?
Difference between em, rem, %, vh, vw.
Difference between Flexbox and Grid.
What is semantic HTML?
Difference between == and === in HTML attributes (boolean ones).
Difference between inline, internal, and external CSS.
How does z-index work?

--------------------------------------------------------------------
Resources
MDN Web Docs - HTML
MDN Web Docs - CSS
W3Schools HTML
W3Schools CSS
CSS Tricks
