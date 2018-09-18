# Next.js + CSS + Typescript

Import `.css` files in your Next.js project with TypeScript typings

Fork from @zeit/next-css but typing with Typescript.

![https://s0.meituan.net/bs/tempfs/file/zhongguoxin/cap1.gif](https://s0.meituan.net/bs/tempfs/file/zhongguoxin/cap1.gif)

## Installation

```
npm install --save next-typed-css
```

or

```
yarn add next-typed-css
```

## Usage

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


