<h1 align="center">
    <a href="https://github.com/vazco">vazco</a>/eslint-config-vazco
</h1>

<p align="center">
    <a href="https://travis-ci.org/vazco/eslint-config-vazco">
        <img src="https://travis-ci.org/vazco/eslint-config-vazco.svg?branch=master" alt="Build Status">
    </a>
    <a href="https://greenkeeper.io/">
        <img src="https://badges.greenkeeper.io/vazco/eslint-config-vazco.svg" alt="Greenkeeper badge">
    </a>
    <img src="https://img.shields.io/david/peer/vazco/eslint-config-vazco.svg" alt="peerDependencies">
    <img src="https://img.shields.io/david/dev/vazco/eslint-config-vazco.svg" alt="devDependencies">
    <a href="https://vazco.eu">
        <img src="https://img.shields.io/badge/vazco-package-blue.svg?logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAYAAAAfSC3RAAAABmJLR0QA%2FwD%2FAP%2BgvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH4QMfFAIRHb8WQgAAAY1JREFUKM%2BNkLFrGgEUxr87FMnpnXdIqxi1Q3VxachgSbcOgRBCTMbgH9CCW%2BjSUminSpEmBEIpHW7rkCmQSSjEKVOGEAK5bOFyk4c5TMRTyZ1fl5aK9ai%2F8b334%2Ft4QBBmLQmz9jpoLSKYPQCfYdaezi6atTKAMoAYgK1pJ8LkQPr5JspHsbO%2BFilAEADQArCA3Ftn%2FC40KebPO4Ln37peNNxrFxPSXTaW9cPiewDbgYkkXwBYB3B5dHES3W8cpM254ctOJhr3wsKqs7Zj%2FdOZZITkMf9yT%2FKq3e18eHf47fmTT5XE1H%2BQ3GAwDyQ%2FkkxMSvLvhP%2FxZVLc42zYJBf%2FSPMkW57nsd%2Fv03VdDgYDjkajIPkryVDIdd1Xtm0%2Fdhznptvtmr7vu5IkRRRFySiKko%2FH45BlebzgJoBdodls%2FjAM49SyrIau69etVmsIIFStVnPFYvFZoVBY1jRtJZlMpjRNm5MkCaIofhfq9XrMMIyeruuc9u1KpRIulUqqqqpLqqqW0%2Bl0OZVKyb8ANqUwunhV3dcAAAAASUVORK5CYII%3D&style=flat-square">
    </a>
</p>


## Install

#### For ESLint 5.x

To install simply add this config (along with ESLint and required dependencies) to your project dev-dependencies:

```
npm install --save-dev babel-eslint
npm install --save-dev eslint
npm install --save-dev eslint-config-vazco
npm install --save-dev eslint-plugin-babel
npm install --save-dev eslint-plugin-react
npm install --save-dev eslint-plugin-vazco

# If you want to use prettier
npm install --save-dev prettier
npm install --save-dev eslint-plugin-prettier
npm install --save-dev eslint-config-prettier
```

Ready to use one-liner (for `default` config):

```
npm i -D babel-eslint eslint eslint-config-vazco eslint-plugin-babel eslint-plugin-react eslint-plugin-vazco
```

Ready to use two-liner (for `prettier` config), requires npm 5+:

```
npm i -D eslint-config-vazco
npx install-peerdeps --dev eslint-config-vazco
```

<details>
<summary><strong>Previous ESLint versions</strong></summary>

#### For ESLint 4.x
We recommend to upgrade to ESLint 5, but if you must you can use older dependencies and config from 3.x branch:

To install simply add this config (along with ESLint and required dependencies) to your project dev-dependencies:

Ready to use one-liner (for `default` config):

```
npm i -D babel-eslint eslint eslint-config-vazco@3 eslint-plugin-babel eslint-plugin-react eslint-plugin-vazco
```

Ready to use two-liner (for `prettier` config), requires npm 5+:

```
npm i -D eslint-config-vazco@3
npx install-peerdeps --dev eslint-config-vazco@3
```

##### ESLint 3.x
We strongly recommend to upgrade to ESLint 5, but if you must you can use older dependencies and config from 2.x branch:

```
npm i -D eslint@3 babel-eslint@7 eslint-config-vazco@2 eslint-plugin-babel@4 eslint-plugin-react@6 eslint-plugin-vazco@1
```

##### ESLint 2.x
If you want to use this config with ESLint 2.x (required e.g. for Node 0.10) you can install config for version 1.x:

```
npm i -D eslint@2 eslint-config-vazco@1 babel-eslint@6 eslint-plugin-babel@3 eslint-plugin-react@5
```

</details>

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

### Alternative config - `vazco/prettier`

[Prettier](https://prettier.io) is an opinionated code formatter: it removes all styling and enforces outputted code to use a consistent style.

Usage is the same as in examples above, just replace `"extends": "vazco"` with `"extends": "vazco/prettier"`.

```json
{
    "extends": "vazco/prettier"
}
```

This config is more strict, and using `eslint --fix` **will completely reformat your code** using prettier.

#### Prettier workflow

Introducing prettier to project can be problematic.
To avoid merge conflicts, all active branches should reformat code at the same time.

Later on code could be `--fix`ed on every commit, with tools like [lint-staged](https://github.com/okonet/lint-staged) and [pre-commit](https://github.com/observing/pre-commit) or [husky](https://github.com/typicode/husky)

## Changelog

All changes introduces in the config are tracked inside [changelog file](CHANGELOG.md).

## How to change the rules

All information regarding making changes in the config and versioning details can be found in [contributing file](CONTRIBUTING.md).

Please read them before opening a Pull Request or suggesting a change.

## License

<img src="https://vazco.eu/banner.png" align="right">

**Like every package maintained by [Vazco](https://vazco.eu/), eslint-config-vazco is [MIT licensed](https://github.com/vazco/uniforms/blob/master/LICENSE).**
