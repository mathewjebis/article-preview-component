# Frontend Mentor - Article preview component solution

This is a solution to the [Article preview component challenge on Frontend Mentor](https://frontendmentor.io). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the component depending on their device's screen size
- See the social media share links when they click the share icon

### Screenshot

_(Tip: Take a screenshot of your finished mobile and desktop states, save them in your project folder, and link them below!)_

- Mobile Layout: `./design/mobile-finished.png`
- Desktop Active State: `./design/desktop-finished.png`

## My process

### Built with

- Semantic HTML5 markup
- CSS Custom Properties (Variables)
- Flexbox layout mechanics
- Mobile-first workflow
- Vanilla JavaScript (DOM manipulation)

### What I learned

During this project, I learned how to handle complex layout context switches between mobile overlays and desktop tooltips using pure CSS absolute positioning and a clean JavaScript toggle structure.

To create the desktop tooltip speech bubble without breaking the document flow, I used CSS pseudo-elements (`::after`) to render the downward-pointing arrow dynamically:

```css
.share-panel::after {
  content: "";
  position: absolute;
  bottom: -8px;
  left: 50%;
  transform: translateX(-50%);
  border-width: 8px 8px 0 8px;
  border-style: solid;
  border-color: var(--Very-Dark-Grayish-Blue) transparent transparent
    transparent;
}
```

## Author

- Frontend Mentor - [@mathewjebis](https://www.frontendmentor.io/profile/mathewjebis)
