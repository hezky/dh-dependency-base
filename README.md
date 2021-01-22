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

Install the ** dh-dependency-base ** package in your project.
In the project directory, run the command:
```javascript
$ npm install --save dh-dependency-base
```

in file settings "[./babelrc](https://github.com/hezky/dh-dependency-base/blob/master/config/.babelrc)" add a dependency on the package "[dh-dependency-base](https://github.com/hezky/dh-dependency-base)"
```javascript
{
  "extends": "./node_modules/dh-dependency-base/config/.babelrc"
}
```

in file settings "[./eslintrc.json](https://github.com/hezky/dh-dependency-base/blob/master/config/.eslintrc.json)" add a dependency on the package "[dh-dependency-base](https://github.com/hezky/dh-dependency-base)"
```javascript
{
  "extends": "./node_modules/dh-dependency-base/config/.eslintrc.json"
}
```

## License
[MIT](https://choosealicense.com/licenses/mit/)
