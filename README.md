# Frontend Mentor – Recipe Page Solution

This is a solution to the [Recipe page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/recipe-page-KiTsR8QQKm). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

---

## Table of Contents

- [Overview](#overview)

  - [The Challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)

- [My Process](#my-process)

  - [Built With](#built-with)
  - [What I Learned](#what-i-learned)
  - [Continued Development](#continued-development)
  - [Useful Resources](#useful-resources)

- [Author](#author)
- [Acknowledgments](#acknowledgments)

---

## Overview

### The Challenge

Your task was to build a responsive recipe page layout to match the provided design. This included:

- Displaying a high-quality recipe image at the top
- Showing a clear title and description
- Presenting preparation times in a styled box
- Listing ingredients with bullet points
- Displaying step-by-step instructions in an ordered list
- Including a simple nutrition table
- Ensuring the entire layout is fully responsive from mobile up to desktop breakpoints

### Screenshot

<p align="center">
  <img src="./Screenshot 2025-06-06 225153.png" alt="Recipe page – desktop preview" width="400" />
</p>

### Links

- **Solution URL:**
  [https://github.com/syarief02/recipe-page-main](https://github.com/syarief02/recipe-page-main)
- **Live Site URL:**
  [https://syarief02.github.io/recipe-page-main/](https://syarief02.github.io/recipe-page-main/)

---

## My Process

### Built With

- **Semantic HTML5**
- **CSS3** (custom properties, `@font-face`, media queries)
- **Flexbox** (for centering the card container)
- **Mobile-first workflow** (breakpoints at 768px and 1024px)
- **Custom loaded fonts** via `@font-face` (Outfit & Young Serif)

### What I Learned

1. **Loading Local Fonts with `@font-face`:**
   I hosted both **Outfit** (weights 400, 600, 700) and **Young Serif** (weight 400) in `./assets/fonts/…` and learned how to reference them in CSS so they serve correctly in all browsers.

2. **Semantic HTML Structure:**

   - Using an `<article>` element for the recipe card, with nested `<section>` elements for “Preparation time,” “Ingredients,” “Instructions,” and “Nutrition.”
   - This improved accessibility and made the markup more meaningful.

3. **Responsive Breakpoints:**

   - On mobile (up to 767px), the card spans 100% width (max-width: 600px).
   - At 768px, I increased max-width to 680px, bumped font sizes, and adjusted margins/padding.
   - At 1024px, the card’s max-width became 720px and typography scaled further for comfortable desktop reading.

4. **Flexbox Centering:**
   The `<main>` wrapper uses `display: flex; justify-content: center; padding: 2rem 1rem;` to horizontally center the card on all screen sizes.

5. **Styling Lists & Tables:**

   - Styled the “Ingredients” list with `list-style: disc inside;`.
   - Styled the “Instructions” list with `list-style: decimal inside;` and used `<strong>` to bold the opening phrase in each step.
   - Built a simple nutrition table with top/bottom borders between rows for clarity.

6. **Mobile-First Design Approach:**
   Starting with a mobile layout and progressively enhancing for larger viewports made it easier to manage sizing and readability.

### Continued Development

- **Accessibility Improvements:**

  - Add proper ARIA roles (e.g., `role="region"` or `aria-label` on sections) to improve screen reader navigation.
  - Ensure color contrast ratios meet WCAG AA standards (especially for text over background colors).

- **CSS Variables & Theming:**

  - Convert repeated HSL color values into CSS custom properties (e.g., `--stone-100: hsl(30, 54%, 90%)`) to make theming and future maintenance simpler.

- **CSS Grid Exploration:**

  - Although Flexbox was sufficient, experimenting with Grid for a two-column layout (for ingredients + nutrition side-by-side on desktop) could be an interesting exercise.

- **Additional Breakpoints:**

  - Test and refine at mid-range device widths (e.g., 480px, 1200px) for even smoother scaling, especially on tablets.

### Useful Resources

- [Recipe Page Challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/recipe-page-KiTsR8QQKm)
  Official challenge page, design assets, and feedback forum.
- [MDN: `@font-face`](https://developer.mozilla.org/en-US/docs/Web/CSS/@font-face)
  Detailed reference on how to host and load custom fonts.
- [CSS-Tricks: A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
  Comprehensive guide for mastering Flexbox layout.
- [MDN: Responsive Design](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Responsive_Design)
  Tips and best practices on creating responsive layouts using media queries.
- [W3C: Web Content Accessibility Guidelines (WCAG)](https://www.w3.org/WAI/standards-guidelines/wcag/)
  Official accessibility standards to ensure inclusive design.

---

## Author

**Syarief Azman**

- Frontend Mentor – [@syarief02](https://www.frontendmentor.io/profile/syarief02)
- GitHub – [syarief02](https://github.com/syarief02)

Feel free to connect with me if you have any questions or feedback!

---

## Acknowledgments

- Big thanks to **Frontend Mentor** for providing an excellent challenge and design.
- Shout-out to all the community members who shared tips on improving responsive design and typography.
