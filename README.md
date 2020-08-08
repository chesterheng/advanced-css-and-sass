# Advanced CSS and Sass: Flexbox, Grid, Animations and More!

## Table of Contents
- [Advanced CSS and Sass: Flexbox, Grid, Animations and More!](#advanced-css-and-sass-flexbox-grid-animations-and-more)
  - [Table of Contents](#table-of-contents)
  - [**Section 1: Welcome, Welcome, Welcome!**](#section-1-welcome-welcome-welcome)
  - [**Section 2: Natours Project — Setup and First Steps (Part 1)**](#section-2-natours-project--setup-and-first-steps-part-1)
    - [4. Section Intro](#4-section-intro)
    - [5. Project Overview](#5-project-overview)
    - [6. Building the Header - Part 1](#6-building-the-header---part-1)
      - [The best way to perform a basic reset using the universal selector](#the-best-way-to-perform-a-basic-reset-using-the-universal-selector)
      - [How to set project-wide font definitions?](#how-to-set-project-wide-font-definitions)
      - [How to clip parts of elements using clip-path?](#how-to-clip-parts-of-elements-using-clip-path)
    - [7. Building the Header - Part 2](#7-building-the-header---part-2)
    - [8. Creating Cool CSS Animations](#8-creating-cool-css-animations)
      - [How to create CSS animations using @keyframes and the animation property?](#how-to-create-css-animations-using-keyframes-and-the-animation-property)
    - [9. Building a Complex Animated Button - Part 1](#9-building-a-complex-animated-button---part-1)
      - [What pseudo-classes are?](#what-pseudo-classes-are)
      - [How to create a creative hover animation effect using the transition property?](#how-to-create-a-creative-hover-animation-effect-using-the-transition-property)
    - [10. Building a Complex Animated Button - Part 2](#10-building-a-complex-animated-button---part-2)
      - [What pseudo-elements are?](#what-pseudo-elements-are)
      - [How and why to use the ::after pseudoelement;](#how-and-why-to-use-the-after-pseudoelement)
  - [**Section 3: How CSS Works: A Look Behind the Scenes**](#section-3-how-css-works-a-look-behind-the-scenes)
    - [12. Three Pillars of Writing Good HTML and CSS (Never Forget Them!)](#12-three-pillars-of-writing-good-html-and-css-never-forget-them)
    - [13. How CSS Works Behind the Scenes: An Overview](#13-how-css-works-behind-the-scenes-an-overview)
    - [14. How CSS is Parsed, Part 1: The Cascade and Specificity](#14-how-css-is-parsed-part-1-the-cascade-and-specificity)
    - [15. Specificity in Practice](#15-specificity-in-practice)
    - [16. How CSS is Parsed, Part 2: Value Processing](#16-how-css-is-parsed-part-2-value-processing)
      - [How CSS values are processed?](#how-css-values-are-processed)
      - [How units are converted from relative to absolute?](#how-units-are-converted-from-relative-to-absolute)
    - [17. How CSS is Parsed, Part 3: Inheritance](#17-how-css-is-parsed-part-3-inheritance)
    - [18. Converting px to rem: An Effective Workflow](#18-converting-px-to-rem-an-effective-workflow)
    - [19. How CSS Renders a Website: The Visual Formatting Model](#19-how-css-renders-a-website-the-visual-formatting-model)
      - [The box model](#the-box-model)
      - [Box types](#box-types)
      - [Positioning Schemes](#positioning-schemes)
      - [Stacking Contexts](#stacking-contexts)
    - [20. CSS Architecture, Components and BEM](#20-css-architecture-components-and-bem)
      - [Thinking about the layout](#thinking-about-the-layout)
      - [Building with meaningful class names](#building-with-meaningful-class-names)
      - [Architecting with files and folders](#architecting-with-files-and-folders)
    - [21. Implementing BEM in the Natours Project](#21-implementing-bem-in-the-natours-project)
  - [**Section 4: Introduction to Sass and NPM**](#section-4-introduction-to-sass-and-npm)
    - [22. Section Intro](#22-section-intro)
    - [23. What is Sass?](#23-what-is-sass)
    - [24. First Steps with Sass: Variables and Nesting](#24-first-steps-with-sass-variables-and-nesting)
    - [25. First Steps with Sass: Mixins, Extends and Functions](#25-first-steps-with-sass-mixins-extends-and-functions)
    - [26. A Brief Introduction to the Command Line](#26-a-brief-introduction-to-the-command-line)
    - [27. NPM Packages: Let's Install Sass Locally](#27-npm-packages-lets-install-sass-locally)
    - [28. NPM Scripts: Let's Write and Compile Sass Locally](#28-npm-scripts-lets-write-and-compile-sass-locally)
    - [29. The Easiest Way of Automatically Reloading a Page on File Changes](#29-the-easiest-way-of-automatically-reloading-a-page-on-file-changes)
  - [**Section 5: Natours Project — Using Advanced CSS and Sass (Part 2)**](#section-5-natours-project--using-advanced-css-and-sass-part-2)
  - [**Section 6: Natours Project — Advanced Responsive Design (Part 3)**](#section-6-natours-project--advanced-responsive-design-part-3)
  - [**Section 7: Trillo Project — Master Flexbox!**](#section-7-trillo-project--master-flexbox)
  - [**Section 8: A Quick Introduction to CSS Grid Layouts**](#section-8-a-quick-introduction-to-css-grid-layouts)
  - [**Section 9: Nexter Project — Master CSS Grid Layouts!**](#section-9-nexter-project--master-css-grid-layouts)
  - [**Section 10: That's It, Everyone!**](#section-10-thats-it-everyone)

## **Section 1: Welcome, Welcome, Welcome!**

- [Course Material and FAQ for my Advanced CSS Course](https://github.com/jonasschmedtmann/advanced-css-course)
- [Jonas' resources page](http://codingheroes.io/resources)
- [Jonas Schmedtmann](https://www.youtube.com/channel/UCNsU-y15AwmU2Q8QTQJG1jw)

**[⬆ back to top](#table-of-contents)**

## **Section 2: Natours Project — Setup and First Steps (Part 1)**

### 4. Section Intro

[Natours](https://natours.netlify.app)
  
**[⬆ back to top](#table-of-contents)**

### 5. Project Overview

[Starter](https://github.com/jonasschmedtmann/advanced-css-course/tree/master/Natours/starter)
  
**[⬆ back to top](#table-of-contents)**

### 6. Building the Header - Part 1

#### The best way to perform a basic reset using the universal selector

```html
<body>
  <header class="header">

  </header>
</body>
```

```css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box; 
}
```

**[⬆ back to top](#table-of-contents)**

#### How to set project-wide font definitions?

```css
body {
  font-family: "Lato", sans-serif;
  font-weight: 400;
  font-size: 16px;
  line-height: 1.7;
  color: #777;
  padding: 30px;
}
```

**[⬆ back to top](#table-of-contents)**

#### How to clip parts of elements using clip-path?

- [CSS clip-path maker](https://bennettfeely.com/clippy/)
```css
.header {
  clip-path: polygon(0 0, 100% 0, 100% 75vh, 0 100%); 
}
```

**[⬆ back to top](#table-of-contents)**

### 7. Building the Header - Part 2

```html
<body>
  <header class="header">
    <div class="logo-box">
      <img src="img/logo-white.png" alt="Logo" class="logo">
    </div>
    <div class="text-box">
      <h1 class="heading-primary">
        <span class="heading-primary-main">Outdoors</span>
        <span class="heading-primary-sub">is where life happens</span>
      </h1>
    </div>
  </header>
</body>
```

```css
.header {
  position: relative;
}

.logo-box {
  position: absolute;
  top: 40px;
  left: 40px;
}

.logo {
  height: 35px;
}

/* The easiest way to center anything with the transform, top and left properties. */
.text-box {
  position: absolute;
  top: 40%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.heading-primary {
  color: #fff;
  text-transform: uppercase;
}

.heading-primary-main {
  display: block;
  font-size: 60px;
  font-weight: 400;
  letter-spacing: 35px;
}

.heading-primary-sub {
  display: block;
  font-size: 20px;
  font-weight: 700;
  letter-spacing: 17.4px;
}
```

**[⬆ back to top](#table-of-contents)**

### 8. Creating Cool CSS Animations

#### How to create CSS animations using @keyframes and the animation property?

```css
.heading-primary {
  backface-visibility: hidden;
}

.heading-primary-main {
  animation-name: moveInLeft;
  animation-duration: 1s;
  animation-timing-function: ease-out;
}

.heading-primary-sub {
  animation: moveInRight 1s ease-out;
}

@keyframes moveInLeft {
  0% {
    opacity: 0;
    transform: translateX(-100px); 
  }
  
  80% {
    transform: translateX(10px); 
  }

  100% {
    opacity: 1;
    transform: translate(0); 
  } 
}

@keyframes moveInRight {
  0% {
    opacity: 0;
    transform: translateX(100px); 
  }
  
  80% {
    transform: translateX(-10px); 
  }

  100% {
    opacity: 1;
    transform: translate(0); 
  } 
}
```

**[⬆ back to top](#table-of-contents)**

### 9. Building a Complex Animated Button - Part 1

#### What pseudo-classes are?

A CSS pseudo-class is a keyword added to a selector that specifies a special state of the selected element(s)

For example, :link, :visited, :hover, :active

**[⬆ back to top](#table-of-contents)**

#### How to create a creative hover animation effect using the transition property?

```html
<a href="" class="btn btn-white">Discover our tours</a>
```

```css
.btn:link,
.btn:visited {
  text-transform: uppercase;
  text-decoration: none;
  padding: 15px 40px;
  display: inline-block;
  border-radius: 100px;
  transition: all .2s;
}

.btn:hover {
  transform: translateY(-3px);
  box-shadow: 0 10px 20px rgba(0, 0, 0, .2);
}

.btn:active {
  transform: translateY(-1px);
  box-shadow: 0 5px 10px rgba(0, 0, 0, .2);
}

.btn-white {
  background-color: #fff;
  color: #777;
}
```

**[⬆ back to top](#table-of-contents)**

### 10. Building a Complex Animated Button - Part 2

#### What pseudo-elements are?

A CSS pseudo-element is a keyword added to a selector that lets you style a specific part of the selected element(s). 

For example, ::after

**[⬆ back to top](#table-of-contents)**

#### How and why to use the ::after pseudoelement; 

In CSS, ::after creates a pseudo-element that is the last child of the selected element. It is often used to add cosmetic content to an element with the content property. It is inline by default.

```css
@keyframes moveInBottom {
  0% {
    opacity: 0;
    transform: translateY(30px); 
  }

  100% {
    opacity: 1;
    transform: translate(0); 
  } 
}

.btn:link,
.btn:visited {
  position: relative;
}

.btn::after {
  content: "";
  display: inline-block;
  height: 100%;
  width: 100%;
  border-radius: 100px;
  position: absolute;
  top: 0;
  left: 0;
  z-index: -1;
  transition: all .4s;
}

.btn-white::after {
  background-color: #fff;
}

.btn:hover::after {
  transform: scaleX(1.4) scaleY(1.6);
  opacity: 0;
}

.btn-animated {
  animation: moveInBottom .5s ease-out .75s;
  animation-fill-mode: backwards;
}
```

**[⬆ back to top](#table-of-contents)**

## **Section 3: How CSS Works: A Look Behind the Scenes**

### 12. Three Pillars of Writing Good HTML and CSS (Never Forget Them!)

| Responsive design             | Maintainable and scalable code | Web performance        |
| ----------------------------- | ------------------------------ | ---------------------- |
| Fluid layouts                 | Clean                          | Less HTTP requests     |
| Media queries                 | Easy-to-understand             | Less code              |
| Responsive images             | Growth                         | Compress code          |
| Correct units                 | Reusable                       | Use a CSS preprocessor |
| Desktop-first vs mobile-first | How to organize files          | Less images            |
|                               | How to name classes            | Compress images        |
|                               | How to structure HTML          |                        |

**[⬆ back to top](#table-of-contents)**

### 13. How CSS Works Behind the Scenes: An Overview

![](section-03/how-css-works.jpg)

**[⬆ back to top](#table-of-contents)**

### 14. How CSS is Parsed, Part 1: The Cascade and Specificity

![](section-03/a-css-rule.jpg)
![](section-03/cascade.jpg)
![](section-03/important.jpg)
![](section-03/specificity.jpg)

Maintainable and scalable code

- CSS declarations marked with !important have the highest priority;
- But, only use !important as a last resource. It’s better to use correct specificities — *more maintainable code!*
- Inline styles will always have priority over styles in external stylesheets;
- A selector that contains **1** ID is more specific than one with *1000* classes;
- A selector that contains **1** class is more specific than one with *1000* elements;
- The universal selector * has no specificity value (0, 0, 0, 0);
- Rely more on **specificity** than on the **order** of selectors;
- But, rely on order when using 3rd-party stylesheets — always put your author stylesheet last.

**[⬆ back to top](#table-of-contents)**

### 15. Specificity in Practice

- [Specificity Calculator](https://specificity.keegan.st)
- [CSS Specificity calculator](https://polypane.app/css-specificity-calculator)

```html
<nav id="nav">
  <div class="pull-right">
    <a class="button button-danger" href="link.html">Don't click here!</a>
  </div>
</nav>
```

```css
body {
  padding: 50px;
}

.button {
  font-size: 20px;
  color: white;
  background-color: blue e
}

a {
  background-color: purple;
}

/* (Inline, IDs, Classes, Elements) */
/* (0, 1, 2, 2) */
#nav div.pull-right a.button {
  background-color: orangered;
}

/* (0, 1, 3, 2) */
#nav div.pull-right a.button:hover {
  background-color: green;
}

/* (0, 1, 2, 1) */
#nav a.button:hover {
  background-color: yellow;
}
```

**[⬆ back to top](#table-of-contents)**

### 16. How CSS is Parsed, Part 2: Value Processing

#### How CSS values are processed?

![](section-03/css-values.jpg)

**[⬆ back to top](#table-of-contents)**

#### How units are converted from relative to absolute?

![](section-03/units.jpg)

**[⬆ back to top](#table-of-contents)**

- Each property has an initial value, used if nothing is declared (and if there is no inheritance — see next lecture); 
- Browsers specify a **root font-size** for each page (usually 16px);
- Percentages and relative values are always converted to pixels;
- Percentages are measured relative to their parent’s **font-size**, if used to specify font-size;
- Percentages are measured relative to their parent’s **width**, if used to specify lengths; 
- em are measured relative to their **parent** font-size, if used to specify font-size; 
- em are measured relative to the **current** font-size, if used to specify lengths;
- rem are always measured relative to the **document’s root** font-size;
- vh and vw are simply percentage measurements of the viewport’s height and width.

**[⬆ back to top](#table-of-contents)**

### 17. How CSS is Parsed, Part 3: Inheritance

Inheritance in CSS

![](section-03/inheritance.jpg)

- Inheritance passes the values for some specific properties from parents to children — **more maintainable code**;
- Properties related to text are inherited: font-family, font-size, color, etc; 
- The computed value of a property is what gets inherited, **not** the declared value. 
- Inheritance of a property only works if no one declares a value for that property; 
- The inherit keyword forces inheritance on a certain property;
- The initial keyword resets a property to its initial value.

**[⬆ back to top](#table-of-contents)**

### 18. Converting px to rem: An Effective Workflow

```css
html {
  font-size: 62.5%;
}

body {
  font-family: "Lato", sans-serif;
  font-weight: 400;
  /* font-size: 16px; */
  line-height: 1.7;
  color: #777;
  padding: 3rem;
}
```

- The inherit keyword specifies that a property should inherit its value from its parent element.
- The * selector selects all elements.
- All element will have the property `box-sizing: inherit;`
- All Child elements will inherit the property `box-sizing: border-box;` from parent element `body` 

```css
*,
*::after,
*::before {
  margin: 0;
  padding: 0;
  box-sizing: inherit; 
}

body {
  box-sizing: border-box; 
}
```

**[⬆ back to top](#table-of-contents)**

### 19. How CSS Renders a Website: The Visual Formatting Model

The Visual Formatting Model

![](section-03/website-rendering.jpg)

Algorithm that calculates boxes and determines the layout of theses boxes, for each element in the render tree, in order to determine the final layout of the page.

- **Dimensions of boxes**: the box model;
- **Box type**: inline, block and inline-block; 
- **Positioning scheme**: floats and positioning; 
- **Stacking contexts**;
- Other elements in the render tree;
- Viewport size, dimensions of images, etc.

**[⬆ back to top](#table-of-contents)**

#### The box model

![](section-03/box-model.jpg)

- **Content**: text, images, etc;
- **Padding**: transparent area around the content, inside of the box;
- **Border**: goes around the padding and the content;
- **Margin**: space between boxes;
- Fill area: area that gets filled with background color or background image.

The box model - Heights and Widths (default)

- total width = right border + right padding + specified width + left padding + left border
- total height = top border + top padding + specified height + bottom padding + bottom border 
- Example: height = 0 + 20px + 100px + 20px + 0 = 140px

The box model - Heights and Widths (box-sizing: border-box)

![](section-03/border-box.jpg)

**[⬆ back to top](#table-of-contents)**

#### Box types

| Block-level boxes                     | Inline-block boxes            | Inline boxes                                          |
| ------------------------------------- | ----------------------------- | ----------------------------------------------------- |
| Elements formatted visually as blocks | A mix of block and inline     | Content is distributed in lines                       |
| 100% of parent’s width                | Occupies only content’s space | Occupies only content’s space                         |
| Vertically, one after another         | No line-breaks                | No line-breaks                                        |
| Box-model applies as showed           | Box-model applies as showed   | No heights and widths                                 |
|                                       |                               | Paddings and margins only horizontal (left and right) |
| display: block                        | display: inline-block         | display: inline                                       |
| display: flex                         |                               |                                                       |
| display: list-item                    |                               |                                                       |
| display: table                        |                               |                                                       |

**[⬆ back to top](#table-of-contents)**

#### Positioning Schemes

| Normal flow                                        | Floats                                                         | Absolute positioning                                                                               |
| -------------------------------------------------- | -------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| Default positioning scheme;                        | Element is removed from the normal flow;                       | Element is removed from the normal flow                                                            |
| NOT floated;                                       | Text and inline elements will wrap around the floated element; | No impact on surrounding content or elements;                                                      |
| NOT absolutely positioned;                         | The container will not adjust its height to the element.       | We use top, bottom, left and right to offset the element from its relatively positioned container. |
| Elements laid out according to their source order. |                                                                |                                                                                                    |
| default                                            | float: left                                                    | position: absolute                                                                                 |
| position: relative                                 | float: right                                                   | position: fixed                                                                                    |

**[⬆ back to top](#table-of-contents)**

#### Stacking Contexts

![](section-03/stacking-contexts.jpg)

**[⬆ back to top](#table-of-contents)**

### 20. CSS Architecture, Components and BEM

The Think - Build - Architect Mindset

| Responsive design | Maintainable and scalable code | Web performance |
| ----------------- | ------------------------------ | --------------- |
|                   | Clean                          |                 |
|                   | Modular                        |                 |
|                   | Reusable                       |                 |
|                   | Ready for growth               |                 |

Think -> Build -> Architect

- **Think** about the layout of your webpage or web app before writing code.
- **Build** your layout in HTML and CSS with a consistent structure for naming classes.
- Create a logical **architecture** for your CSS with files and folders.

**[⬆ back to top](#table-of-contents)**

#### Thinking about the layout

![](section-03/atomic-design.jpg)

Component-driven design

- **Modular building blocks** that make up interfaces;
- Held together by the **layout** of the page;
- **Re-usable** across a project, and between different projects; 
- **Independent**, allowing us to use them anywhere on the page.

**[⬆ back to top](#table-of-contents)**

#### Building with meaningful class names

![](section-03/bem.jpg)

**[⬆ back to top](#table-of-contents)**

#### Architecting with files and folders

The 7-1 pattern

- 7 different folders for partial Sass files, and 1 main Sass file to import all other files into a compiled CSS stylesheet.

The 7 Folders

- base/ 
- components/ 
- layout/ 
- pages/ 
- themes/ 
- abstracts/ 
- vendors/

**[⬆ back to top](#table-of-contents)**

### 21. Implementing BEM in the Natours Project

```html
<header class="header">
  <div class="header__logo-box">
    <img src="img/logo-white.png" alt="Logo" class="header__logo">
  </div>
  <div class="header__text-box">
    <h1 class="heading-primary">
      <span class="heading-primary--main">Outdoors</span>
      <span class="heading-primary--sub">is where life happens</span>
    </h1>

    <a href="" class="btn btn--white btn--animated">Discover our tours</a>
  </div>
</header>
```

```css
.header {
  height: 95vh;
  background-image: linear-gradient(to right bottom, rgba(126, 213, 111, 0.8), rgba(40, 180, 133, 0.8)), url(../img/hero.jpg);
  background-size: cover;
  background-position: top;
  position: relative;

  clip-path: polygon(0 0, 100% 0, 100% 75vh, 0 100%); 
}

.header__logo-box {
  position: absolute;
  top: 4rem;
  left: 4rem;
}

.header__logo {
  height: 3.5rem;
}

.header__text-box {
  position: absolute;
  top: 40%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
}

.heading-primary {
  color: #fff;
  text-transform: uppercase;

  backface-visibility: hidden;
  margin-bottom: 6rem;
}

.heading-primary--main {
  display: block;
  font-size: 6rem;
  font-weight: 400;
  letter-spacing: 3.5rem;

  animation-name: moveInLeft;
  animation-duration: 1s;
  animation-timing-function: ease-out;
  /* animation-delay: 3s; */
}

.heading-primary--sub {
  display: block;
  font-size: 2rem;
  font-weight: 700;
  letter-spacing: 1.75rem;

  animation: moveInRight 1s ease-out;
}

.btn:link,
.btn:visited {
  text-transform: uppercase;
  text-decoration: none;
  padding: 1.5rem 4rem;
  display: inline-block;
  border-radius: 10rem;
  transition: all .2s;
  position: relative;
  font-size: 1.6rem;
}

.btn:hover {
  transform: translateY(-.3rem);
  box-shadow: 0 1rem 2rem rgba(0, 0, 0, .2);
}

.btn:active {
  transform: translateY(-.1rem);
  box-shadow: 0 .5rem 1rem rgba(0, 0, 0, .2);
}

.btn--white {
  background-color: #fff;
  color: #777;
}

.btn--white::after {
  background-color: #fff;
}

.btn--animated {
  animation: moveInBottom .5s ease-out .75s;
  animation-fill-mode: backwards;
}
```

**[⬆ back to top](#table-of-contents)**

## **Section 4: Introduction to Sass and NPM**

### 22. Section Intro
**[⬆ back to top](#table-of-contents)**

### 23. What is Sass?

Sass is a CSS preprocessor, an extension of CSS that adds power and elegance to the basic language.

![](section-04/sass.jpg)

Main SASS features

- **Variables**: for reusable values such as colors, font-sizes, spacing, etc;
- **Nesting**: to nest selectors inside of one another, allowing us to write less code;
- **Operators**: for mathematical operations right inside of CSS;
- **Partials and imports**: to write CSS in different files and importing them all into one single file;
- **Mixins**: to write reusable pieces of CSS code;
- **Functions**: similar to mixins, with the difference that they produce a value that can than be used; 
- **Extends**: to make different selectors inherit declarations that are common to all of them;
- **Control directives**: for writing complex code using conditionals and loops (not covered in this course).

![](section-04/sass-syntax.jpg)

**[⬆ back to top](#table-of-contents)**

### 24. First Steps with Sass: Variables and Nesting

```html
<nav>
  <ul class="navigation">
    <li><a href="#">About us</a></li>
    <li><a href="#">Pricing</a></li>
    <li><a href="#">Contact</a></li>
  </ul>
  <div class="buttons">
    <a class="btn-main" href="#">Sign up</a>
    <a class="btn-hot" href="#">Get a quote</a>
  </div>
</nav>
```

```scss
* {
  margin: 0;
  padding: 0;
}

// SaSS variables
$color-primary: #f9ed69; //yellow color
$color-secondary: #f08a5d; //orange color
$color-tertiary: #b83b5e; //pink color
$color-text-dark: #333; //dark grey
$color-text-light: #eee; //light grey

$width-button: 150px;

nav {
  margin: 30px;
  background-color: $color-primary;

  // Fix for displaying no background when using floats
  &:after {
    content: "";
    clear: both;
    display: table;
  }
}

.navigation {
  list-style: none;
  float: left;

  // Nested selector
  li {
    display: inline-block;
    margin-left: 30px;

    // No limit on how many nested selectors you have
    // &: === .nagivation li
    &:first-child {
      margin: 0;
    }
    
    a:link, 
    a:active {
      text-decoration: none;
      text-transform: uppercase;
      color: $color-text-dark;
    }
  }
}

.buttons {
  float: right;
}

.btn-main:link,
.btn-hot:link {
  padding: 10px;
  display: inline-block;
  text-align: center;
  border-radius: 100px;
  text-decoration: none;
  text-transform: uppercase;
  width: $width-button;
  color: $color-text-light;
}

.btn-main {
  &:link {
    background-color: $color-secondary;
  }

  &:hover {
    background-color: darken($color-secondary, 15%);
  }
}

.btn-hot {
  &:link {
    background-color: $color-tertiary;
  }

  &:hover {
    background-color: lighten($color-tertiary, 15%);
  }
}
```

**[⬆ back to top](#table-of-contents)**

### 25. First Steps with Sass: Mixins, Extends and Functions

- Mixins allow you to define styles that can be re-used throughout your stylesheet.
- Extends allows you to share styles between two selectors.
- Functions allow you to define complex operations on SassScript values that you can re-use throughout your stylesheet.

```scss
$color-text-dark: #333; //dark grey
$color-text-light: #eee; //light grey

@mixin clearfix {
   &::after{
    content:"";
    clear:both;
    display:table;
  }
}

@mixin style-link-text($color) {
  text-decoration: none;
  text-transform: uppercase;
  color: $color;
}

@function divide($a, $b) {
  @return $a / $b;
}

nav {
  margin: divide(60, 2) * 1px; // 30px
  background-color: $color-primary;

  @include clearfix
}

.navigation {
  list-style: none;
  float: left;

  li {
    a:link, 
    a:active {
      @include style-link-text($color-text-dark)
    }
  }
}

// both .btn-main:link, .btn-hot:link will share styles
%btn-placeholder {
  padding: 10px;
  display: inline-block;
  text-align: center;
  border-radius: 100px;
  width: $width-button;
  @include style-link-text($color-text-light)
}

.btn-main {
  &:link {
    @extend %btn-placeholder;
    background-color: $color-secondary;
  }
}

.btn-hot {
  &:link {
    @extend %btn-placeholder;
    background-color: $color-tertiary;
  }
}
```

**[⬆ back to top](#table-of-contents)**

### 26. A Brief Introduction to the Command Line
**[⬆ back to top](#table-of-contents)**

### 27. NPM Packages: Let's Install Sass Locally
**[⬆ back to top](#table-of-contents)**

### 28. NPM Scripts: Let's Write and Compile Sass Locally
**[⬆ back to top](#table-of-contents)**

### 29. The Easiest Way of Automatically Reloading a Page on File Changes
**[⬆ back to top](#table-of-contents)**

## **Section 5: Natours Project — Using Advanced CSS and Sass (Part 2)**
**[⬆ back to top](#table-of-contents)**

## **Section 6: Natours Project — Advanced Responsive Design (Part 3)**
**[⬆ back to top](#table-of-contents)**

## **Section 7: Trillo Project — Master Flexbox!**
**[⬆ back to top](#table-of-contents)**

## **Section 8: A Quick Introduction to CSS Grid Layouts**
**[⬆ back to top](#table-of-contents)**

## **Section 9: Nexter Project — Master CSS Grid Layouts!**
**[⬆ back to top](#table-of-contents)**

## **Section 10: That's It, Everyone!**
**[⬆ back to top](#table-of-contents)**