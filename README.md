# Mint UI

[![Build Status](https://travis-ci.org/ElemeFE/mint-ui.svg?branch=master)](https://travis-ci.org/ElemeFE/mint-ui)
[![npm](https://img.shields.io/npm/v/mint-ui.svg?maxAge=3600)](https://www.npmjs.com/package/mint-ui)
[![NPM downloads](http://img.shields.io/npm/dm/mint-ui.svg)](https://npmjs.org/package/mint-ui)
![JS gzip size](http://img.badgesize.io/elemefe/mint-ui/master/lib/index.js.svg?compression=gzip&label=gzip%20size:%20JS)
![CSS gzip size](http://img.badgesize.io/elemefe/mint-ui/master/lib/style.css.svg?compression=gzip&label=gzip%20size:%20CSS)
[![Join the chat at https://gitter.im/ElemeFE/mint-ui](https://badges.gitter.im/ElemeFE/mint-ui.svg)](https://gitter.im/ElemeFE/mint-ui?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

> Mobile UI elements for **Vue 2.0**

- [Homepage](http://mint-ui.github.io)
- [Documentation](http://mint-ui.github.io/docs)

## Installation
```shell
npm i mint-ui -S

# for Vue 1.x
npm i mint-ui@1 -S
```

## Usage

Import all components.

```javascript
import Vue from 'vue';
import Mint from 'mint-ui';
import 'mint-ui/lib/style.css';

Vue.use(Mint);
```

Or import specified component. (Use [babel-plugin-component](https://www.npmjs.com/package/babel-plugin-component))

```javascript
import { Cell, Checklist } from 'mint-ui';

Vue.component(Cell.name, Cell);
Vue.component(Checklist.name, Checklist);
```


Equals to

```javascript
import Vue from 'vue';
import Mint from 'mint-ui';
import 'mint-ui/lib/style.css';

Vue.use(Mint);

// import specified component

import MtRadio from 'mint-ui/lib/radio';
import 'mint-ui/lib/radio/style.css';

Vue.component(MtRadio.name, MtRadio);
```

## babel-plugin-component
- Auto import css file
- Modular import component

Installation
```shell
npm i babel-plugin-component -D
```

Usage

.babelrc
```json
{
  "plugins": ["other-plugin", ["component", [
    { "libraryName": "mint-ui", "style": true }
  ]]]
}
```

## CDN
RawGit

- https://cdn.rawgit.com/ElemeFE/mint-ui/master/lib/index.js
- https://cdn.rawgit.com/ElemeFE/mint-ui/master/lib/style.css

NPMCDN

- https://unpkg.com/mint-ui/lib/index.js
- https://unpkg.com/mint-ui/lib/style.css

## Development

```shell
npm run dev
```

## Contribution
Please make sure to read the [Contributing Guide](https://github.com/ElemeFE/mint-ui/blob/master/.github/CONTRIBUTING_en-us.md) before making a pull request.

## License
MIT

# Tech Stack List
## Libraries:

- "lodash.merge": "^4.4.0",
- "lodash.unescape": "^4.0.0",
"react": "~15.3.1",
"react-native": "^0.34.1",
"react-native-html-render": "^1.0.4",
"react-native-scrollable-tab-view": "^0.5.3",
"react-native-svg": "^4.3.1",
"react-redux": "^4.4.0",
"react-static-container": "^1.0.1",
"redux": "^3.3.1",
"redux-api-middleware": "chunghe/RN-redux-api-middleware#master",
"redux-thunk": "^2.0.1",
"victory-chart-native": "^1.0.0"
"babel-eslint": "^6.1.0",
"eslint": "^2.13.1",
"eslint-config-airbnb": "^9.0.1",
"eslint-plugin-import": "^1.9.2",
"eslint-plugin-jsx-a11y": "^1.5.3",
"eslint-plugin-react": "^5.2.2",
"lint-staged": "^1.0.1",
"pre-commit": "^1.1.3",
"remote-redux-devtools": "^0.4.9",
"remote-redux-devtools-on-debugger": "^0.6.2",
"rnpm-plugin-upgrade": "^0.26.0"

##IDE: 

Visual Studio Code: v1.20.0
XCode: 9.2(9c40b)
Android Studio: 3.0

##SDK: 

"react-native-material-design": "^0.3.7"
https://github.com/react-native-material-design/react-native-material-design
