# Frontend Mentor - Huddle landing page with single introductory section solution

This is a solution to the [Huddle landing page with single introductory section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/huddle-landing-page-with-a-single-introductory-section-B_2Wvxgi0). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- View the optimal layout for the page depending on their device's screen size
- See hover states for all interactive elements on the page

### Screenshot

![](./Screenshot.png)

### Links

- Solution URL: [Github](https://github.com/coinfilip/frontend-mentor/tree/main/newbie/huddle-landing-page-with-single-introductory-section-master)
- Live Site URL: [Github Pages](https://coinfilip.github.io/frontend-mentor/newbie/huddle-landing-page-with-single-introductory-section-master)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- [Font Awesome](https://fontawesome.com/) - For icons

### What I learned

This is my first time to handle a challenge that is not a component (like the previous ones). And with first times, another set of new roadblocks are encountered. 

First is the structure, and second are the icons. 

For this specific challenge, there are 3 main containers created inside **body**. A ```header``` (for the logo), ```main``` (for mockups, text + buttons) and ```footer```(for social media icons).

Almost tried and went the usual way of using one main container inside **body** but end up on the set up above.

On the other hand, icons are quite complicated to handle. With the exception of the last one, almost all of the font icon libraries recommended by Frontend Mentor to use require either a log-in or a monthly subscription, to which I do not desire to use. So I ended up using the offline way, but the journey's not quite straightforward. 

First, I tried to download the SVGs from Font Awesome and include it to the footer section using img. The challenge with this method is the changing of color of those images when a cursor hovers over the element. So, tried to search for a solution on that roadblock until I found another way to include the icons, but not using img elements. 

The second and currently used way to include icons is to copy the code inside the SVG file and paste it inside the html file. 

```html
<svg class="icon-socials" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 320 512"><!--! Font Awesome Pro 6.4.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. --><path d="M279.14 288l14.22-92.66h-88.91v-60.13c0-25.35 12.42-50.06 52.24-50.06h40.42V6.26S260.43 0 225.36 0c-73.22 0-121.08 44.38-121.08 124.72v70.62H22.89V288h81.39v224h100.17V288z"/></svg>
```

Then you can reference it on the CSS file to manipulate the color on your liking, either by using the ```svg``` selector or by another identifier that you'll define on the element.

```css
.icon-socials {
    fill: white;
}
```

Lastly, instead of using ```<link>``` tags on html to include external fonts, I tried the ```@import``` css method for this challenge. Although both does the same thing, one thing I noticed is the way DevTools handles these two. When defining font family values on DevTools, Chrome might not recognize the fonts added thru the ```@import``` css method especially when you add rules directly to the html file/inspector stylesheet. 

```css
@import url('https://fonts.googleapis.com/css2?family=Open+Sans&family=Poppins:wght@400;600&display=swap');
```

### Continued development

Refactoring code is hard and head-scratching. Substituting values from pixels to relative sizes. But I guess it gets better (or worse) as I gain more experience over time. 

Also, I hope I can get myself to use those kits from Font Awesome in the future challenges. My reason for not using it this time is to avoid having dependencies to a tool that may change in the future and have complications with my previous code.

### Useful resources

- [Resize image proportionally with CSS | GeeksforGeeks](https://www.geeksforgeeks.org/resize-image-proportionally-with-css/) - This helped me adopt the ```width``` and ```max-width``` property over the 3 main containers inside body, and also using *auto* as value for ```width``` if a value was set on the ```height``` for an image element like logo.
- [Change Color of SVG on Hover | CSS Tricks](https://css-tricks.com/change-color-of-svg-on-hover/#aa-inline-svg) - This led me to ditch the img and use svg to include icons on the footer section. *Guess that will also be my favorite way to add SVGs*

## Author

- Website - [Github Profile](https://github.com/coinfilip)
- Frontend Mentor - [@coinfilip](https://www.frontendmentor.io/profile/coinfilip)

## Acknowledgments

- The Odin Project
- those behind the sites cited in Useful resources section 
- Frontend Mentor for the opportunity to take on this challenge