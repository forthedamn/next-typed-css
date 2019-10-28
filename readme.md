# Next.js + CSS or Sass + Typescript

### next-typed-css@latest Support next.js 7 & 8

> next.js 6 plz use next-typed-css@0.2.1 *

Import `.css(.scss)` files in your Next.js project with TypeScript typings

Fork from @zeit/next-css and @zeit/next-sass but typing with Typescript.

![https://s0.meituan.net/bs/tempfs/file/zhongguoxin/cap1.gif](https://s0.meituan.net/bs/tempfs/file/zhongguoxin/cap1.gif)

## Installation

```
npm install --save next-typed-css
```

or

```
yarn add next-typed-css
```

## Usage with CSS

Most config same as [@zeit/next-css](https://github.com/zeit/next-plugins/tree/master/packages/next-css)


## Difference

### Use typings CSS with Typescript

Typing css based on [typings-for-css-modules-loader](https://github.com/Jimdo/typings-for-css-modules-loader)

```
// next.config.js
const withCSS = require('next-typed-css')
module.exports = withCSS({
  // no need to set 'cssModule: true' again
  tsCssModules: true
  cssLoaderOptions: {
    // typings-for-css-modules-loader config here
    namedExport: true
  }
})
```

## Usage with Sass

Most config same as [@zeit/next-sass](https://github.com/zeit/next-plugins/tree/master/packages/next-sass)


## Difference

### Use typings Sass with Typescript

```
// next.config.js
const withSass = require('next-typed-css/sass')
module.exports = withSass({
  // no need to set 'cssModule: true' again
  tsCssModules: true
  cssLoaderOptions: {
    // typings-for-css-modules-loader config here
    namedExport: true
  }
})
```


