# eslint-config-vazco [![Build Status](https://travis-ci.org/vazco/eslint-config-vazco.svg?branch=master)](https://travis-ci.org/vazco/eslint-config-vazco) ![Peer dependencies](https://img.shields.io/david/peer/vazco/eslint-config-vazco.svg) ![Dev dependencies](https://img.shields.io/david/dev/vazco/eslint-config-vazco.svg)

[ESLint shareable config](http://eslint.org/docs/developer-guide/shareable-configs.html) with rules used by [Vazco.eu](http://vazco.eu) in Meteor/React projects


## Install

#### For ESLint 3.x

To install simply add this config (along with ESLint and required dependencies) to your project dev-dependencies:

```
npm install --save-dev eslint
npm install --save-dev babel-eslint
npm install --save-dev eslint-config-vazco
npm install --save-dev eslint-plugin-babel
npm install --save-dev eslint-plugin-react
npm install --save-dev eslint-plugin-vazco
```

Ready to use one-liner:

```
npm i -D eslint babel-eslint eslint-config-vazco eslint-plugin-babel eslint-plugin-react eslint-plugin-vazco
```

#### For ESLint 2.x (legacy)

If you want to use this config with ESLint 2.x (required e.g. for Node 0.10) you can install previous major version:

```
npm install --save-dev eslint@2 eslint-config-vazco@1 babel-eslint@6 eslint-plugin-babel@3 eslint-plugin-react@5
```

## Usage

Extend your project ESLint rules with our config. This can be done in few ways:

#### .eslintrc / .eslintrc.json

```javascript
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
    },
    
    "scripts": {
        "eslint": "$(npm bin)/eslint --ext .js,.jsx ."
    }
}
```

## Changelog

All changes introduces in the config are tracked inside [changelog file](CHANGELOG.md).

## How to change the rules

All information regarding making changes in the config and versioning details can be found in [contributing file](CONTRIBUTING.md).

Please read them before opening a Pull Request or suggesting a change.

## Licence

MIT. Copyright (c) [Vazco.eu](http://vazco.eu).
