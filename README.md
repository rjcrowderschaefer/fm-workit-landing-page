# Frontend Mentor - Workit landing page solution

This is a solution to the [Workit landing page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/workit-landing-page-2fYnyle5lu). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- View the optimal layout for the interface depending on their device's screen size
- See hover and focus states for all interactive elements on the page

### Screenshot

![Mobile](https://i.imgur.com/yNmZ8Kt.png)
![Tablet](https://i.imgur.com/KtyNXFw.png)
![Desktop](https://i.imgur.com/Hcwv9Wm.png)
![Desktop - "Learn More" hover](https://i.imgur.com/HPq0qCd.png)
![Desktop - "Apply for access" link hover](https://i.imgur.com/KZmkCZU.png)
![Desktop - "Apply for access" button hover](https://i.imgur.com/9CpwIgk.png)

### Links

- [GitHub Repo](https://github.com/rjcrowderschaefer/fm-workit-landing-page)
- [Live Site URL](https://main--sensational-syrniki-131233.netlify.app/)

## My process

I used a mobile first approach for the development of this site with a breakpoint of 393px and then developed the tablet view at 768px and the desktop view at 1440px. I leveraged semantic HTML when and where possible and focused on keeping the CSS clean and concise in an attempt to keep the code as DRY as possible. This was my first time leveraging the overflow:hidden property in conjunction with absolute and relative positioning in order to place the svg assets throughout the page.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

This project allowed me to work specifically with three distince breakpoints, leading with mobile first, and how to apply svg assets in various absolute positions throughout the page. I also worked with specific CSS styling techniques that I hadn't used previously, including the border-bottom radius properties to apply container-specific styling. Although not exact to the markup, I got the design as close as possible and have some additional areas to research and imporve upon moving forward.

To see how you can add code snippets, see below:

```html
<section class="insights-container">
      <article class="insights-block">
      <div class="insights-num">1</div>
      <p class="insights-description">
        <span class="insights-header">Actionable insights</span>
        <span class="insights-detail">
        Optimize your products, improve customer satisfaction and stay ahead of
        the competition with our product data analytics.
      </span>
      </p>
      ....
      </section>
```
<!-- Setting up the insights container with various levels, including article, div, p and span elements allowed me to easily adjust the layout for each breakpoint without requiring the restructuring of my HTML -->

```css
.insights-container {
  display: flex;
  justify-content: center;
  flex-direction: column;
  text-align: center;
  background-color: #FCF8FF;
  padding-top: 115px;
  padding-bottom: 65px;
  color: #24053E;
  border-bottom-left-radius: 100% 50px;
  border-bottom-right-radius: 100% 50px;
  box-shadow: 0px 5px 5px .5px #979797;
  margin-bottom: 75px;
}
```
<!-- The design of this container required a curved buttom border with a box shadow applied. The curved bottom border took quite a bit of troubleshooting and I got this almost to the design spec -->

### Continued development

This project allowed me to practice how to organize and layer relative parent elements and their corresponding absolute child elements. I was also able to troubleshoot how to include container elements that may not be visible on the page but are required to implement certain properties like overflow:hidden to some of the absolute positioned elements. A few areas of continued developmenta and practice for myself moving forward:

- How to apply curved borders that allow for straight edges at the corners instead of the slightly rounded edges provided with the border-bottom-left-radius and similar properties.
- How to build a truly responsive website that responds and adapts to the breakpoints between the primary breakpoints.
- How to align with best practices when using relative and absolute positioning with parent and child elements. How do I ensure that the absolute elements remain positioned where expected as the viewport width expands and contracts in between the primary breakpoints.

## Author

- LinkedIn - [RJ Crowder-Schaefer](https://www.linkedin.com/in/rjcrowderschaefer/)
- Frontend Mentor - [@rjcrowderschaefer](https://www.frontendmentor.io/profile/rjcrowderschaefer)
- GitHub - [@rjcrowderschaefer](https://github.com/rjcrowderschaefer)
