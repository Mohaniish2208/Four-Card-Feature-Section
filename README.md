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

- View the optimal layout for the site depending on their device’s screen size  
- See four feature cards arranged in a centered grid beneath a two-line header and a short paragraph  
- Observe a clean, modern design where each card has a thin colored border on top, an icon tucked into the bottom-right corner, and a slight drop shadow

### Screenshot

![Final Product](Final-Screenshot.png)

Four card feature section showing **Supervisor**, **Team Builder**, **Karma**, and **Calculator** cards arranged in a grid on a clean white background. Each card contains an icon, a heading, and a short description: Supervisor monitors activity to identify project roadblocks, Team Builder scans our talent network to create the optimal team for your project, Karma regularly evaluates our talent to ensure quality, Calculator uses data from past projects to provide better delivery estimates. The page header reads Reliable efficient delivery Powered by Technology. The overall tone is professional and modern.

### Links

- Solution URL: [Solution](https://your-solution-url.com)
- Live Site URL: [Live Site](https://mohaniish2208.github.io/Four-Card-Feature-Section/)

## My process

### Built with

- **Semantic HTML5** markup for a clear document structure  
- **Custom CSS** (desktop-first)  
- **Flexbox** to arrange and center both the intro section and the four cards  
- **Responsive design** adjustments via media queries  
- **Google Fonts:** “Poppins” for all text  
- **HSL color values** for precise control over each card’s top border hue  

### What I learned

Use this section to recap over some of your major learnings while working through this project. Writing these out and providing code samples of areas you want to highlight is a great way to reinforce your own knowledge.

To see how you can add code snippets, see below:

```html
 <section class="masterContainer">
      <section class="containerS">
        <h3 class="super">Supervisor</h3>
        <p class="sPara">Monitors activity to identify project roadblocks</p>
        <img class="imgS" src="images/icon-supervisor.svg" alt="supervisor img">
      </section>

      <section class="jointContainer">
        <section class="containerT">
          <h3 class="team">Team Builder</h3>
          <p class="tPara">Scans our talent network to create the optimal team for your project</p>
          <img class="imgT" src="images/icon-team-builder.svg" alt="team img">
        </section>

        <section class="containerK">
          <h3 class="karma">Karma</h3>
          <p class="kPara">Regularly evaluates our talent to ensure quality</p>
          <img class="imgK" src="images/icon-karma.svg" alt="karma img">
        </section>
      </section>

      <section class="containerC">
        <h3 class="calc">Calculator</h3>
        <p class="cPara">Uses data from past projects to provide better delivery estimates</p>
        <img class="imgC" src="images/icon-calculator.svg" alt="calculator img">
      </section>
    </section>
```
Handled multiple sections (representing 4 cards).

```css
.masterContainer {
  display: flex;
  flex-direction: row;
  gap: 2.5em;
  align-items: center;
  justify-content: center;
  margin: 3.5em;
}
```
Using Flexbox with gap and justify-content: center was key to laying out the four cards in a single row on desktop and centering them automatically.

### Continued development

- Refine Mobile Layout: Right now, the cards are in a single horizontal row. I want to add media queries so that on narrow screens they stack into two rows of two, or a single column on very small devices.

- Explore CSS Grid: While Flexbox worked well for centering, I’d like to experiment with CSS Grid to manage gaps and alignment more granularly, especially if I need unequal spacing in the future.

- Add Hover States: Currently there is no visible hover effect on the cards. I plan to add a subtle scale or shadow change on hover to improve interactivity.

- Improve Accessibility: Ensure all text has adequate contrast and add focus-visible styles so keyboard users can navigate the cards and links clearly.

- Semantic Enhancements: Consider wrapping each card in an appropriate ARIA role or a more specific HTML element (e.g., using <article> for each feature card) to improve semantic meaning.

### Useful resources

MDN Web Docs – [Flexbox Guide](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Basic_Concepts_of_Flexbox)
Helped me understand how justify-content, align-items, and gap work together to center and space flex items.

CSS-Tricks – [Absolute Positioning Inside a Relative Parent](https://css-tricks.com/absolute-positioning-inside-relative-parent/)
A clear explanation of how to pin child elements inside a parent by using position: relative and position: absolute.

[Google Fonts](https://fonts.google.com/specimen/Poppins)
Used to import and apply the “Poppins” font for headings and paragraph text.


## Author

- Frontend Mentor - [@Mohaniish2208](https://www.frontendmentor.io/profile/Mohaniish2208)

## Acknowledgments

Thanks to Frontend Mentor for the detailed design, which challenges me to build real-world layouts.