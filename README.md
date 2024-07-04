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
- [Author](#author)



## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot
Desktop View

![](./images/Screenshot%20(137).png)

Mobile View 
![](./images/Screenshot%20(138).png)


### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflows

### What I learned

**Key Learnings:**

1. **CSS Flexbox and Responsive Design:**
   - Utilized CSS Flexbox to create a flexible and responsive layout.
   - Implemented media queries to ensure the design adapts seamlessly across various screen sizes, enhancing the user experience on both mobile and desktop devices.

```css
.entire-page {
    width: 100vw;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    background-color: var(--cream);
}

@media (min-width: 700px) {
    .container {
        width: 80%;
        flex-direction: row;
    }
}

@media (min-width: 1060px) {
    .container {
        width: 50%;
    }
}
```

2. **Typography and Font Styling:**
   - Incorporated Google Fonts to use "Fraunces" and "Montserrat" for a clean and modern look.
   - Applied different font weights and styles to create visual hierarchy and improve readability.

```css
@import url('https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,100..900;1,9..144,100..900&family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap');

.small-heading {
    text-transform: uppercase;
    font-family: Montserrat, sans-serif;
    font-weight: 500;
    letter-spacing: 0.4rem;
    font-size: 15px;
    color: var(--dark-grayish-blue);
}

.large-heading {
    font-size: 2.24rem;
    line-height: 2.5rem;
    font-family: Fraunces;
    color: var(--very-dark-blue);
}
```

3. **CSS Variables:**
   - Defined CSS variables for primary and neutral colors to maintain a consistent color palette throughout the project.
   - This approach streamlined the process of applying and managing colors across the entire stylesheet.

```css
:root {
    /* Primary Color */
    --dark-cyan: hsl(158, 36%, 37%);
    --cream: hsl(30, 38%, 92%);
    /* Neutral Color */
    --very-dark-blue: hsl(212, 21%, 14%);
    --dark-grayish-blue: hsl(228, 12%, 48%);
    --white: hsl(0, 0%, 100%);
}
```

4. **Button Styling and Hover Effects:**
   - Styled the "Add to Cart" button with a distinct background color, padding, and border-radius.
   - Added a hover effect to the button to improve interactivity and provide feedback to the user.

```css
.btn {
    margin: 2rem 0;
    width: 90%;
    padding: 1.3rem;
    border: none;
    border-radius: 1rem;
    background-color: var(--dark-cyan);
}

button:hover {
    cursor: pointer;
}
```

5. **Image Handling:**
   - Managed image sizes and applied border-radius to ensure the images fit well within their containers and maintain a consistent visual style.
   - Used different images for mobile and desktop views to enhance the overall visual presentation.

```css
.page-img {
    width: 100%;
    height: 19rem;
    border-radius: 1rem 1rem 0 0;
}

@media (min-width: 700px) {
    .page-img {
        border-radius: 1rem 0 0 1rem;
        height: 100%;
        width: 100%;
    }
}
```

### Continued Development:

1. **JavaScript Interactivity:**
   - Plan to add JavaScript functionality to make the "Add to Cart" button interactive. This will include updating the cart icon and displaying a notification when an item is added.

2. **Accessibility Enhancements:**
   - Intend to improve the accessibility of the project by adding ARIA labels, ensuring proper focus states, and making the design more navigable using keyboard-only inputs.

3. **Advanced CSS Techniques:**
   - Aim to explore advanced CSS techniques such as CSS Grid for more complex layouts and CSS animations to add subtle effects to enhance user engagement.

4. **Code Optimization:**
   - Plan to refactor and optimize the CSS code for better performance and maintainability, ensuring that the styles are as efficient and clean as possible.


## Author

- GitHub - [Bankole David](https://github.com/BANKOLEDO)
- Frontend Mentor - [@BANKOLEDO](https://www.frontendmentor.io/profile/BANKOLEDO)
- Twitter - [@bankydavid12](https://www.twitter.com/bankydavid12)


