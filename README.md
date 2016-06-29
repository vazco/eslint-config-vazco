# eslint-config-vazco [![Build Status](https://travis-ci.org/vazco/eslint-config-vazco.svg?branch=master)](https://travis-ci.org/vazco/eslint-config-vazco)

[ESLint shareable config](http://eslint.org/docs/developer-guide/shareable-configs.html) with rules used by [Vazco.eu](http://vazco.eu) in Meteor/React projects


## Install

```
$ npm install --save-dev eslint eslint-config-vazco babel-eslint eslint-plugin-babel eslint-plugin-react
```


## Usage

Extend your project ESLint rules with our config. This can be done in few ways:

#### .eslintrc / .eslintrc.json

```json
{
    "extends": "vazco",
    "rules": {
        // custom project rules
    }
}
```

#### .eslintrc.yaml

```yaml
extends:
  - vazco

rules:
  // custom project rules
```

#### package.json

```json
{
    "eslintConfig": {
        "extends": "vazco"
    }
}
```

## Modifying the config

All information regarding making changes in the config and versioning details can be found in [contributing](CONTRIBUTING.md) file.

Please read them before opening a Pull Request or suggesting a change.

## Licence

MIT. Copyright (c) [Vazco.eu](http://vazco.eu).
