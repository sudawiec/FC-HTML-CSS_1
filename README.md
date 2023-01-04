# FC-HTML-CSS_1

The final project of the HTML/CSS module of the Future Collars Bootcamp

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

Project is based on Figma project design provided by Future Collars

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements
- See smooth scroll animation after clicking the links
- Click a hamburger button on the small screen's sizes and see the vertical menu 

### Screenshot

![The project no.1 website preview](./imgs/project-no1.png)

### Links

- Source code URL: [https://github.com/sudawiec/FC-HTML-CSS_1](https://github.com/sudawiec/FC-HTML-CSS_1)
- Live site URL: [https://fabulous-nasturtium-720f96.netlify.app](https://fabulous-nasturtium-720f96.netlify.app)

## My process

### Built with

- Semantic HTML markup
- Flexbox
- Mobile-first workflow
- CSS custom properties(variables)

### What I learned

- Usage of the :nth-of-type() selector with (odd) and (even) keywords

```css
.person:nth-of-type(odd) {
  margin-bottom: 2.33em;
}
.person:nth-of-type(even) {
  flex-direction: row-reverse;
}
```

- CSS transitions which allows me to change property values smoothly, over a given duration

```css
.box {
  transition: all 0.5s ease;
}
```

- The transform property which let me rotate, scale, skew, and translate an element

```css
.box:hover {
  transform: scale(1.05);
}
```

- Creating some elements using ::after and ::befor pseudo-elements and theirs positioning

```css
.nav-toggle__hamburger {
  position: relative;
}
.nav-toggle__hamburger,
.nav-toggle__hamburger::after,
.nav-toggle__hamburger::before {
  width: 35px;
  height: 3px;
  background-color: var(--white);
}
.nav-toggle__hamburger::after,
.nav-toggle__hamburger::before {
  content: '';
  position: absolute;
  inset: auto 0 auto 0;
}
.nav-toggle__hamburger::after {
  bottom: 10px;
}
.nav-toggle__hamburger::before {
  top: 10px;
}
```

- Usage of [cubic-bezier()](https://css-tricks.com/advanced-css-animation-using-cubic-bezier/) function

```css
.vertical-nav {
  transform: transition 250ms cubic-bezier(0.5, 0, 0.5, 1);
}
```

### Continued development

The next step I'm going to focus on:

- Resolve some bug issues with a hamburger navigation
- Making boxes clickable and redirectable

### Useful resources

- [MDN Web Docs](https://developer.mozilla.org/en-US/) - Great and irreplaceable resource of knowledge
- [W3Schools](https://www.w3schools.com/) - Great and irreplaceable resource of knowledge
- [CSS-Tricks](https://css-tricks.com/) - They have handy solutions with nice graphic design

## Author

- Radek Warakomski - [sudawiec](https://github.com/sudawiec)
