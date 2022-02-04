# The New CSS Reset
This new CSS reset is using the new CSS features:
- The global CSS reset keywords, ‘unset’ and ‘revert’ keywords.
- The new property of ‘all’ which can reset all properties combined.
- The ```:where()``` pseudo-class to remove specificity.
- The ```:not()``` pseudo-class with multi arguments.

## What is the-new-css-reset resetting?
This CSS reset is built from the understanding that we don’t want to use default styles we are getting from the browsers, except the ‘display’ property.

This CSS reset removes all the default styles which we are getting on specific HTML elements except the ‘display’ property, as I already mentioned, and special HTML elements like ```iframe```, ```canvas```, ```img```, ```svg```, and ```video```.

In case you want the default style of the browser of a specific HTML element back, you can revert back to the default styles of the browser. For example:
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

[Download the Latest Version](https://raw.githubusercontent.com/elad2412/the-new-css-reset/main/css/reset.css)

## NPM and How to Use?
The package name on NPM is 'the-new-css-reset'.

Import ```/css/reset.css``` before the regular styles of the project.

In a React project, insert it to the main entry file:
```js
import "the-new-css-reset/css/reset.css"
```

## Accessibility Recommendation

To keep your website accessibly, don't forget to take care of the ```:focus``` states.
```css
:focus { /* focus styles */ }

/* or/and */

:focus-visible { /* keyboard only focus styles */ }
```

## Browser Support
All evergreen browsers 
- Chrome, Edge: version 88+
- FireFox: version 84+
- Safari/iOS browsers: version 14+
- Opera: version 75+
- Samsung Browser: version 15+
