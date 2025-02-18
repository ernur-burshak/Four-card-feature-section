# Frontend Mentor - Four card feature section solution

This is a solution to the [Four card feature section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/four-card-feature-section-weK1eFYK). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![](./design/desktop-design.jpg)

### Links

- Solution URL: [solution URL here](https://github.com/ernur-burshak/Four-card-feature-section)
- Live Site URL: [live site URL here](https://ernur-burshak.github.io/Four-card-feature-section/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

- In this lesson, I taught you how to use CSS Grid. In the beginning it was difficult to understand, then I learned and did a good job.
- Used header.
- I learned some css styles.

```html
<header>
  <div>
    <h1 class="">Reliable, efficient delivery</h1>
    <h2>Powered by Technology</h2>
  </div>
  <p class="header-description">
    Our Artificial Intelligence powered tools use millions of project data
    points to ensure that your project is successful
  </p>
</header>
```

```css
.card::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 5px;
  border-radius: 8px 8px 0 0;
}
```

```css
@media (min-width: 48rem) and (max-width: 64rem) {
  .cards-container {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: auto auto auto;
    gap: 32px;
    justify-items: center;
  }

  .card-cyan {
    grid-column: 1 / 3; /* Занимает две колонки */
    grid-row: 1;
  }

  .card-red {
    grid-column: 1 / 2; /* занимает только 1-ю колонку.*/
    grid-row: 2;
  }

  .card-yellow {
    grid-column: 2 / 3; /*занимает 2-ю колонку.*/
    grid-row: 2;
  }

  .card-blue {
    grid-column: 1 / 3; /* Занимает две колонки */
    grid-row: 3;
  }

  h1,
  h2 {
    font-size: 2.25rem;
  }

  header {
    width: 33.75rem;
  }
}
```

```css
@media (min-width: 64.0625rem) {
  .cards-container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: auto auto;
    gap: 32px;
    justify-items: center;
    align-items: center;
  }

  .card {
    width: 21.875rem;
    max-width: none;
  }

  .card-cyan {
    grid-column: 1; /* Занимает две колонки */
    grid-row: 1 / 3;
  }

  .card-red {
    grid-column: 2;
    grid-row: 1 / 2;
  }

  .card-yellow {
    grid-column: 2;
    grid-row: 2 / 3;
  }

  .card-blue {
    grid-column: 3; /* Занимает две колонки */
    grid-row: 1 / 3;
  }

  h1,
  h2 {
    font-size: 2.25rem;
  }

  header {
    width: 33.75rem;
  }
}
```

### Continued development

I want to improve my skills in using Grid.

### Useful resources

- [resource 1](https://www.frontendmentor.io/) - He helped me discover the Flexbox and Grid theme.
- [resource 2](https://chatgpt.com/) - He helped me write the code.

## Author

- Website - [Ernur](https://ernur-burshak.github.io/Four-card-feature-section/)
- Frontend Mentor - [@ernur-burshak](https://www.frontendmentor.io/profile/ernur-burshak)
- Linkedin - [Ernur Burshak](https://www.linkedin.com/in/ernur-burshak-7b6b0b31b?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app)

## Acknowledgments

I always thank the Frontend Mentor platform for giving me a good practice.
