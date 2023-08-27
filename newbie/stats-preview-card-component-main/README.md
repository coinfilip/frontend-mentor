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
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Screenshot

![](./Screenshot.png)

### Links

- Solution URL: [Github](https://github.com/coinfilip/frontend-mentor/tree/main/newbie/stats-preview-card-component-main)
- Live Site URL: [Github Pages](https://coinfilip.github.io/frontend-mentor/newbie/stats-preview-card-component-main/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

This is one of the stressful challenges yet as hours are spent on trying to replicate the same spacing and sizes of the fonts from the designs provided. One of the things I learned is not to be keen on trying to perfect things, especially on styling. 

One of the roadblocks I immediately faced on is adding the image that is purely black and white and showing it with a shade of violet as shown in the design preview files. The solution I found is not so ideal but it comes close to the desired result:

```css
.right {
  background-color: var(--soft-violet);
  background-blend-mode: multiply;
}
```

Also, for the mobile design, another roadblock is the image added not displaying in its entirety after adding the background declaration. Rushed to Google and MDN to check, and found the ```background-size``` property. 

```css
.right {
  background: url(../images/image-header-mobile.jpg) no-repeat top center;
  background-size: cover;
}
```

### Continued development

Looks like I need to be exposed on a lot of CSS properties to be more equipped on the succeeding challenges I will take. That and also trying to be familiar with the underutilized and slowly decaying knowledge of CSS Grid.

### Useful resources

- [background-size MDN reference](https://developer.mozilla.org/en-US/docs/Web/CSS/background-size) - This helped me to have the image cover the whole container instead of showing a zoomed out version of the image on mobile size.
- [How to overlay image with color in CSS | Stackoverflow](https://stackoverflow.com/a/69440151) - Although it does not match exactly with the ones in desktop and mobile design, it helped me to overlay a color on top of the mostly black and white image provided by the challenge.

## Author

- Website - [Github  Profile](https://github.com/coinfilip)
- Frontend Mentor - [@coinfilip](https://www.frontendmentor.io/profile/coinfilip)

## Acknowledgments

- The Odin Project
- those behind the sites cited in Useful resources section
- Frontend Mentor for the opportunity to take on this challenge
