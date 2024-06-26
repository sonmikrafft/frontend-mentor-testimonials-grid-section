# Frontend Mentor - Testimonials grid section solution

This is a solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![Desktop](./screenshots/desktop.png)
![Mobile](./screenshots/mobile.png)


## My process

### Built with

- CSS Grid
- HTML and SCSS
- Mobile-first workflow
- Webstorm with pre-built server and File Watcher with SCSS for building CSS

### What I learned

Use this section to recap over some of your major learnings while working through this project. Writing these out and providing code samples of areas you want to highlight is a great way to reinforce your own knowledge.

To see how you can add code snippets, see below:

- Grid:
```css
.grid {
  display: grid;
  gap: 1.5rem;
  grid-template-areas: "violet_item" "gray_item" "white_item" "black_item" "white2_item";

  @include breakpoint-up(large) {
    grid-template-columns: 1fr 1fr 1fr 1fr;
    grid-template-areas: "violet_item violet_item gray_item white2_item" "white_item black_item black_item white2_item";
  }
  
  &__item {
    border-radius: 0.5rem;
    padding: 1.5rem 1.75rem;
  }
}

.violet {
  grid-area: violet_item; 
}
```
- Background-Image behind text:
```css
.violet {
  position: relative;

  &:before {
    content: "";
    position: absolute;
    background-image: url("/images/bg-pattern-quotation.svg");
    background-size: cover;
    background-repeat: no-repeat;
    top: 0rem;
    right: 1rem;
    width: 6.5rem;
    height: 6.5rem;
  }

  &__text {
    position: relative; 
  }
}
```

### Useful resources

- [An Interactive Guide to CSS Grid](https://www.joshwcomeau.com/css/interactive-guide-to-grid/) 


## Author

- Github - [Sonja Krafft](https://www.github.com/sonmikrafft)
- Frontend Mentor - [@sonmikrafft](https://www.frontendmentor.io/profile/sonmikrafft)