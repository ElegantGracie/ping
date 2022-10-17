# Frontend Mentor - Ping coming soon page solution

This is a solution to the [Ping coming soon page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/ping-single-column-coming-soon-page-5cadd051fec04111f7b848da). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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
- See hover states for all interactive elements on the page
- Submit their email address using an `input` field
- Receive an error message when the `form` is submitted if:
	- The `input` field is empty. The message for this error should say *"Whoops! It looks like you forgot to add your email"*
	- The email address is not formatted correctly (i.e. a correct email address should have this structure: `name@host.tld`). The message for this error should say *"Please provide a valid email address"*

### Screenshot

 - ![Mobile view](./assets/images/Screenshot1.jpg)
 - ![Larger screens](./assets/images/Screenshot2.jpg) 

### Links

- Solution URL: [Github link](https://github.com/ElegantGracie/ping-coming-soon-page-master)
- Live Site URL: [Live link](https://elegantgracie.github.io/ping-coming-soon-page-master/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

I learnt more about email validation 
```js
  const emailMatch = /^\w+([\.-]?\w+)*@\w+([\.-]?\w+)*(\.\w{2,3})+$/.test(('email').value);
  if(emailMatch) {
          return error.innerText = ""
      }
```
Rediscovered that a link tag could have a border. This was when I was trying to center the icons. I have been using the border of the divs before to create borders around the links
```html
    <div class="icon">
      <a href="#"><i class="fa-brands fa-facebook-f"></i></a>
    </div>
```
```css
  The previous style for the above mentioned HTML was - 
  .icon {
    margin: 0.5rem;  
    color: var(--blue);
    width: 2rem;
    height: 2rem;
    border: 0.5px solid var(--gray);
    border-radius: 50%;
    text-align: center;
    padding: 0.4rem;
  }
  
  Then the stlye I used was - 
  .icon a {
    margin: 0.5rem;  
    color: var(--blue);
    width: 2rem;
    height: 2rem;
    border: 0.5px solid var(--gray);
    border-radius: 50%;
    padding: 2rem auto;
    text-decoration: none;
    display: flex;
    justify-content: center;
    align-items: center;
  }
```

### Continued development

Going further I would continue working on my form validation codes.

### Useful resources

- [Email validation](https://linuxhint.com/email-validation-javascript/) - This is the article that helped with my understanding of email validation.

## Author

- Frontend Mentor - [@ElegantGracie](https://www.frontendmentor.io/profile/ElegantGracie)
- Twitter - [@Elegant_Gracie_](https://www.twitter.com/Elegant_Gracie_)

## Acknowledgments

Thank you Naima Aftab, your article on email validation was a great help. Also Techathon bootcamp, thank you for bringing frontendmentor my way.
