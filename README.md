
# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
- [The challenge](#the-challenge)
- [Screenshot](#screenshot)
- [Links](#links)
- [My process](#my-process)
- [Built with](#built-with)
- [What I learned](#what-i-learned)
- [Continued development](#continued-development)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size
- See hover states for all interactive elements on the page

### Screenshot

![Design Screenshot](./Product_Preview_Card.png)

### Links

- Solution URL: [GitHub Repo](https://github.com/Agalya141/Product_Preview_Card)
- Live Site URL: [Live Demo](https://agalya141.github.io/Product_Preview_Card/)

## My process

### Built with

- Semantic HTML5 markup
- CSS Custom Properties (Variables)
- Flexbox layout model
- Mobile-first/Responsive workflow
- Google Fonts integration (Fraunces + Montserrat)
- `<picture>` element for art-directed responsive images

### What I learned

During this project, I strengthened my understanding of CSS layout mechanics and responsive design. Specifically, I practiced:

1. **Flex `gap` scoping:** Learning that `gap` only applies between the **direct children** of a flex container — an extra wrapper element in between silently breaks it, even though the CSS itself has no error.
2. **Spacing ownership:** Realizing that `padding` set on a parent card leaks into every child, including images meant to sit edge-to-edge — spacing needs to be scoped to the element it's actually meant for.
3. **Deliberate breakpoint overrides:** Making sure a `max-width` set in a media query actually replaces the mobile-first value instead of silently conflicting with it.

```css
/* Example: gap only works on direct children of the flex container */
.text_section {
display: flex;
flex-direction: column;
gap: 0.5rem;
}
```

### Continued development

In future projects, I want to focus on:
- Building spacing systems with intentional hierarchy (varied gaps) instead of one uniform value everywhere.
- Getting more comfortable with responsive image techniques (`<picture>`, `srcset`) without duplicating logic in CSS.
- Writing cleaner, DRY CSS — avoiding repeated resets and duplicate rules across a file.

## Author

- GitHub - [@Agalya141](https://github.com/Agalya141)
- Frontend Mentor - [@Agalya141](https://www.frontendmentor.io/profile/Agalya141)
- LinkedIn - [Agalya M](https://www.linkedin.com/in/agalya6)