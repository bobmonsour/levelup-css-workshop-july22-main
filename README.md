# Based on Level-Up With Modern CSS Workshop

> Presented by Stephanie Eckles - [@5t3ph](https://twitter.com/5t3ph) - author of [ModernCSS.dev](https://moderncss.dev), [SmolCSS.dev](https://smolcss.dev), and [StyleStage.dev](https://stylestage.dev)
> This is a modified version of the Day 3 repo from the workshop. Modified by @bobmonsour.

## Goal of the modifications

1. Integrate the Open Props CSS custom properties framework
2. Do #1 on build using the postcss-jit-props plugin (just in time props). Note that this does not work for local development, only for production.
3. Maintain use of cssnano, autoprefixer, and postcss-logical plugins.

Note: To use Open Props in development, ideally, one would have access to all of the available properties. I have used Open Props on my personal website and had to use environment variables and separate main css file (one that imports all the open props for local dev work, and a second that does not, yet relies on the postcss-jit-props plugin to do the work of injecting only the props actually references in the resulting css file...which in our case is generated using sass).

## Development Scripts

**`npm start`**

> Run 11ty with hot reload at localhost:8080, including reload based on Sass changes

Note again: 'npm start' can be made to work, but I don't have time for that just now...an example can be found on [the repo of my personal site](https://github.com/bobmonsour/bobmonsour.com).

**`npm run build`**

> Production build includes minified, autoprefixed CSS and site pages ready to deploy on an external host.

This repo has been [deployed to Netlify](https://levelup-css-day3.netlify.app/).
