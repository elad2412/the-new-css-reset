# The New CSS Reset
This new CSS reset is using the new CSS features:
- The global CSS reset keywords, ‘unset’ and ‘revert’ keywords.
- The new property of ‘all’ which can reset all properties combined.
- The :where() pseudo-class to remove specificity.
- The :not() pseudo-class with multi arguments.

## What the-new-css-reset is resetting?
This CSS reset is built from the understanding we don't want to use the default style we are getting from the browsers, except the 'display' property.

This CSS reset removes all the default styles which we are getting on specific HTML elements except the 'display' property, as I already mention, and except special HTML elements like iframe, canvas, img, svg, video.

In case you want the default style of the browser of a specific HTML element back, you can revert back to the default styles of the browser. For example:
```
input[type="checkbox"],
input[type="radio"] {
    all: revert;
}
 ```
 
 or all input elements:
 ```
 input,
 textarea,
 select {
    all: revert;
 }
 ```

[Download the Latest Version](https://raw.githubusercontent.com/elad2412/the-new-css-reset/main/css/reset.css)

## NPM and How to Use ?
The package name at NPM is 'the-new-css-reset'.

Import the /css/reset.css before the regular styles of the project.

In React project, insert to main entry file
```angular2html
import "the-new-css-reset/css/reset.css"
```

## Browser Support
All evergreen browsers 
- Chrome, Edge: version 88+
- FireFox: version 84+
- Safari/iOS browsers: version 14+
- Opera: version 75+
- Samsung Browser: version 15+
