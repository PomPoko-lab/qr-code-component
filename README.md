# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)

## Overview

### Screenshot

![](images/completed.jpg)

### Links

- Solution URL: [https://www.frontendmentor.io/solutions/qr-code-component-with-flexbox-hpl2Uh1SS](https://www.frontendmentor.io/solutions/qr-code-component-with-flexbox-hpl2Uh1SS)
- Live Site URL: [https://pompoko-lab.github.io/qr-code-component/](https://pompoko-lab.github.io/qr-code-component/)

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

The main challenge I came across was forcing the footer to the bottom of the page.

```css
.footer-class {
  position: fixed;
  bottom: 0;
  text-align: center;
  width: 100%;
}
```

After some peer reviews, flexbox was implemented into the body (or main) to better format the component.

My main challenge here was implementing the width of the card to be calculated by flex-basis. My conclusion was to addd `min-width: 0;` to the card element itself.

```css
main {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
}

.card {
  flex: 0 0 350px;
  min-width: 0;
}
```
