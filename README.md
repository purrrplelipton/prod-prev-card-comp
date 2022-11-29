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
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

![](/design/purrrplelipton-screenshot.jpg)

### Links

- Solution URL: [Add solution URL here](https://github.com/prod-prev-card-comp.git)
- Live Site URL: [Add live site URL here](https://purrrplelipton.github.io/prod-prev-card-comp/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

I learnt how powerful the picture tag in HTML can be and was introduced to the :is pseudo class in CSS, see below:

````html
<picture class="prod_img">
  <source
    srcset="/images/image-product-desktop.jpg"
    media="(min-width: 625px)"
  />
  <img
    src="/images/image-product-mobile.jpg"
    alt="chanel gabrielle perfume laying on a white surface with green leaves at the top left and bottom right of it"
  /> </picture
>``` ```html
<div class="flex-group">
  <p class="prod_prc">
    <span class="sr-only">Current Price:</span>
    $149.99
  </p>
  <p class="prod_orgnl-prc">
    <span class="sr-only">Original Price:</span>
    <s>$169.99</s>
  </p>
</div>
````

```css
.sr-only:not(:focus):not(:active) {
  clip: rect(0 0 0 0);
  clip-path: inset(50%);
  height: 1px;
  overflow: hidden;
  position: absolute;
  white-space: nowrap;
  width: 1px;
}
```

If you want more help with writing markdown, we'd recommend checking out [The Markdown Guide](https://www.markdownguide.org/) to learn more.

### Continued development

This project just brought the picture tag to my notice. I wish to use it more often now. And some element that cant be read out properly like the crossed out previous price, need extra steps to make them make sense to people who need aid.

### Useful resources

- [Modern CSS Reset / Global Styles](https://www.joshwcomeau.com/css/custom-css-reset/) - This helped me with basic CSS resetting, a always donn't know what to change whe i'm starting a project. I really liked this pattern and will use it going forward.
- [Kevin Powell](https://www.youtube.com/@KevinPowell) - This is a video which helped me understand the Picture tag in HTML. I'd recommend it to anyone still learning this concept.

## Author

- Frontend Mentor - [@purrrplelipton](https://www.frontendmentor.io/profile/purrrplelipton)
- Twitter - [@purrrplelipton](https://www.twitter.com/purrrplelipton)

## Acknowledgments

- Jennifer - [@Jennifer-Iheanacho](https://www.linkedin.com/in/jennifer-iheanacho-654497216/)
