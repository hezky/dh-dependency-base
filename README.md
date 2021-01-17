# dh-dependency-base

- [Readme in Czech](doc/README-czech.md)

Basic settings with packages and settings.

## Detail
Sets basic dependencies packages:
- babel = javascript compiler
- core-js = includes polyfills for ECMAScript up to 2021
- dotenv = loads environment variables from .env file
- eslint = an AST-based pattern checker for JavaScript
- chai = BDD/TDD assertion library for node.js and the browser. Test framework agnostic
- mocha = simple, flexible, fun test framework
- prettier = is an opinionated code formatter

The basic settings for babel and eslint are in the folder "./config/" directory.

## Usage

### in file "./package.json" (settings projekt) add dependency
```javascript
{
  ...
  "dependencies": {
    "dh-dependency-base": "^0.0.21"
  },
  ...
}
```

### in file "./babelrc" (settings babel)
```javascript
{
  "extends": "./node_modules/dh-dependency-base/config/.babelrc"
}
```

### in file "./eslintrc.json" (settings eslint)
```javascript
{
  "extends": "./node_modules/dh-dependency-base/config/.eslintrc.json"
}
```

## License
[MIT](https://choosealicense.com/licenses/mit/)
