# Frontend Mentor - News homepage solution

This is a solution to the [News homepage challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/news-homepage-H6SWTa1MFl). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Frontend Mentor - News homepage solution](#frontend-mentor---news-homepage-solution)
  - [Table of contents](#table-of-contents)
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

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the interface depending on their device's screen size
- See hover and focus states for all interactive elements on the page

### Screenshot
desktop
![image](https://user-images.githubusercontent.com/71990996/210128160-ce3e84eb-a5bc-451a-8f48-6b0864f7d225.png)
![image](https://user-images.githubusercontent.com/71990996/210128169-7ade67b9-ab11-4c0b-84bf-7f10914ae860.png)
mobile
![image](https://user-images.githubusercontent.com/71990996/210128193-2c33b3bd-24b3-4973-a40c-fc8e505cbef9.png)
![image](https://user-images.githubusercontent.com/71990996/210128200-c658c3ba-c52c-4f4a-b624-e5308a8270c6.png)
![image](https://user-images.githubusercontent.com/71990996/210128215-4792bddc-a1e3-4b7b-b79c-4890284fce7c.png)
![image](https://user-images.githubusercontent.com/71990996/210128222-c729ead2-e7f2-49cc-8319-588f8358c7c8.png)



![](./screenshot.jpg)

### Links

- Solution URL: [solution URL here](https://github.com/tobezhanabi/News-homepage)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

I learned the hardway to create a responsive website layout without using CSS Grid or focusing on flexbox. Also learned to create a responsive navigation bar and collapsed it using javascript 

```html
<!--mob version-->
    <div class="mob-menu">
      <a class="mob-logo" href="#"
        ><img src="./assets/images/logo.svg" alt="my logo"
      /></a>
      <img class="mob-open" src="./assets/images/icon-menu.svg" alt="open" />
      <div class="mob-wrapper close">
        <img
          class="mob-close"
          src="./assets/images/icon-menu-close.svg"
          alt="closesvg"
        />
        <div class="mob-list">
          <a href="#" class="mob-list_item">Home</a>
          <a href="#" class="mob-list_item">New</a>
          <a href="#" class="mob-list_item">Popular</a>
          <a href="#" class="mob-list_item">Trending</a>
          <a href="#" class="mob-list_item">Categories</a>
        </div>
      </div>
    </div>
```

```css
.mob-open,
.mob-close {
  width: 40px;
  height: 40px;
}
.mob-open {
  position: fixed;
  right: 85px;
  top: 35px;
}
.mob-logo {
  width: 100%;
  background-color: white;
  height: 50px;
  position: fixed;
  top: 35px;
  float: left;
  left: 85px;
}
.mob-menu {
  padding: 20px;
  background-color: white;
}
.mob-list {
  height: 100%;
  width: 60%;
  top: 0px;
  position: fixed;
  right: 0;
  display: flex;
  flex-direction: column;
  padding-left: 18px;
  align-items: ;
  justify-content: center;
  gap: 30px;
  background-color: white;
}
.mob-list_item {
  font-size: 18px;
}
.mob-list_item:last-child {
  margin-bottom: 60px;
}
```

```js
const open = document.querySelector(".mob-open");
const close = document.querySelector(".mob-close");

const wrapper = document.querySelector(".mob-wrapper").classList;

open.addEventListener("click", () => {
  wrapper.toggle("opened");
  wrapper.toggle("close");
});

close.addEventListener("click", () => {
  wrapper.toggle("opened");
  wrapper.toggle("close");
});

```


### Continued development

I want to learn the standard way to create a responsive website. And also how to create a website with react

### Useful resources

- [resource 1](https://www.w3schools.com/howto/howto_js_collapse_sidebar.asp) - This helped me to understand how collapsed nav bar can be placed but it didnt fully solve my issue of making responsive. 


## Author

- Frontend Mentor - [@tobezhanabi](https://www.frontendmentor.io/profile/tobezhanabi)
- Twitter - [@hanabiplug](https://www.twitter.com/hanabiplug)
