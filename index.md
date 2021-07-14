# The New CSS Reset

This new CSS reset is using the new CSS features:
- The global CSS reset keywords, ‘unset’ and ‘revert’ keywords.
- The new property of ‘all’ which can reset all properties combined.
- The :where() pseudo-class to remove specificity.
- The :not() pseudo-class with multi arguments.

[Download the Latest Version](https://raw.githubusercontent.com/elad2412/the-new-css-reset/main/css/reset.css)

## How it Looks and Works
```
/*** The new CSS Reset - version 1.0.0 (last updated 8.7.2021) ***/

/* Remove all the styles of the "User-Agent-Stylesheet", except for the 'display' property */
*:where(:not(iframe, canvas, img, svg, video):not(svg *)){
    all: unset;
    display: revert;
}

/* Preferred box-sizing value */
*,
*::before,
*::after{
    box-sizing: border-box;
}

/* Remove list styles (bullets/numbers) */
ol, ul {
    list-style: none;
}

/* For images to not be able to exceed their container */
img {
    max-width: 100%;
}

/* removes spacing between cells in tables */
table{
    border-collapse: collapse;
}


```
## Browsers Support
All evergreen browsers (except Samsung Internet browser version 14, will be support in the next version).

## Extensive Reading and Watching
- [Understanding the “Initial”, “Inherit” and “Unset” CSS Keywords](https://elad.medium.com/understanding-the-initial-inherit-and-unset-css-keywords-2d70b7121695)
- [How Does CSS Work?](https://elad.medium.com/how-does-css-work-92fe7116916d)
- [The CSS Keywords That No One Really Understands (Video)](https://www.youtube.com/watch?v=nnhUBRRhKW0)

Made by [Elad Shechter (twitter)](https://twitter.com/eladsc)

