# Frontend Mentor - Testimonials grid section solution

This is a solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![Screenshot](/screenshot.png)

### Links

- Solution URL: [My Solution](https://your-solution-url.com)
- Live Site URL: [Github Pages](https://delanohendrix.github.io/Testimonials-Grid-Section/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

I made an effort to make sure I designed the card to be modular since they all shared the same basic layout. From there I could use the class "tcard" (testimonial card) and do one universal design. Next I was given the choice to either use the psuedo element nth-child to target each card individually or just give each an additional class based on color; I chose to go with the latter to make it easier to see specific adjustments versus overall adjustments to the design.

An example of the universal card layout and the targeted specific design adjustments:

```html
<div class="tcard purple">
  <div class="reviewer">
    <img src="images/image-daniel.jpg" alt="" />
    <p>
      Name <br />
      <span>Verified Graduate</span>
    </p>
  </div>
  <h2 class="quote">Quote Text</h2>
  <p class="review">Review Text</p>
</div>
```

```css
.purple {
  background-color: var(--moderate-violet);
  background-image: url(../images/bg-pattern-quotation.svg);
  background-repeat: no-repeat;
  background-position: top right 10%;
  color: var(--white);
}
.purple .reviewer img {
  border: 2px solid var(--opa-white);
}
.purple .review {
  padding-right: 24px;
}
```

### Useful resources

- [CSS Reference](https://cssreference.io/) - This site helped me by refreshing me on the usage of various css attributes and properties.

## Author

- Frontend Mentor - [@delanohendrix](https://www.frontendmentor.io/profile/delanohendrix)
