
## babel 基本安裝

> npm install --save-dev @babel/core

> npm install --save-dev @babel/cli

> npm install --save-dev @babel/preset-env

> npm install --save @babel/polyfill

> npm install --save @babel/polyfill

------

## 用法
### babel.config.js
const presets = [
  [
    "@babel/env",
    {
      targets: {
        edge: "17",
        firefox: "60",
        chrome: "67",
        safari: "11.1",
      },
      "corejs": "2",
      useBuiltIns: "usage",
    },
  ],
];

module.exports = { presets };


### 執行

>  .\node_modules\.bin\babel src --out-dir dist

or

>  npx babel src --out-dir dist
-------