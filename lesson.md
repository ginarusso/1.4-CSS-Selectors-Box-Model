## Brief

### Lesson Overview

The first half of the lesson will be focusing on block and inline HTML elements. A mini activity will help the learners identify what elements are block or inline. The next half of the lesson will focus on semantic HTML to describe different parts of a webpage to both the browser and the developer.

---

## Part 1 - HTML Block and Inline

Every HTML element has a default display value, depending on what type of element it is.

There are two display values: block and inline.

### Block elements

Block-level elements always start on a new line, and the browsers automatically add some space / margin before and after the element. They always takes up the full width available on the browser window.

Block elements can be imagined as children's blocks stacked one on top of the other.

Two commonly used block elements are: ```<p>``` and ```<div>```.

The ```<p>``` element defines a paragraph in an HTML document.

The ```<div>``` element defines a division or a section in an HTML document. It is often used as a container for other HTML elements.

The ```<div>``` element has no required attributes, but style, class and id are common.

When used together with CSS, the ```<div>``` element can be used to style blocks of content.

```html
<!-- index.html -->
<p>A paragraph is a block-level element. Even if the text doesn't reach the end of the screen...</p>
<p>The next paragraph will be separated to a new line</p>
<div>Another block element is a div. It denotes a division or section of HTML code</div>
<div>
    <p>Multiple elements can be nested inside a div, even other divs.</p>
    <p>However, be mindful of how divs can be nested, else there will be what is called a "div soup"</p>
</div>
```

### Inline elements

Inline elements do not start on a new line. Each inline element only takes up as much width as necessary.

Inline elements can be imagined as children's blocks side by side each other.

The common used inline element is the ```<span>``` element.

The ```<span>``` element is an inline container used to mark up a part of a text, or a part of a document. It has no required attributes, but style, class and id are common.

When used together with CSS, the ```<span>``` element can be used to style parts of the text.

```html
<!-- index.html -->
<span>This is a span.</span>
<span>This is another span.</span>
<span>Notice how each span appears side by side each other.</span>
```

### Mini exercise

Identify which elements are block or inline:

```
<form>
<table>
<input>
<a>
<h1>
<nav>
<img>
<button>
<textarea>
<ol>
<li>
<strong>
<em>
<label>
<ul>
```
---

## Part 2 - Semantic HTML

Semantic elements clearly describe their meaning and content.

Examples of non-semantic elements: ```<div>``` and ```<span>``` - Tells nothing about its content.

Examples of semantic elements: ```<form>```, ```<table>```, and ```<article>``` - Clearly defines its content.

Many web sites contain HTML code like: ```<div id="nav"> <div class="header"> <div id="footer">``` to indicate navigation, header, and footer.

In HTML there are some semantic elements that can be used to define different parts of a web page.

```html
<article>
<aside>
<details>
<figcaption>
<figure>
<footer>
<header>
<main>
<mark>
<nav>
<section>
<summary>
<time>
```

<img src="./assets/img_sem_elements.gif">

Here are some of the commonly used elements:

The ```<header>``` element represents a container for introductory content or a set of navigational links.

The ```<nav>``` element defines a set of navigation links.

The ```<aside>``` element defines some content aside from the content it is placed in (like a sidebar).

The ```<section>``` element defines a section in a document.

The ```<article>``` element specifies independent, self-contained content.

The ```<footer>``` element defines a footer for a document or section.


### Code along
```html
<!-- semantic.html -->
<!DOCTYPE html>
<html>
    <head>
        <title>Semantic HTML</title>
    </head>
    <body>
        <header>
            <h1>My Portfolio</h1>
        </header>
        <nav>
            <ul>
                <li>Home</li>
                <li>About me</li>
                <li>Gallery</li>
                <li>Contact me</li>
            </ul>
        </nav>
        <section id="home">
            <h2>Home</h2>
            <p>This is the welcome part</p>
        </section>
        <section id="about">
            <h2>About me</h2>
            <p>This is about me part</p>
        </section>
        <section>
            <h2>Gallery</h2>
            <img src="https://picsum.photos/200" alt="random image">
            <img src="https://picsum.photos/200" alt="random image">
            <img src="https://picsum.photos/200" alt="random image">
            <img src="https://picsum.photos/200" alt="random image">
        </section>
        <section id="contact">
            <h2>Contact me</h2>
            <form>
                <label for="name">Name:</label>
                <input type="text" name="name" placeholder="Enter your name"/>
                <br>
                <label for="email">Email:</label>
                <input type="email" name="email" placeholder="Enter your email"/>
                <br>
                <textarea>Leave your message...</textarea>
                <br>
                <button type="submit">Submit</button>
            </form>
        </section>
    </body>
</html>
```
---

