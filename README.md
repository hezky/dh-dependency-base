# dh-dependency-base

[Readme in Czech (Readme v Češtině)](https://github.com/hezky/dh-dependency-base/blob/master/doc/README-czech.md)

Basic settings with packages and settings.

## Detail
Sets basic dependencies packages:
* [babel](https://github.com/babel/babel) - javascript compiler
* [core-js](https://github.com/zloirock/core-js) - includes polyfills for ECMAScript up to 2021
* [dotenv](https://github.com/motdotla/dotenv) - loads environment variables from .env file
* [eslint](https://github.com/eslint/eslint) - an AST-based pattern checker for JavaScript
* [chai](https://github.com/chaijs/chai) - BDD/TDD assertion library for node.js and the browser. Test framework agnostic
* [mocha](https://github.com/mochajs/mocha) - simple, flexible, fun test framework
* [prettier](https://github.com/prettier/prettier) - is an opinionated code formatter

The basic settings for babel and eslint are in the folder "./config/" directory.

## Usage

in file "[./package.json](https://github.com/hezky/dh-dependency-base/blob/master/package.json)" add a dependency on the "[dh-dependency-base](https://github.com/hezky/dh-dependency-base)" package
```javascript
{
  ...
  "dependencies": {
    "dh-dependency-base": "^0.0.21"
  },
  ...
}
```

in file "[./babelrc](https://github.com/hezky/dh-dependency-base/blob/master/config/.babelrc)" add a dependency on the "[dh-dependency-base](https://github.com/hezky/dh-dependency-base)" to babel
```javascript
{
  "extends": "./node_modules/dh-dependency-base/config/.babelrc"
}
```

in file "[./eslintrc.json](https://github.com/hezky/dh-dependency-base/blob/master/config/.eslintrc.json)" add a dependency on the "[dh-dependency-base](https://github.com/hezky/dh-dependency-base)" to eslint
```javascript
{
  "extends": "./node_modules/dh-dependency-base/config/.eslintrc.json"
}
```

## License
[MIT](https://choosealicense.com/licenses/mit/)
