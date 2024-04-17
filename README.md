# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### Screenshot

![](./screenshot.jpg)

### Links

- Repository URL: [GitHub](https://github.com/moadavou/qr-code-component)
- Live Site URL: [GitHub Pages](https://moadavou.github.io/qr-code-component/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

I learned very little regarding CSS and HTML for this project. However, this was my first time working with Git and GitHub. Using these tools rendered new challenges for me. I learned how to use the terminal for Git commands, GitHub Desktop, and link responsive files. 

My greatest error was using an absolute path to link the QR code image. 

```html
<img src="/images/image-qr-code.png" alt="QR code">
```

This worked great with the Live Server Extension in VS Code. But the image wouldn't render on GitHub Pages since the link looked for `images` as a direct child of the root folder. Because of how GitHub hosts, the root folder of the site is not actually the same as the root folder of the repositorie.

```html
<img src="./images/image-qr-code.png" alt="QR code">
```

or...

```html
<img src="images/image-qr-code.png" alt="QR code">
```

...makes the file path relative (it looks for `images` as a direct child of the current location).

### Continued development

I want to continue focusing on working with a mobile-first workflow (I usually do desktop-first), responsiveness and accessibility. Since I'm a beginner, I want to make sure that the basics are good. I also want to continue to work with Git and GitHub, to further develop these skills. 

## Author

- Frontend Mentor - [@moadavou](https://www.frontendmentor.io/profile/moadavou)
- GitHub - [@moadavou](https://github.com/moadavou)

## Acknowledgments

[@AlexKMarshall](https://github.com/AlexKMarshall) was very kind and quick in his response when I asked why my QR code image wasn't showing up on GitHub Pages. 