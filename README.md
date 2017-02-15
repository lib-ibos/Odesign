# 修改自 Ant Design [![](https://img.shields.io/travis/ant-design/ant-design.svg?style=flat-square)](https://travis-ci.org/ant-design/ant-design) [![npm package](https://img.shields.io/npm/v/antd.svg?style=flat-square)](https://www.npmjs.org/package/antd) [![NPM downloads](http://img.shields.io/npm/dm/antd.svg?style=flat-square)](https://npmjs.org/package/antd) [![Dependency Status](https://david-dm.org/ant-design/ant-design.svg?style=flat-square)](https://david-dm.org/ant-design/ant-design) [![Join the chat at https://gitter.im/ant-design/ant-design](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/ant-design/ant-design?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

An enterprise-class UI design language and React-based implementation.

## :loudspeaker: Document Translation Recruitment

We are now working on translate components document to English, and we need some translator and reviewer. https://github.com/ant-design/ant-design/issues/1471

## Features

- An enterprise-class design language and high quality UI.
- Graceful UI components out of the box, base on [React Component](http://react-component.github.io/badgeboard/).
- A npm + webpack + babel + dora [workflow](http://ant-tool.github.io/index.html).

## Install

```bash
npm install antd
```

## Usage

### Use prebuilt bundle

```jsx
import { DatePicker } from 'antd';
ReactDOM.render(<DatePicker />, mountNode);
```

And import style manually:

```jsx
import 'antd/dist/antd.css';  // or 'antd/dist/antd.less'
```

### Use modularized antd

- Use [babel-plugin-antd](https://github.com/ant-design/babel-plugin-antd) (Recommended)

   ```js
   // .babelrc
   {
     "plugins": [["antd", { style: "css" }]]
   }
   ```

   Then you can import components from antd directly.

   ```jsx
   // import js and css modularly, parsed by babel-plugin-antd
   import { DatePicker } from 'antd';
   ```

- Manually import

   ```jsx
   import DatePicker from 'antd/lib/date-picker';  // just for js
   ```


## Browser Support

Normal browsers and Internet Explorer 8+.

> [IE8 issues](https://github.com/xcatliu/react-ie8)

## TypeScript

tsconfig.json

```
{
  "compilerOptions": {
    "moduleResolution": "node",
    "jsx": "preserve"
  }
}
```

