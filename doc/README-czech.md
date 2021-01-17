# dh-dependency-base

- [Použití v anglickém jazyce](../README.md)

Základní nastavení s balíčky a nastavením.

## Detail
Nastaví závislosti základních balíčků:
- babel = javascript compiler
- core-js = zahrnuje polyfills pro ECMAScript až 2021
- dotenv = načítá proměnné prostředí ze .env souboru do process.env
- eslint = nástroj pro identifikaci a vykazování vzorů nalezených v kódu ECMAScript / JavaScript
- chai = BDD / TDD assertion knihovna pro použití v jiném javascript testovacím frameworku
- mocha = javascript testovací framework
- prettier = formátovač kódu

Základní nastavení babel a eslint je v adresáři "./config/".

## Použití

### v souboru "./package.json" (nastavení projektu) přidejte závislost
```javascript
{
  ...
  "dependencies": {
    "dh-dependency-base": "^0.0.21"
  },
  ...
}
```

### v souboru "./babelrc" (nastavení babel)
```javascript
{
  "extends": "./node_modules/dh-dependency-base/config/.babelrc"
}
```

### v souboru "./eslintrc.json" (nastavení eslint)
```javascript
{
  "extends": "./node_modules/dh-dependency-base/config/.eslintrc.json"
}
```

## License
[MIT](https://choosealicense.com/licenses/mit/)
