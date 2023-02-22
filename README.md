# Frontend Mentor - Landing Page for Online Courses

A solution provided by jefflangtech [Skilled e-learning landing page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/skilled-elearning-landing-page-S1ObDrZ8q).

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

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![](./preview.png)

### Links

- Solution URL: [Frontend Mentor Solution](https://your-solution-url.com)
- Live Site URL: [Github Repo](https://jefflangtech.github.io/elearning-landing-page/index.html)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid

### What I learned

This page layout seemed primed for grid, and I learned how to implement auto-fill with some fancy calculations with custom variables to fit the layout to the screen size as it changed. 

This is the first time I've thought about using custom variables in this fashion, and although I think the practice could spin out of control and result in unreadable code, it makes for some interesting use cases.

Gotta give credit to Mike Herchel for his blog post on CSS-TRICKS: [An Auto-Filling CSS Grid With Max Columns of a Minimum Size](https://css-tricks.com/an-auto-filling-css-grid-with-max-columns/)

```css
      .courses {
        max-width: 118rem;
        --grid-column-gap: 1.88rem;
        padding-inline: 10.3rem;
        margin-inline: auto;
        display: grid;
        grid-template-columns: repeat(auto-fill, minmax(max(16.5rem, calc((100% / 3) - var(--grid-column-gap))), 1fr));
        row-gap: 3.5rem;
        column-gap: var(--grid-column-gap);
        padding-bottom: 8.75rem;
        padding-top: 1.5rem;
      }
```

### Continued development

While I get faster, more comfortable with different layouts and systems, I will probably focus on the big constructs like flexbox and grid. Those, along with incorporating more of the tricks that come with them, seem to have a lot of uses.

### Useful resources

As always, Kevin Powell for the win...

- [Kevin Powell - You can do that with margins?](https://www.youtube.com/watch?v=Azfj1efPAH0) - This was exactly what I need to get the spacing correct on the class cards.

## Author

- Website - [JeffLangTech](https://jefflangtech.github.io/)
- Frontend Mentor - [@jefflangtech](https://www.frontendmentor.io/profile/jefflangtech)
- Twitter - [@jefflangtech](https://www.twitter.com/jefflangtech)

