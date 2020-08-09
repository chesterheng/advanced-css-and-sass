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
    - [27. NPM Packages: Let's Install Sass Locally](#27-npm-packages-lets-install-sass-locally)
    - [28. NPM Scripts: Let's Write and Compile Sass Locally](#28-npm-scripts-lets-write-and-compile-sass-locally)
    - [29. The Easiest Way of Automatically Reloading a Page on File Changes](#29-the-easiest-way-of-automatically-reloading-a-page-on-file-changes)
  - [**Section 5: Natours Project — Using Advanced CSS and Sass (Part 2)**](#section-5-natours-project--using-advanced-css-and-sass-part-2)
    - [31. Converting Our CSS Code to Sass: Variables and Nesting](#31-converting-our-css-code-to-sass-variables-and-nesting)
    - [32. Implementing the 7-1 CSS Architecture with Sass](#32-implementing-the-7-1-css-architecture-with-sass)
    - [33. Review: Basic Principles of Responsive Design and Layout Types](#33-review-basic-principles-of-responsive-design-and-layout-types)
    - [34. Building a Custom Grid with Floats](#34-building-a-custom-grid-with-floats)
    - [35. Building the About Section - Part 1](#35-building-the-about-section---part-1)
      - [Thinking about components](#thinking-about-components)
      - [How and why to use utility classes?](#how-and-why-to-use-utility-classes)
      - [How to use the background-clip property?](#how-to-use-the-background-clip-property)
      - [How to transform multiple properties simultaneously?](#how-to-transform-multiple-properties-simultaneously)
    - [36. Building the About Section - Part 2](#36-building-the-about-section---part-2)
      - [Tertiary Heading component](#tertiary-heading-component)
      - [Paragraph component](#paragraph-component)
      - [Text Button component](#text-button-component)
    - [37. Building the About Section - Part 3](#37-building-the-about-section---part-3)
      - [How to use the outline-offset property together with outline?](#how-to-use-the-outline-offset-property-together-with-outline)
      - [How to style elements that are NOT hovered while others are?](#how-to-style-elements-that-are-not-hovered-while-others-are)
    - [38. Building the Features Section](#38-building-the-features-section)
      - [How to include and use an icon font?](#how-to-include-and-use-an-icon-font)
      - [Another way of creating the "skewed section"](#another-way-of-creating-the-skewed-section)
      - [How and when to use the direct child selector?](#how-and-when-to-use-the-direct-child-selector)
    - [39. Building the Tours Section - Part 1](#39-building-the-tours-section---part-1)
      - [Thinking about components](#thinking-about-components-1)
      - [How to build an amazing, rotating card?](#how-to-build-an-amazing-rotating-card)
    - [40. Building the Tours Section - Part 2](#40-building-the-tours-section---part-2)
      - [Front Side Card component: Picture, Heading, Details](#front-side-card-component-picture-heading-details)
      - [How to use perspective in CSS?](#how-to-use-perspective-in-css)
      - [How to use the backface-visibility property?](#how-to-use-the-backface-visibility-property)
      - [Using background blend modes?](#using-background-blend-modes)
      - [How and when to use box-decoration-break;](#how-and-when-to-use-box-decoration-break)
    - [41. Building the Tours Section - Part 3](#41-building-the-tours-section---part-3)
      - [Back Side Card component: CTA](#back-side-card-component-cta)
      - [Green Button](#green-button)
    - [42. Building the Stories Section - Part 1](#42-building-the-stories-section---part-1)
      - [Thinking about components](#thinking-about-components-2)
      - [Story component](#story-component)
      - [How to make text flow around shapes with shape-outside and float?](#how-to-make-text-flow-around-shapes-with-shape-outside-and-float)
    - [43. Building the Stories Section - Part 2](#43-building-the-stories-section---part-2)
      - [Story Shape component - Figure Caption](#story-shape-component---figure-caption)
    - [44. Building the Stories Section - Part 3](#44-building-the-stories-section---part-3)
      - [Story component - Background video](#story-component---background-video)
      - [How to use the <video> HTML element?](#how-to-use-the-video-html-element)
      - [How to create a background video covering an entire section?](#how-to-create-a-background-video-covering-an-entire-section)
      - [How and when to use the object-fit property?](#how-and-when-to-use-the-object-fit-property)
    - [45. Building the Booking Section - Part 1](#45-building-the-booking-section---part-1)
      - [Thinking about components](#thinking-about-components-3)
      - [How to implement "solid-color gradients"?](#how-to-implement-solid-color-gradients)
    - [46. Building the Booking Section - Part 2](#46-building-the-booking-section---part-2)
      - [Input component: Full name and Email address](#input-component-full-name-and-email-address)
      - [How the general and adjacent sibling selectors work and why we need them?](#how-the-general-and-adjacent-sibling-selectors-work-and-why-we-need-them)
      - [How to use the ::input-placeholder pseudo-element?](#how-to-use-the-input-placeholder-pseudo-element)
      - [How and when to use the :focus, :invalid, :placeholder-shown?](#how-and-when-to-use-the-focus-invalid-placeholder-shown)
    - [47. Building the Booking Section - Part 3](#47-building-the-booking-section---part-3)
      - [Techniques to build custom radio buttons](#techniques-to-build-custom-radio-buttons)
      - [Green button](#green-button-1)
      - [How and when to use the :checked pseudo-classes?](#how-and-when-to-use-the-checked-pseudo-classes)
    - [48. Building the Footer](#48-building-the-footer)
      - [How to design a simple website footer?](#how-to-design-a-simple-website-footer)
    - [49. Building the Navigation - Part 1](#49-building-the-navigation---part-1)
    - [50. Building the Navigation - Part 2](#50-building-the-navigation---part-2)
    - [51. Building the Navigation - Part 3](#51-building-the-navigation---part-3)
    - [52. Building a Pure CSS Popup - Part 1](#52-building-a-pure-css-popup---part-1)
    - [53. Building a Pure CSS Popup - Part 2](#53-building-a-pure-css-popup---part-2)
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

### 27. NPM Packages: Let's Install Sass Locally

[node-sass](https://github.com/sass/node-sass)

**[⬆ back to top](#table-of-contents)**

### 28. NPM Scripts: Let's Write and Compile Sass Locally

```console
npm run compile:sass
```

**[⬆ back to top](#table-of-contents)**

### 29. The Easiest Way of Automatically Reloading a Page on File Changes

[Live Server](https://github.com/tapio/live-server)

```console
npm i live-server -g
live-server
```

**[⬆ back to top](#table-of-contents)**

## **Section 5: Natours Project — Using Advanced CSS and Sass (Part 2)**

### 31. Converting Our CSS Code to Sass: Variables and Nesting

```scss
$color-primary: #55c57a;
$color-primary-light: #7ed56f;
$color-primary-dark: #28b485;

$color-grey-dark: #777;
$color-white: #fff;
$color-black: #000;

.header {
  height: 95vh;
  background-image: linear-gradient(to right bottom, rgba($color-primary-light, 0.8), rgba($color-primary-dark, 0.8)), url(../img/hero.jpg);
  background-size: cover;
  background-position: top;
  position: relative;

  clip-path: polygon(0 0, 100% 0, 100% 75vh, 0 100%);

  &__logo-box {
    position: absolute;
    top: 4rem;
    left: 4rem;
  }

  &__logo {
    height: 3.5rem;
  }
  
  &__text-box {
    position: absolute;
    top: 40%;
    left: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
  }
}
```

**[⬆ back to top](#table-of-contents)**

### 32. Implementing the 7-1 CSS Architecture with Sass

![](section-05/sass-architecture.jpg)

**[⬆ back to top](#table-of-contents)**

### 33. Review: Basic Principles of Responsive Design and Layout Types

Basic Responsive Design Principles

- Fluid Grids And Layouts

To allow content to easily adapt to the current viewport width used to browse the website. Uses % rather than px for all layout-related lengths.

- Flexible/Responsive Images

Images behave differently than text content, and so we need to ensure that they also adapt nicely to the current viewport.

- Media Queries

To change styles on certain viewport widths (breakpoints), allowing us to create different version of our website for different widths.

![](section-05/layout-types.jpg)

**[⬆ back to top](#table-of-contents)**

### 34. Building a Custom Grid with Floats

- How to architect and build a simple grid system; 
- How the attribute selector works;
- How the :not pseudo-class works;
- How calc() works, and what’s the difference between calc() and simple Sass operations.

![](section-05/css-grid.jpg)

```html
    <section class="grid-test">
      <div class="row">
        <div class="col-1-of-2">Col 1 of 2</div>
        <div class="col-1-of-2">Col 1 of 2</div>
      </div>
      <div class="row">
        <div class="col-1-of-3">Col 1 of 3</div>
        <div class="col-1-of-3">Col 1 of 3</div>
        <div class="col-1-of-3">Col 1 of 3</div>
      </div>
      <div class="row">
        <div class="col-1-of-3">Col 1 of 3</div>
        <div class="col-2-of-3">Col 2 of 3</div>
      </div>
      <div class="row">
        <div class="col-1-of-4">Col 1 of 4</div>
        <div class="col-1-of-4">Col 1 of 4</div>
        <div class="col-1-of-4">Col 1 of 4</div>
        <div class="col-1-of-4">Col 1 of 4</div>
      </div>
      <div class="row">
        <div class="col-1-of-4">Col 1 of 4</div>
        <div class="col-1-of-4">Col 1 of 4</div>
        <div class="col-2-of-4">Col 2 of 4</div>
      </div>
      <div class="row">
        <div class="col-1-of-4">Col 1 of 4</div>
        <div class="col-3-of-4">Col 3 of 4</div>
      </div>
    </section>
```

```scss
.row {
  max-width: $grid-width;
  background-color: #eee;
  // center block element
  margin: 0 auto;

  // select everything except last child
  &:not(:last-child) {
    margin-bottom: $gutter-vertical;
  }

  @include clearfix;

  // select all class selector start with "col-"
  [class^="col-"] {
    background-color: orangered;
    float: left;

    &:not(:last-child) {
      margin-right: $gutter-horizontal;
    }
  }

  .col-1-of-2 {
    width: calc((100% - #{$gutter-horizontal}) / 2);
  }

  .col-1-of-3 {
    width: calc((100% - 2 * #{$gutter-horizontal}) / 3);
  }

  .col-2-of-3 {
    width: calc(2 * ((100% - 2 * #{$gutter-horizontal}) / 3) + #{$gutter-horizontal});
  }

  .col-1-of-4 {
    width: calc((100% - 3 * #{$gutter-horizontal}) / 4);
  }

  .col-2-of-4 {
    width: calc(2 * ((100% - 3 * #{$gutter-horizontal}) / 4) + #{$gutter-horizontal});
  }

  .col-3-of-4 {
    width: calc(3 * ((100% - 3 * #{$gutter-horizontal}) / 4) + 2 * #{$gutter-horizontal});
  }
}
```

**[⬆ back to top](#table-of-contents)**

### 35. Building the About Section - Part 1

#### Thinking about components

![](section-05/about-section.jpg)

- Secondary Heading
- Tertiary Heading
- Paragraph
- Text Button
- Image Composition

```html
      <section class="section-about">
        <div class="u-center-text u-margin-bottom-big">
          <h2 class="heading-secondary">
            Exciting tours for adventurous people
          </h2>
        </div>
        <div class="row">
          <div class="col-1-of-2"></div>
          <div class="col-1-of-2"></div>
        </div>
      </section>
```

```css
.section-about {
  background-color: $color-grey-light-1;
  padding: 25rem 0;
  margin-top: -20vh;
}
```

**[⬆ back to top](#table-of-contents)**

Secondary Heading component

```html
<div class="u-center-text u-margin-bottom-big">
  <h2 class="heading-secondary">
    Exciting tours for adventurous people
  </h2>
</div>
```

```scss
.heading-secondary {
  font-size: 3.5rem;
  text-transform: uppercase;
  font-weight: 700;
  display: inline-block;
  background-image: linear-gradient(to right, $color-primary-light, $color-primary-dark);
  background-clip: text;
  -webkit-background-clip: text;
  color: transparent;
  letter-spacing: .2rem;
  transition: all .2s;

  &:hover {
    transform: skewY(2deg) skewX(15deg) scale(1.1);
    text-shadow: .5rem 1rem 2rem rgba($color-black, .2);
  }
}
```

**[⬆ back to top](#table-of-contents)**

#### How and why to use utility classes?

```scss
.u-center-text {
  // center inline-block child
  text-align: center;
}

.u-margin-bottom-small { margin-bottom: 2rem; }
.u-margin-bottom-medium { margin-bottom: 4rem; }
.u-margin-bottom-big { margin-bottom: 8rem; }
```

**[⬆ back to top](#table-of-contents)**

#### How to use the background-clip property?

```scss
.heading-secondary {
  display: inline-block;
  background-image: linear-gradient(to right, $color-primary-light, $color-primary-dark);
  -webkit-background-clip: text;
  color: transparent;
}
```

**[⬆ back to top](#table-of-contents)**

#### How to transform multiple properties simultaneously?

```scss
.heading-secondary {
  transition: all .2s;

  &:hover {
    transform: skewY(2deg) skewX(15deg) scale(1.1);
    text-shadow: .5rem 1rem 2rem rgba($color-black, .2);
  }
}
```

**[⬆ back to top](#table-of-contents)**

### 36. Building the About Section - Part 2

```html
<h3 class="heading-tertiary u-margin-bottom-small">You are going to fall in love with nature</h3>
<p class="paragraph">
  Lorem ipsum dolor sit, amet consectetur adipisicing elit. Iste rerum ullam accusantium omnis officia, repellendus qui quae, maxime itaque dolores corporis provident. Illo temporibus magnam praesentium, maiores ipsa beatae dolor?
</p>
<h3 class="heading-tertiary u-margin-bottom-small">Live adventures like you never have before</h3>
<p class="paragraph">
  Lorem ipsum dolor sit amet, consectetur adipisicing elit. Recusandae quos, reiciendis perspiciatis rem quis velit quae deleniti itaque? Modi harum voluptates minus? Molestiae, id libero impedit consequatur quae amet inventore?
</p>

<a href="#" class="btn-text">
  Learn more &rarr;
</a>
```

**[⬆ back to top](#table-of-contents)**

#### Tertiary Heading component

```scss
.heading-tertiary {
  font-size: $default-font-size;
  font-weight: 700;
  text-transform: uppercase;
}
```

**[⬆ back to top](#table-of-contents)**

#### Paragraph component

```scss
.paragraph {
  font-size: $default-font-size;

  &:not(:last-child) {
    margin-bottom: 3rem;
  }
}
```

**[⬆ back to top](#table-of-contents)**

#### Text Button component

```scss
.btn-text {
  &:link,
  &:visited {
    font-size: $default-font-size;
    color: $color-primary;
    display: inline-block;
    text-decoration: none;
    border-bottom: 1px solid $color-primary;
    padding: 3px;
    transition: all .2s;
  }

  &:hover {
    background-color: $color-primary;
    color: $color-white;
    box-shadow: 0 1rem 2rem rgba($color-black, .15);
    transform: translateY(-2px);
  }

  &:active {
    box-shadow: 0 .5rem 1rem rgba($color-black, .15);
    transform: translateY(0);
  }
}
```

**[⬆ back to top](#table-of-contents)**

### 37. Building the About Section - Part 3

Image Composition component

```html
<div class="composition">
  <img src="img/nat-1-large.jpg" alt="Photo 1" class="composition__photo composition__photo--p1">
  <img src="img/nat-2-large.jpg" alt="Photo 2" class="composition__photo composition__photo--p2">
  <img src="img/nat-3-large.jpg" alt="Photo 3" class="composition__photo composition__photo--p3">
</div>
```

```scss
.composition {
  position: relative;

  &__photo {
    width: 55%;
    box-shadow: 0 1.5rem 4rem rgba($color-black, 0.4);
    border-radius: 2px;
    position: absolute;
    z-index: 10;
    transition: all .2s;
    outline-offset: 2rem;

    &--p1 {
      left: 0;
      top: -2rem;
    }

    &--p2 {
      right: 0;
      top: 2rem;
    }

    &--p3 {
      left: 20%;
      top: 10rem;
    }

    &:hover {
      outline: 1.5rem solid $color-primary;
      transform: scale(1.05) translateY(-.5rem);
      box-shadow: 0 2.5rem 4rem rgba($color-black, .5);
      z-index: 20;
    }
  }

  // composition:hover composition__photo:not(:hover)
  &:hover &__photo:not(:hover) {
    transform: scale(0.95);
  }
}
```

**[⬆ back to top](#table-of-contents)**

#### How to use the outline-offset property together with outline?

```scss
.composition {
  position: relative;

  &__photo {
    outline-offset: 2rem;

    &:hover {
      outline: 1.5rem solid $color-primary;
    }
  }
}
```

**[⬆ back to top](#table-of-contents)**

#### How to style elements that are NOT hovered while others are?

```scss
.composition {
  position: relative;

  &__photo {
    &:hover {
      outline: 1.5rem solid $color-primary;
      transform: scale(1.05) translateY(-.5rem);
      box-shadow: 0 2.5rem 4rem rgba($color-black, .5);
      z-index: 20;
    }
  }

  // composition:hover composition__photo:not(:hover)
  &:hover &__photo:not(:hover) {
    transform: scale(0.95);
  }
}
```

**[⬆ back to top](#table-of-contents)**

### 38. Building the Features Section

![](section-05/features-section.jpg)

```html
<section class="section-features">
  <div class="row">
    <div class="col-1-of-4">
      <div class="feature-box">
        <i class="feature-box__icon icon-basic-world"></i>
        <h3 class="heading-tertiary u-margin-bottom-small">Explore the world</h3>
        <p class="feature-box__text">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Recusandae rerum commodi atque, natus inventore.
        </p>
      </div>
    </div>
    <div class="col-1-of-4">
      <div class="feature-box">
        <i class="feature-box__icon icon-basic-compass"></i>
        <h3 class="heading-tertiary u-margin-bottom-small">Meet nature</h3>
        <p class="feature-box__text">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Recusandae rerum commodi atque, natus inventore.
        </p>
      </div>
    </div>
    <div class="col-1-of-4">
      <div class="feature-box">
        <i class="feature-box__icon icon-basic-map"></i>
        <h3 class="heading-tertiary u-margin-bottom-small">Find your way</h3>
        <p class="feature-box__text">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Recusandae rerum commodi atque, natus inventore.
        </p>
      </div>
    </div>
    <div class="col-1-of-4">
      <div class="feature-box">
        <i class="feature-box__icon icon-basic-heart"></i>
        <h3 class="heading-tertiary u-margin-bottom-small">Live a healther life</h3>
        <p class="feature-box__text">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Recusandae rerum commodi atque, natus inventore.
        </p>
      </div>
    </div>
  </div>
</section>
```

```scss
.section-features {
  padding: 20rem 0;
  background-image: linear-gradient(to right bottom, rgba($color-primary-light, 0.8), rgba($color-primary-dark, 0.8)), url(../img/nat-4.jpg);
  background-size: cover;

  transform: skewY(-7deg);
  margin-top: -10rem;

  // select all direct child: row selector in this case
  & > * {
    transform: skewY(7deg);
  }
}
```

```scss
.feature-box {
  background-color: rgba($color-white, .8);
  font-size: 1.5rem;
  padding: 2.5rem;
  text-align: center;
  border-radius: 3px;
  box-shadow: 0 1.5rem 4rem rgba($color-black, .15);
  transition: transform .3s;

  &__icon {
    font-size: 6rem;
    margin-bottom: .5rem;
    display: inline-block;
    background-image: linear-gradient(to right, $color-primary-light, $color-primary-dark);
    -webkit-background-clip: text;
    color: transparent;
  }

  &:hover {
    transform: translateY(-1.5rem) scale(1.03);
  }

  &__text {

  }
}
```

**[⬆ back to top](#table-of-contents)**

#### How to include and use an icon font?

![](section-05/css.jpg)

- Goto [Linea Icon](https://linea.io/)
- Download linea_complete_1.0.zip
- Unzip linea_complete_1.0.zip
- Goto _basic/_ICONFONT/ folder
- Rename styles.css to icon-font.css
- Copy fonts folder to css project folder
- Copy icon-font.css file to css project folder
- Include icon-font.css in index.html
- Refer to linea_complete_1.0/_basic/_ICONFONT/icons-reference.html for icon name

**[⬆ back to top](#table-of-contents)**

#### Another way of creating the "skewed section"

```scss
.section-features {
  transform: skewY(-7deg);
  margin-top: -10rem;
}
```

**[⬆ back to top](#table-of-contents)**

#### How and when to use the direct child selector?

```html
<section class="section-features">
  <div class="row">
  </div>
</section>
```

```scss
.section-features {
  // select all direct child of section-features
  // Example: row selector
  & > * {
    transform: skewY(7deg);
  }
}
```

**[⬆ back to top](#table-of-contents)**

### 39. Building the Tours Section - Part 1

#### Thinking about components

- Secondary Heading
- 3 Cards
  - Front: Picture, Heading, Details
  - Back: CTA
- Green Button

![](section-05/section-tours-front.jpg)
![](section-05/section-tours-back.jpg)

```html
<section class="section-tours">
  <div class="u-center-text u-margin-bottom-big">
    <h2 class="heading-secondary">
      Most popular tours
    </h2>
  </div>
  <div class="row">
    <div class="col-1-of-3">
      <div class="card">
        <div class="card__side card__side--front">
          <div class="card__picture card__picture--1">&nbsp</div>
          <h4 class="card__heading">
            <span class="card__heading-span card__heading-span--1">
              The Sea Explorer
            </span>
          </h4>
          <div class="card__details">
            <ul>
              <li>3 day tours</li>
              <li>Up to 30 people</li>
              <li>2 tour guides</li>
              <li>Sleep in cozy hotel</li>
              <li>Difficulty: easy</li>
            </ul>
          </div>
        </div>
        <div class="card__side card__side--back card__side--back--1">
          <div class="card__cta">
            <div class="card__price-box">
              <p class="card__price-only">Only</p>
              <p class="card__price-value">$297</p>
            </div>
            <a href="" class="btn btn--white">Book now</a>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="u-center-text u-margin-top-huge">
    <a href="#" class="btn btn--green">Discover all tours</a>
  </div>
</section>
```

```scss
.section-tours {
  background-color: $color-grey-light-1;
  padding: 25rem 0 15rem 0;
  margin-top: -10rem;
}

.card {
  // FUNCTIONALITY
  perspective: 150rem;
  -moz-perspective: 150rem;
  position: relative;
  height: 52rem;

  &__side {
    height: 52rem;
    transition: all .8s ease;
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    backface-visibility: hidden;
    border-radius: 3px;
    overflow: hidden;
    box-shadow: 0 1.5rem 4rem rgba($color-black, .15);

    &--front {
      background-color: $color-white;
    }

    &--back {
      transform: rotateY(180deg);

      &--1 {
        background-image: linear-gradient(to right bottom, $color-secondary-light, $color-secondary-dark);
      }
    }
  }

  &:hover &__side--front {
    transform: rotateY(180deg);
  }

  &:hover &__side--back {
    transform: rotateY(0);
  }

  // FRONT SIDE STYLING
  &__picture {
    background-size: cover;
    height: 23rem;
    background-blend-mode: screen;
    -webkit-clip-path: polygon(0 0, 100% 0, 100% 85%, 0 100%);
    clip-path: polygon(0 0, 100% 0, 100% 85%, 0 100%);
    border-top-left-radius: 3px;
    border-top-right-radius: 3px;

    &--1 {
      background-image: linear-gradient(to right bottom, $color-secondary-light, $color-secondary-dark), url(../img/nat-5.jpg);
    }
  }

  &__heading {
    font-size: 2.5rem;
    font-weight: 300;
    text-transform: uppercase;
    text-align: right;
    color: $color-white;
    position: absolute;
    top: 12rem;
    right: 2rem;
    width: 75%;
  }

  &__heading-span {
    padding: 1rem 1.5rem;
    -webkit-box-decoration-break: clone;
    box-decoration-break: clone;

    &--1 {
      background-image: linear-gradient(to right bottom, $color-secondary-light, $color-secondary-dark);
    }
  }

  &__details {
    padding: 3rem;

    ul {
      list-style: none;
      width: 80%;
      margin: 0 auto;

      li {
        text-align: center;
        font-size: 1.5rem;
        padding: 1rem;

        &:not(:last-child) {
          border-bottom: 1px solid $color-grey-light-2;
        }
      }
    }
  }

  // BACK SIDE STYLING
  &__cta {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 90%;
    text-align: center;
  }

  &__price-box {
    text-align: center;
    color: $color-white;
    margin-bottom: 8rem;
  }

  &__price-only {
    font-size: 1.4rem;
    text-transform: uppercase;
  }

  &__price-value {
    font-size: 6rem;
    font-weight: 100;
  }
}
```

**[⬆ back to top](#table-of-contents)**

#### How to build an amazing, rotating card?

```html
<div class="card">
  <div class="card__side card__side--front">
    FRONT
  </div>
  <div class="card__side card__side--back card__side--back--1">
    BACK
  </div>
</div>
```

```scss
.card {
  perspective: 150rem;
  -moz-perspective: 150rem;
  position: relative;
  height: 52rem;

  &__side {
    height: 52rem;
    transition: all .8s ease;
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    backface-visibility: hidden;
    border-radius: 3px;
    overflow: hidden;
    box-shadow: 0 1.5rem 4rem rgba($color-black, .15);

    &--front {
      background-color: $color-white;
    }

    &--back {
      transform: rotateY(180deg);
    }
  }

  &:hover &__side--front {
    transform: rotateY(180deg);
  }

  &:hover &__side--back {
    transform: rotateY(0);
  }
}
```

**[⬆ back to top](#table-of-contents)**

### 40. Building the Tours Section - Part 2

#### Front Side Card component: Picture, Heading, Details

```html
<section class="section-tours">
  <div class="u-center-text u-margin-bottom-big">
    <h2 class="heading-secondary">
      Most popular tours
    </h2>
  </div>
  <div class="row">
    <div class="col-1-of-3">
      <div class="card">
        <div class="card__side card__side--front">
          <div class="card__picture card__picture--1">&nbsp</div>
          <h4 class="card__heading">
            <span class="card__heading-span card__heading-span--1">
              The Sea Explorer
            </span>
          </h4>
          <div class="card__details">
            <ul>
              <li>3 day tours</li>
              <li>Up to 30 people</li>
              <li>2 tour guides</li>
              <li>Sleep in cozy hotel</li>
              <li>Difficulty: easy</li>
            </ul>
          </div>
        </div>
        <div class="card__side card__side--back card__side--back--1">
          BACK
        </div>
      </div>
    </div>
  </div>
  <div class="u-center-text u-margin-top-huge">
    <a href="#" class="btn btn--green">Discover all tours</a>
  </div>
</section>
```

```scss
.card {
  &__picture {
    background-size: cover;
    height: 23rem;
    background-blend-mode: screen;
    -webkit-clip-path: polygon(0 0, 100% 0, 100% 85%, 0 100%);
    clip-path: polygon(0 0, 100% 0, 100% 85%, 0 100%);
    border-top-left-radius: 3px;
    border-top-right-radius: 3px;

    &--1 {
      background-image: linear-gradient(to right bottom, $color-secondary-light, $color-secondary-dark), url(../img/nat-5.jpg);
    }
  }

  &__heading {
    font-size: 2.5rem;
    font-weight: 300;
    text-transform: uppercase;
    text-align: right;
    color: $color-white;
    position: absolute;
    top: 12rem;
    right: 2rem;
    width: 75%;
  }

  &__heading-span {
    padding: 1rem 1.5rem;
    -webkit-box-decoration-break: clone;
    box-decoration-break: clone;

    &--1 {
      background-image: linear-gradient(to right bottom, $color-secondary-light, $color-secondary-dark);
    }
  }

  &__details {
    padding: 3rem;

    ul {
      list-style: none;
      width: 80%;
      margin: 0 auto;

      li {
        text-align: center;
        font-size: 1.5rem;
        padding: 1rem;

        &:not(:last-child) {
          border-bottom: 1px solid $color-grey-light-2;
        }
      }
    }
  }
}
```

**[⬆ back to top](#table-of-contents)**

#### How to use perspective in CSS?

The [perspective](https://developer.mozilla.org/en-US/docs/Web/CSS/perspective) CSS property determines the distance between the z=0 plane and the user in order to give a 3D-positioned element some perspective.

The perspective property defines how far the object is away from the user. So, a lower value will result in a more intensive 3D effect than a higher value.

When defining the perspective property for an element, it is the CHILD elements that get the perspective view, NOT the element itself.

```scss
.card {
  perspective: 150rem;
  -moz-perspective: 150rem;
}
```

**[⬆ back to top](#table-of-contents)**

#### How to use the backface-visibility property?

The [backface-visibility](https://developer.mozilla.org/en-US/docs/Web/CSS/backface-visibility) CSS property sets whether the back face of an element is visible when turned towards the user.

This div element has "backface-visibility: hidden", and the back face of the div element is invisible:

![](section-05/backface-visibility-hidden.jpg)

This div element has "backface-visibility: visible", and the back face of the div element shows a mirror image of the front face:

![](section-05/backface-visibility-visible.jpg)

```html
<div class="card">
  <div class="card__side card__side--front">
    
  </div>
  <div class="card__side card__side--back card__side--back--1">
    
  </div>
</div>
```

```scss
.card {
  &__side {
    backface-visibility: hidden;

    &--front {
      background-color: $color-white;
    }

    &--back {
      transform: rotateY(180deg);
    }
  }

  &:hover &__side--front {
    transform: rotateY(180deg);
  }

  &:hover &__side--back {
    transform: rotateY(0);
  }
}
```

**[⬆ back to top](#table-of-contents)**

#### Using background blend modes?

The [background-blend-mode](https://developer.mozilla.org/en-US/docs/Web/CSS/background-blend-mode) CSS property sets how an element's background images should blend with each other and with the element's background color.

![](section-05/box-decoration-break-slice.jpg)
![](section-05/box-decoration-break-clone.jpg)

```scss
.card {
  &__picture {
    background-size: cover;
    height: 23rem;
    background-blend-mode: screen;

    &--1 {
      background-image: linear-gradient(to right bottom, $color-secondary-light, $color-secondary-dark), url(../img/nat-5.jpg);
    }
  }
}
```

**[⬆ back to top](#table-of-contents)**

#### How and when to use box-decoration-break;

The [box-decoration-break](https://developer.mozilla.org/en-US/docs/Web/CSS/box-decoration-break) CSS property specifies how an element's fragments should be rendered when broken across multiple lines, columns, or pages.

```scss
.card {
  &__heading-span {
    padding: 1rem 1.5rem;
    -webkit-box-decoration-break: clone;
    box-decoration-break: clone;

    &--1 {
      background-image: linear-gradient(to right bottom, $color-secondary-light, $color-secondary-dark);
    }
  }
}
```

**[⬆ back to top](#table-of-contents)**

### 41. Building the Tours Section - Part 3

#### Back Side Card component: CTA

```html
<section class="section-tours">
  <div class="u-center-text u-margin-bottom-big">
    <h2 class="heading-secondary">
      Most popular tours
    </h2>
  </div>
  <div class="row">
    <div class="col-1-of-3">
      <div class="card">
        <div class="card__side card__side--front">
          FRONT
        </div>
        <div class="card__side card__side--back card__side--back--1">
          <div class="card__cta">
            <div class="card__price-box">
              <p class="card__price-only">Only</p>
              <p class="card__price-value">$297</p>
            </div>
            <a href="" class="btn btn--white">Book now</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>
```

```scss
.card {
  &__cta {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 90%;
    text-align: center;
  }

  &__price-box {
    text-align: center;
    color: $color-white;
    margin-bottom: 8rem;
  }

  &__price-only {
    font-size: 1.4rem;
    text-transform: uppercase;
  }

  &__price-value {
    font-size: 6rem;
    font-weight: 100;
  }
}
```

**[⬆ back to top](#table-of-contents)**

#### Green Button

```html
<div class="u-center-text u-margin-top-huge">
  <a href="#" class="btn btn--green">Discover all tours</a>
</div>
```

```scss
.btn {
  &--green {
    background-color: $color-primary;
    color: $color-white;

    &::after {
      background-color: $color-primary;
    }
  }
}
```

**[⬆ back to top](#table-of-contents)**

### 42. Building the Stories Section - Part 1

#### Thinking about components

- Secondary Heading
- Story
  - Shape
  - Text
  - Background video
- Text button
 
![](section-05/story-part-1.jpg)

**[⬆ back to top](#table-of-contents)**

#### Story component

```html
<section class="section-stories">
  <div class="u-center-text u-margin-bottom-big">
    <h2 class="heading-secondary">
      We make people genuinely happy
    </h2>
  </div>
  <div class="row">
    <div class="story">
      <figure class="story__shape">
        <img src="img/nat-8.jpg" alt="Person on a tour" class="story__img">
      </figure>
      <div class="story__text">
        <h3 class="heading-tertiary u-margin-bottom-small">I had the best week ever with my family</h3>
        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Error, facilis impedit perspiciatis voluptatum iure odio earum in tenetur explicabo beatae, quas minima iste provident omnis quod deleniti sed pariatur quibusdam!</p>
      </div> 
    </div>
  </div>
</section>
```

```scss
.section-stories {
  padding: 15rem 0;
  background-color: $color-grey-light-1;
}

.story {
  width: 75%;
  margin: 0 auto;
  box-shadow: 0 3rem 6rem rgba($color-black, .1);
  background-color: $color-white;
  border-radius: 3px;
  padding: 6rem;
  padding-left: 9rem;
  font-size: $default-font-size;
  transform: skewX(-12deg);

  &__shape {
    width: 15rem;
    height: 15rem;
    float: left;
    -webkit-shape-outside: circle(50% at 50% 50%);
    shape-outside: circle(50% at 50% 50%);
    -webkit-clip-path: circle(50% at 50% 50%);
    clip-path: circle(50% at 50% 50%);
    transform: translateX(-3rem) skewX(12deg);
  }

  &__img {
    height: 100%;
  }

  &__text {
    transform: skewX(12deg);
  }
}
```

**[⬆ back to top](#table-of-contents)**

#### How to make text flow around shapes with shape-outside and float?

The [shape-outside](https://developer.mozilla.org/en-US/docs/Web/CSS/shape-outside) CSS property defines a shape—which may be non-rectangular—around which adjacent inline content should wrap.

```scss
.story {
  width: 75%;
  margin: 0 auto;
  box-shadow: 0 3rem 6rem rgba($color-black, .1);
  background-color: $color-white;
  border-radius: 3px;
  padding: 6rem;
  padding-left: 9rem;
  font-size: $default-font-size;
  transform: skewX(-12deg);

  &__shape {
    width: 15rem;
    height: 15rem;
    float: left;
    -webkit-shape-outside: circle(50% at 50% 50%);
    shape-outside: circle(50% at 50% 50%);
    -webkit-clip-path: circle(50% at 50% 50%);
    clip-path: circle(50% at 50% 50%);
    transform: translateX(-3rem) skewX(12deg);
  }

  &__img {
    height: 100%;
  }
}
```

**[⬆ back to top](#table-of-contents)**

### 43. Building the Stories Section - Part 2

![](section-05/story-figure-caption.jpg)

**[⬆ back to top](#table-of-contents)**

#### Story Shape component - Figure Caption

The HTML [`<figcaption>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/figcaption) or Figure Caption element represents a caption or legend describing the rest of the contents of its parent `<figure>` element.

```html
<div class="story">
  <figure class="story__shape">
    <img src="img/nat-8.jpg" alt="Person on a tour" class="story__img">
    <figcaption class="story__caption">
      Mary Smith
    </figcaption>
  </figure>
</div>
```

```scss
.story {
  &__shape {
    position: relative;
    overflow: hidden;
  }

  &__img {
    height: 100%;
    transform: translateX(-4rem) scale(1.4);
    backface-visibility: hidden;
    transition: all 0.5s;
  }

  &__caption {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, 20%);
    color: $color-white;
    text-transform: uppercase;
    font-size: 1.7rem;
    text-align: center;
    opacity: 0;
    transition: all 0.5s;
    backface-visibility: hidden;
  }

  &:hover &__caption {
    opacity: 1;
    transform: translate(-50%, -50%);
  }

  &:hover &__img {
    transform: translateX(-4rem) scale(1);
    filter: blur(3px) brightness(80%);
  }
}
```

**[⬆ back to top](#table-of-contents)**

### 44. Building the Stories Section - Part 3

![](section-05/bg-video.jpg)

**[⬆ back to top](#table-of-contents)**

#### Story component - Background video

[Coverr: Free Stock Footage | Royalty Free Videos for Download](https://coverr.co)

```html
<div class="bg-video">
  <video class="bg-video__content" autoplay muted>
    <source src="img/video.mp4" type="video/mp4" />
    <source src="img/video.webm" type="video/webm" />
    Your browser is not supported!
  </video>
</div>
```

```scss
.section-stories {
  position: relative;
}

.story {
  background-color: rgba($color-white, .6);
}

.bg-video {
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 100%;
  z-index: -1;
  opacity: .15;
  overflow: hidden;

  &__content {
    height: 100%;
    width: 100%;
    object-fit: cover;
  }
}
```

#### How to use the <video> HTML element?

```html
<div class="bg-video">
  <video class="bg-video__content" autoplay muted>
    <source src="img/video.mp4" type="video/mp4" />
    <source src="img/video.webm" type="video/webm" />
    Your browser is not supported!
  </video>
</div>
```

**[⬆ back to top](#table-of-contents)**

#### How to create a background video covering an entire section?

```scss
.section-stories {
  position: relative;
}

.bg-video {
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 100%;
  z-index: -1;
  opacity: .15;
  overflow: hidden;

  &__content {
    height: 100%;
    width: 100%;
    object-fit: cover;
  }
}
```

**[⬆ back to top](#table-of-contents)**

#### How and when to use the object-fit property?

The [object-fit](https://developer.mozilla.org/en-US/docs/Web/CSS/object-fit) CSS property sets how the content of a replaced element, such as an <img> or <video>, should be resized to fit its container.

```scss
.section-stories {
  position: relative;
}

.bg-video {
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 100%;
  z-index: -1;
  opacity: .15;
  overflow: hidden;

  &__content {
    height: 100%;
    width: 100%;
    object-fit: cover;
  }
}
```

**[⬆ back to top](#table-of-contents)**

### 45. Building the Booking Section - Part 1

#### Thinking about components

- Form
  - Secondary Heading
  - Input: Full name and Email address
  - Radio button
  - Green button

![](section-05/book-part-1.jpg)

```html
<section class="section-book">
  <div class="row">
    <div class="book">
      <div class="book__form">
        <form action="" class="form">
          <div class="u-margin-bottom-medium">
            <h2 class="heading-secondary">
              Start booking now
            </h2>
          </div>
          <div class="form__group">
            <input type="text" class="form__input" placeholder="Full Name" id="name" required>
            <label for="name" class="form__label">Full name</label>
          </div>
          <div class="form__group">
            <input type="email" class="form__input" placeholder="Email address" id="email" required>
            <label for="email" class="form__label">Email address</label>
          </div>
        </form>
      </div>
    </div>
  </div>
</section>
```

```scss
.section-book {
  padding: 15rem 0;
  background-image: linear-gradient(to right bottom, $color-primary-light, $color-primary-dark);
}

.book {
  background-image: 
    linear-gradient(
      105deg, 
      rgba($color-white, 0.9) 0%, 
      rgba($color-white, 0.9) 50%, 
      transparent 50%), 
    url(../img/nat-10.jpg);
  background-size: cover;
  border-radius: 3px;
  box-shadow: 0 1.5rem 4rem rgba($color-black, 0.2);

  height: 50rem;

  &__form {
    width: 50%;
    padding: 6rem;
  }
}
```

**[⬆ back to top](#table-of-contents)**

#### How to implement "solid-color gradients"?

The [linear-gradient()](https://developer.mozilla.org/en-US/docs/Web/CSS/linear-gradient) CSS function creates an image consisting of a progressive transition between two or more colors along a straight line. Its result is an object of the `<gradient>` data type, which is a special kind of `<image>`.

```scss
.book {
  background-image: 
    linear-gradient(
      105deg, 
      rgba($color-white, 0.9) 0%, 
      rgba($color-white, 0.9) 50%, 
      transparent 50%), 
    url(../img/nat-10.jpg);
  background-size: cover;
  border-radius: 3px;
  box-shadow: 0 1.5rem 4rem rgba($color-black, 0.2);
  height: 50rem;
}
```

**[⬆ back to top](#table-of-contents)**

### 46. Building the Booking Section - Part 2

#### Input component: Full name and Email address

![](section-05/book-part-2.jpg)

```scss
.form {
  &__group:not(:last-child) {
    margin-bottom: 2rem;
  }

  &__input {
    font-size: 1.5rem;
    font-family: inherit;
    color: inherit;
    padding: 1.5rem 2rem;
    border-radius: 2px;
    background-color: rgba($color-white, .5);
    border: none;
    border-bottom: 3px solid transparent;
    width: 90%;
    display: block;
    transition: all .3s;

    &:focus {
      outline: none;
      box-shadow: 0 1rem 2rem rgba($color-black, .2);
      border-bottom: 3px solid $color-primary;
    }

    &:focus:invalid {
      border-bottom: 3px solid $color-secondary-dark;
    }

    &::-webkit-input-placeholder {
      color: $color-grey-dark-2;
    }
  }

  &__label {
    font-size: 1.2rem;
    font-weight: 700;
    margin-left: 2rem;
    margin-top: .7rem;
    display: block;
    transition: all .3s;
  }

  &__input:placeholder-shown + &__label {
    opacity: 0;
    visibility: hidden;
    transform: translateY(-4rem);
  }
}
```

**[⬆ back to top](#table-of-contents)**

#### How the general and adjacent sibling selectors work and why we need them?

The [general sibling combinator](https://developer.mozilla.org/en-US/docs/Web/CSS/General_sibling_combinator) (~) separates two selectors and matches the second element only if it follows the first element (though not necessarily immediately), and both are children of the same parent element.

The [adjacent sibling combinator](https://developer.mozilla.org/en-US/docs/Web/CSS/Adjacent_sibling_combinator) (+) separates two selectors and matches the second element only if it immediately follows the first element, and both are children of the same parent element.

```html
<form action="" class="form">
  <div class="form__group">
    <input type="text" class="form__input" placeholder="Full Name" id="name" required>
    <label for="name" class="form__label">Full name</label>
  </div>
</div>
```

```scss
.form {
  // form__input and form__label are adjacent siblings
  &__input:placeholder-shown + &__label {
    opacity: 0;
    visibility: hidden;
    transform: translateY(-4rem);
  }
}
```

**[⬆ back to top](#table-of-contents)**

#### How to use the ::input-placeholder pseudo-element?

```scss
.form {
  &__input {
    // customise placeholder text
    &::-webkit-input-placeholder {
      color: $color-grey-dark-2;
    }
  }
}
```

**[⬆ back to top](#table-of-contents)**

#### How and when to use the :focus, :invalid, :placeholder-shown?

The [:focus](https://developer.mozilla.org/en-US/docs/Web/CSS/:focus) CSS pseudo-class represents an element (such as a form input) that has received focus. It is generally triggered when the user clicks or taps on an element or selects it with the keyboard's "tab" key.

The [:invalid](https://developer.mozilla.org/en-US/docs/Web/CSS/:invalid) CSS pseudo-class represents any `<input>` or other `<form>` element whose contents fail to validate.

The [:placeholder-shown](https://developer.mozilla.org/en-US/docs/Web/CSS/:placeholder-shown) CSS pseudo-class represents any `<input>` or `<textarea>` element that is currently displaying placeholder text.

```scss
.form {
  &__group:not(:last-child) {
    margin-bottom: 2rem;
  }

  &__input {
    &:focus {
      outline: none;
      box-shadow: 0 1rem 2rem rgba($color-black, .2);
      border-bottom: 3px solid $color-primary;
    }

    &:focus:invalid {
      border-bottom: 3px solid $color-secondary-dark;
    }

    &::-webkit-input-placeholder {
      color: $color-grey-dark-2;
    }
  }

  // css property is applied when placeholder is shown
  // css property is remove when placeholder is gone, user key in value
  &__input:placeholder-shown + &__label {
    opacity: 0;
    visibility: hidden;
    transform: translateY(-4rem);
  }
}
```

**[⬆ back to top](#table-of-contents)**

### 47. Building the Booking Section - Part 3

#### Techniques to build custom radio buttons

![](section-05/book-part-3.jpg)

```html
<div class="form__group u-margin-bottom-medium">
  <div class="form__radio-group">
    <input type="radio" class="form__radio-input" id="small" name="size">
    <label for="small" class="form__radio-label">
      <span class="form__radio-button"></span>
      Small tour group
    </label>
  </div>
  <div class="form__radio-group">
    <input type="radio" class="form__radio-input" id="large" name="size">
    <label for="large" class="form__radio-label">
      <span class="form__radio-button"></span>
      Large tour group
    </label>
  </div>
</div>
```

```scss
.form {
  &__radio-group {
    width: 49%;
    display: inline-block;
  }

  &__radio-input {
    display: none;
  }

  &__radio-label {
    font-size: $default-font-size;
    cursor: pointer;
    position: relative;
    padding-left: 4.5rem;
  }

  &__radio-button {
    height: 3rem;
    width: 3rem;
    border: 5px solid $color-primary;
    border-radius: 50%;
    display: inline-block;
    position: absolute;
    left: 0;
    top: -.4rem;

    &::after {
      content: "";
      display: block;
      height: 1.3rem;
      width: 1.3rem;
      border-radius: 50%;
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      background-color: $color-primary;
      opacity: 0;
      transition: opacity .2s;
    }
  }

  // form__radio-input:checked
  // form__radio-label is sibling of form__radio-input:checked
  // form__radio-button::after is child of form__radio-label
  &__radio-input:checked ~ &__radio-label &__radio-button::after {
    opacity: 1;
  }
}
```

**[⬆ back to top](#table-of-contents)**

#### Green button

```html
<div class="form__group">
  <button class="btn btn--green">Next step &rarr;</button>
</div>
```

```scss
.btn {
  // add & for the <button> element
  &,
  &:link,
  &:visited {
    ...

    // change for the <button> element
    border: none;
    cursor: pointer;
  }

  // add :focus for the <button> element
  &:active,
  &:focus {
    outline: none;
    ...
  }
}
```

**[⬆ back to top](#table-of-contents)**

#### How and when to use the :checked pseudo-classes?

The [:checked](https://developer.mozilla.org/en-US/docs/Web/CSS/:checked) CSS pseudo-class selector represents any radio (`<input type="radio">`), checkbox (`<input type="checkbox">`), or option (`<option>` in a `<select>`) element that is checked or toggled to an on state.

```scss
.form {
  // form__radio-input:checked
  // form__radio-label is sibling of form__radio-input:checked
  // form__radio-button::after is child of form__radio-label
  &__radio-input:checked ~ &__radio-label &__radio-button::after {
    opacity: 1;
  }
}
```

**[⬆ back to top](#table-of-contents)**

### 48. Building the Footer

#### How to design a simple website footer?

![](section-05/footer.jpg)

```html
<footer class="footer">
  <div class="footer__logo-box">
    <img src="img/logo-green-2x.png" alt="Full logo" class="footer__logo">
  </div>
  <div class="row">
    <div class="col-1-of-2">
      <div class="footer__navigation">
        <ul class="footer__list">
          <li class="footer__item"><a href="#" class="footer__link">Company</a></li>
          <li class="footer__item"><a href="#" class="footer__link">Contact us</a></li>
          <li class="footer__item"><a href="#" class="footer__link">Careers</a></li>
          <li class="footer__item"><a href="#" class="footer__link">Privacy policy</a></li>
          <li class="footer__item"><a href="#" class="footer__link">Terms</a></li>
        </ul>
      </div>
    </div>
    <div class="col-1-of-2">
      <p class="footer__copyright">
        Built by <a href="#" class="footer__link">Jonas Schmedtmann</a> for his online course <a href="#" class="footer__link">Advanced CSS and Sass</a>.
        Copyright &copy; by Jonas Schmedtmann. You are 100% allowed to use this webpage for both personal
        and commercial use, but NOT to claim it as your own design. A credit to the original author, Jonas
        Schmedtmann, is of course highly appreciated!
      </p>
    </div>
  </div>
</footer>
```

```scss
.footer {
  background-color: $color-grey-dark-3;
  padding: 10rem 0;
  font-size: 1.4rem;
  color: $color-grey-light-1;

  &__logo-box {
    text-align: center;
    margin-bottom: 8rem;
  }

  &__logo {
    width: 15rem;
    height: auto
  }
  
  &__navigation {
    border-top: 1px solid $color-grey-dark;
    padding-top: 2rem;
    display: inline-block;
  }
  
  &__list {
    list-style: none;
  }
  
  &__item {
    display: inline-block;

    &:not(:last-child) {
      margin-right: 1.5rem;
    }
  }
  
  &__link {
    &:link,
    &:visited {
      color: $color-grey-light-1;
      background-color: $color-grey-dark-3;
      text-decoration: none;
      text-transform: uppercase;
      display: inline-block;
      transition: all .2s;
    }

    &:hover,
    &:active {
      color: $color-primary;
      box-shadow: 0 1rem 2rem rgba($color-black, .4);
      transform: rotate(5deg) scale(1.3);
    }
  }
  
  &__copyright {
    border-top: 1px solid $color-grey-dark;
    padding-top: 2rem;
    width: 80%;
    float: right;
  }
}
```

**[⬆ back to top](#table-of-contents)**

### 49. Building the Navigation - Part 1
**[⬆ back to top](#table-of-contents)**

### 50. Building the Navigation - Part 2
**[⬆ back to top](#table-of-contents)**

### 51. Building the Navigation - Part 3
**[⬆ back to top](#table-of-contents)**

### 52. Building a Pure CSS Popup - Part 1
**[⬆ back to top](#table-of-contents)**

### 53. Building a Pure CSS Popup - Part 2
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