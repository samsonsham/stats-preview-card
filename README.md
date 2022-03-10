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

![](https://ik.imagekit.io/c5xc1x6srka/screenshot/screen_stat-preview2_eLWQlAieQ.png)

### Links

- Solution URL: [https://github.com/samsonsham/stats-preview-card](https://github.com/samsonsham/stats-preview-card)
- Live Site URL: [https://samsonsham.github.io/stats-preview-card/](https://samsonsham.github.io/stats-preview-card/)

## My process

- Set up SCSS file structure. Define all the styles given by style guide, including colours and font into SCSS files.
- Define components and setup corresponding DOM elements in HTML file.
- Mobile first, build each elements by with colours, alignment, and adjusting size.
- Then add media query for desktop view.

### Built with

- Semantic HTML5 markup
- SCSS
- Flexbox
- Mobile-first workflow

### What I learned

- Add colour overlay on to `<img>` element.
- `mix-blend-mode: multiply` to mix the image with a colour overlay
- The desktop and mobile pixel provided in style guide are not the breakpoint itself, but the range of resolution I have to deal with.
- Use more meaningful element `<ul>` `<li>`.

```html
<div class="wrap">
  <img src="./images/image-header-mobile.jpg" class="img-mobile" />
  <img src="./images/image-header-desktop.jpg" class="img-desktop" />
</div>
```

```css
.wrap {
  position: relative;
}
.wrap:before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 100%;
  background: $soft_violet_overlay;
  mix-blend-mode: multiply;
  border-radius: 0 5px 5px 0;
  z-index: 999;
}
```

### Useful resources

- [How to add color overlay on an image](https://stackoverflow.com/questions/44673676/how-to-add-color-overlay-on-an-image) - This helped me for the way to put a colour overlay on top of an `<img>` element.

## Author

- Website - [Samson Sham](https://samson-sham-portfolio.vercel.app)
- Frontend Mentor - [@samsonsham](https://www.frontendmentor.io/profile/samsonsham)
- Twitter - [@samson_sham](https://www.twitter.com/samson_sham)

### Acknowledgments

I would like to thank [@D3press3dd](https://www.frontendmentor.io/profile/D3press3dd), [@GrzywN](https://www.frontendmentor.io/profile/GrzywN), [@srglbrkchn](https://www.frontendmentor.io/profile/srglbrkchn), [@vanzasetia](https://www.frontendmentor.io/profile/vanzasetia) for valuable comments, helping and guiding me to improving my image handling and responsive design.
