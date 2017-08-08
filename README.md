# eslint-config-vazco [![Build Status](https://travis-ci.org/vazco/eslint-config-vazco.svg?branch=master)](https://travis-ci.org/vazco/eslint-config-vazco) ![Peer dependencies](https://img.shields.io/david/peer/vazco/eslint-config-vazco.svg) ![Dev dependencies](https://img.shields.io/david/dev/vazco/eslint-config-vazco.svg)

[ESLint shareable config](http://eslint.org/docs/developer-guide/shareable-configs.html) with rules used by [Vazco.eu](http://vazco.eu) in Meteor/React projects


## Install

#### For ESLint 4.x

To install simply add this config (along with ESLint and required dependencies) to your project dev-dependencies:

```
npm install --save-dev babel-eslint
npm install --save-dev eslint
npm install --save-dev eslint-config-prettier
npm install --save-dev eslint-config-vazco
npm install --save-dev eslint-plugin-babel
npm install --save-dev eslint-plugin-prettier
npm install --save-dev eslint-plugin-react
npm install --save-dev eslint-plugin-vazco
npm install --save-dev prettier
```

Ready to use one-liner:

```
npm i -D babel-eslint eslint eslint-config-prettier eslint-config-vazco eslint-plugin-babel eslint-plugin-prettier eslint-plugin-react eslint-plugin-vazco prettier
```

#### For previous ESLint versions

##### ESLint 2.x

If you want to use this config with ESLint 2.x (required e.g. for Node 0.10) you can install config for version 1.x:

```
npm i -D eslint@2 eslint-config-vazco@1 babel-eslint@6 eslint-plugin-babel@3 eslint-plugin-react@5
```

##### ESLint 3.x

We strongly recommend to upgrade to ESLint 4, but if you must you can use older dependencies and config from 2.x branch:

```
npm i -D eslint@3 babel-eslint@7 eslint-config-vazco@2 eslint-plugin-babel@4 eslint-plugin-react@6 eslint-plugin-vazco@1
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
