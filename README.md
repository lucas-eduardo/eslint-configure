# ESLint config

### Whats included?

- standard;
- react;
- react-hooks;
- jsx-a11y;
- prettier;
- eslint-plugin-import-helpers;

### Setup

1. Install the dependencies
```
npm i -D eslint @lucaseduardoio/eslint-config
```

2. Create a `.eslintrc.json` file extending the config:
```
{
  "extends": "@lucaseduardoio/eslint-config/react"
  // "extends": "@lucaseduardoio/eslint-config/node"
}
```

3. You can add/override any ESLint config by changing your own `.eslintrc.json` file. The example below will only add the self-closing tag rule and leave all the default rules untouched.
```
{
  "extends": "@lucaseduardoio/eslint-config/react",
  "rules": {
    "react/self-closing-comp": "error"
  }
}
```

> You can also use a `.eslintrc.js` instead of JSON if you prefer.

> ***Inspiration from the [rocketseat](https://github.com/Rocketseat/eslint-config-rocketseat) repository***
