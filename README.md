# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- View the optimal layout depending on their device's screen size

### Screenshot

![](./screenshot.jpg)


### Links

- [Solution URL](https://your-solution-url.com)
- [Live Site URL](https://stats-preview-card-component-one-pi.vercel.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow


### What I learned

Using the ARIA list and listitem roles here comes back as a warning (unnecessary) from the W3C validator, but given I've removed the default list stying I'm not entirely sure the roles aren't completely useless. At the very least, I don't think it's hurting anything. And given that I'm trying to become more aware and consistent with my implementation of accessibility features in my code using the roles here helps build up some muscle memory.

```html
<ul role="list" class="card-content__stats-list">
  <li role="listitem" class="stats-list-item">
    <span class="card-stat__number">10k+</span> <span class="card-stat__label">companies</span>
  </li>
  <li role="listitem" class="stats-list-item">
    <span class="card-stat__number">314</span> <span class="card-stat__label">templates</span>
  </li>
  <li role="listitem" class="stats-list-item">
    <span class="card-stat__number">12M+</span> <span class="card-stat__label">queries</span>
  </li>
</ul> HTML code I'm proud of</h1>
```

Achieving the violet overlay effect on the image using a background color combined with mix-blend-mode and opacity properties seemed like the most straightforward way to go. Though, I'm sure there a few other routes I could have taken. 

```css
.card-image-box {
  background: var(--clr-soft-violet);
}

.card-image-box picture {
  height: 100%;
}

.card-image {
  height: 100%;
  width: 100%;
  object-fit: cover;
  mix-blend-mode: multiply;
  opacity: 0.75;
}
```

### Continued development

This is the first of several component-type projects I plan on working on over the next several months. While most of my dedicated learning time is devoted to JavaScript, React, Node and Python, these types of projects (which are mostly CSS-based) seem like an efficient way to keep my CSS and design skills improving, or at least at a baseline.


## Author

- Website - [Matt Pahuta](https://www.mattpahuta.com)
- Frontend Mentor - [@mattpahuta](https://www.frontendmentor.io/profile/MattPahuta)
- LinkedIn - [Matt Pahuta](www.linkedin.com/in/mattpahuta)
