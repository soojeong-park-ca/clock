# JS + CSS Clock

JS + CSS Clock is a realtime clock website built with Vanilla JavaScript.

## Table of contents

- [Overview](#overview)
  - [Screenshots](#screenshots)
  - [Demo Link](#demo-link)
- [About the Project](#about-the-project)
  - [Status](#status)
  - [Built with](#built-with)
  - [Reflection](#reflection)
- [Author](#author)

## Overview

### Screenshots

![JS + CSS Clock](./js-css-clock-ss.png)

### Demo Link

**[💻 Live Site URL](https://soojeong-park-ca.github.io/clock/)**

## About the Project

### Status

✅ Completed & Deployed

### Built with

- HTML
- CSS
- Vanilla JS

### Reflection

This was another Vanilla JS project from JavaScript 30 course by Wes Bos.

Some features to highlight in this project are:

- using the `transition-timing-function` CSS property to animate the clock hands in a way that looks more real (clock hand briefly going slightly over the time and quickly bouncing back to the actual time)

- using the `transform-origin` CSS property to fix the center axis for the clock hands so they can rotate when the time passes in the way real clocks do

```css
.hand {
  width: 50%;
  height: 6px;
  background: white;
  position: absolute;
  top: 50%;
  left: 0;
  /* set up center axis for clock hands */
  transform-origin: 100%;
  /* start position all pointing at 12 on clock */
  transform: rotate(90deg);
  /* smooth transitioning and real clock-like timing function */
  transition: all 0.05s;
  transition-timing-function: cubic-bezier(0.18, 2.71, 0.44, 0.99);
}
```

Some new CSS tricks that I learned from this project are:

- `transform-origin` CSS property
- setting `<element>.style.<CSS-property> = ""` after assigning a certain inline-style to the `<element>` resets the inline-style to empty, thus going back to the original CSS style from the `<styles>` tag or stylesheet

## Author

Soojeong Park [@codingsooj](https://twitter.com/codingsooj)
