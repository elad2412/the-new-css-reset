# ⏪ The New CSS Reset
**A package that resets some of the default, user agent based, styles.**

It **doesn't** affect the `display` property and special HTML elements like ```iframe```, ```canvas```, ```img```, ```svg``` and ```video```.

**This package is using the new CSS features:**
- The global CSS reset keywords, `unset` and `revert` keywords.
- The new property of `all` which can reset all properties combined.
- The ```:where()``` pseudo-class to remove specificity.
- The ```:not()``` pseudo-class with multi arguments.

## Motivation
This package is built with the understanding that we don’t want to use default styles we are getting from the browsers, except for the `display` property.

## How to get started?
**Run ```npm i the-new-css-reset``` OR [Download the Latest Version](https://raw.githubusercontent.com/elad2412/the-new-css-reset/main/css/reset.css).**

**Once installed, you can use it in two different ways:**

1) Import ```/css/reset.css``` before the regular styles of the project.
2) Include the following snippet in one of the JavaScript/TypeScript entry files:
```js
import "the-new-css-reset/css/reset.css";
```

## Want to exclude some of the resets?

**You can revert to the default styles of the browser!**

For example:


```css
input[type="checkbox"],
input[type="radio"] {
    all: revert;
}
 ```
 
 or all input elements:
 ```css
 input,
 textarea,
 select {
    all: revert;
 }
 ```

## Accessibility Recommendation

**To keep your website accessible, don't forget to take care of the ```:focus``` states.**
```css
:focus { /* focus styles */ }

/* or/and */

:focus-visible { /* keyboard only focus styles */ }
```

## Browser Support

![Chrome](https://raw.githubusercontent.com/alrra/browser-logos/master/src/chrome/chrome_48x48.png) | ![Edge](https://raw.githubusercontent.com/alrra/browser-logos/master/src/edge/edge_48x48.png) | ![Firefox](https://raw.githubusercontent.com/alrra/browser-logos/master/src/firefox/firefox_48x48.png) | ![Safari](https://raw.githubusercontent.com/alrra/browser-logos/master/src/safari/safari_48x48.png) | ![Opera](https://raw.githubusercontent.com/alrra/browser-logos/master/src/opera/opera_48x48.png) | ![Samsung Internet](https://raw.githubusercontent.com/alrra/browser-logos/master/src/samsung-internet/samsung-internet_48x48.png)
--- | --- | --- | --- | --- | --- |
88+ ✔ | 88+ ✔ | 84+ ✔ | 14+ ✔ | 75+ ✔ | 15+ ✔ |
