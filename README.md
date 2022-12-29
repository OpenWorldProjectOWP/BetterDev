# BetterDev
# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)

## Overview

The goal of this challenge is to reproduce to the best of the dev's ability the landing page of an existing file. The dev is given the imgs/svgs and a limited list of style specs, the rest is up to the dev that is taking on the challenge to figure out.

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Links

- Solution URL: [frontendmentor.com](https://www.frontendmentor.io/solutions/product-preview-card-component-ok4OwXU77e)
- Live Site URL: [vercel.com](https://better-dev-three.vercel.app/)

## My process

I first added all HTML elements into the index file so that I could see how the browser was initially forming the content in 1440px which is the first pixel count given for building the "desktop" version of the site. The next step was to start assigning elements into containers, so I created several container divs ranging from "container" to individual "card" classes to help with specificity within the CSS. After the elements were assigned containers I started formatting the page with vanilla CSS and started by declaring some repeating styles inside of the :root by creating a variable to store them. After the basic style var's were declared I formatted the body itself and then styled the rest of the HTML from top to bottom, left to right. After trial and error I moved on to add some @media queries into the CSS so that I could quickly style the given 375px format for the "mobile" version. The site can easily be altered to add more flexibility between devices but I didn't want to crowd the styles sheet and over-complicate the given challenge.

### Built with

- Semantic HTML5 markup
- CSS custom properties

### What I learned

I learned that even though I have worked on my own projects, trying to develope from an original reference can still be humbling. At first I crowded the HTML with too many div's and things quickly became messy when trying to display elements as flex when each container had so many other items. I was able to determine how to effectively section off my elements from each other (even though I used some unconventional methods) and cut down the required CSS by roughly 100 or so lines.

Nesting some containers (I know...boo) seemed to really help set up the initial formatting and eventually helped with specificity.

---

Using this structure to set up future identifiers for CSS styling may not have been what most dev's would do but it allowed me to avoid messy configurations with flex later on in the challenge, and let's just be honest...it worked!

```html
<p><strong> $149.99 </strong> <em>$169.99</em></p>
```

Creating these variable values to use in my style rules was a huge time saver.

```css
:root {
  /* Primary colors */
  --Dark-cyan: hsl(158, 36%, 37%);
  --cream: hsl(30, 38%, 92%);

  /* Nuetral colors */
  --Very-dark-blue: hsl(212, 21%, 14%);
  --Dark-grayish-blue: hsl(228, 12%, 48%);
  --white: hsl(0, 0%, 100%);

  /* Below is the typography to be used */

  /* Body copy */
  --paragraph: 14px;

  /* fonts - will have google fonts links in html */
  --general: "Montserrat", sans-serif; /*will have 500 & 700 weights */

  --fancy: "Fraunces", serif; /*will have weight a of 700 */
}
```

---

### Continued development

I have a lot to look forward to moving forward. I need to hone my skills when it comes to formatting sites to look a certain way and being able to write clean code to accomlish that goal. Right now it seems that my code is not clean and is definitely my #1 goal for my future projects. As styles get more complicated I need to be more familiar with CSS concepts like grid and table. My semantic skills are solid but I believe there is always room to improve and the methods we use are constantly changing making it a goal to continue to refine and continue to learn all I can to be the most effective when writing semantic markup.

## Author

- Website - [Open World Project](https://openworldproject.dev)
- Frontend Mentor - [@OpenWorldProjectOWP](https://www.frontendmentor.io/profile/OpenWorldProjectOWP)
