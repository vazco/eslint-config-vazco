# eslint-config-vazco

[ESLint shareable config](http://eslint.org/docs/developer-guide/shareable-configs.html) with rules used by [Vazco.eu](http://vazco.eu) in Meteor/React projects


## Install

```
$ npm install --save-dev eslint eslint-config-vazco babel-eslint eslint-plugin-babel eslint-plugin-react
```


## Usage

Extend your project ESLint rules with our config.

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

## Adding new config sets

At the moment there is only one, `default` config.

There could be new configs added in the future by just adding new yaml files.

E.g. create `example.yaml` (potentially based on `default.yaml`) file in main directory and once published it could be imported in other projects:

```json
{
    "extends": "vazco/example"
}
```
