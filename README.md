# Based on Level-Up With Modern CSS Workshop

> Presented by Stephanie Eckles - [@5t3ph](https://twitter.com/5t3ph) - author of [ModernCSS.dev](https://moderncss.dev), [SmolCSS.dev](https://smolcss.dev), and [StyleStage.dev](https://stylestage.dev)
> This is a modified version of the Day 3 repo from the workshop. Modified by @bobmonsour.

## Goal of the modifications to Stephanie's base repo

1. Integrate the Open Props CSS custom properties framework
2. Do #1 using postcss on production builds to use only the properties referenced in the CSS generated by sass
3. Maintain use of cssnano, autoprefixer, and postcss-logical plugins.

## Development Scripts

**`npm start`**

> Run 11ty with hot reload at localhost:8080, including reload based on Sass changes

**`npm run build`**

> Production build includes minified, autoprefixed CSS and site pages ready to deploy on an external host.

This repo has been [deployed to Netlify](https://levelup-css-day3.netlify.app/).
