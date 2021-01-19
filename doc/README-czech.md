# dh-dependency-base

[Použití v anglickém jazyce (Readme in English)](https://github.com/hezky/dh-dependency-base/blob/master/README.md)

Základní nastavení s balíčky a nastavením.

## Detail
Nastaví závislosti základních balíčků:
* [babel](https://github.com/babel/babel) - javascript compiler
* [core-js](https://github.com/zloirock/core-js) - zahrnuje polyfills pro ECMAScript až 2021
* [dotenv](https://github.com/motdotla/dotenv) - načítá proměnné prostředí ze .env souboru do process.env
* [eslint](https://github.com/eslint/eslint) - nástroj pro identifikaci a vykazování vzorů nalezených v kódu ECMAScript / JavaScript
* [chai](https://github.com/chaijs/chai) - BDD / TDD assertion knihovna pro použití v jiném javascript testovacím frameworku
* [mocha](https://github.com/mochajs/mocha) - javascript testovací framework
* [prettier](https://github.com/prettier/prettier) - formátovač kódu

Základní nastavení babel a eslint je v adresáři "[./config/](https://github.com/hezky/dh-dependency-base/tree/master/config)".

## Použití

v souboru "[./package.json](https://github.com/hezky/dh-dependency-base/blob/master/package.json)" přidejte závislost na balíček "[dh-dependency-base](https://github.com/hezky/dh-dependency-base)"
```javascript
{
  ...
  "dependencies": {
    "dh-dependency-base": "^0.0.21"
  },
  ...
}
```

v souboru "[./babelrc](https://github.com/hezky/dh-dependency-base/blob/master/config/.babelrc)" přidejte závislost na "[dh-dependency-base](https://github.com/hezky/dh-dependency-base)" na babel
```javascript
{
  "extends": "./node_modules/dh-dependency-base/config/.babelrc"
}
```

v souboru "[./eslintrc.json](https://github.com/hezky/dh-dependency-base/blob/master/config/.eslintrc.json)" přidejte závislost na "[dh-dependency-base](https://github.com/hezky/dh-dependency-base)" na eslint
```javascript
{
  "extends": "./node_modules/dh-dependency-base/config/.eslintrc.json"
}
```

## License
[MIT](https://choosealicense.com/licenses/mit/)
