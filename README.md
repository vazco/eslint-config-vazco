<h1 align="center">
    <a href="https://github.com/vazco">vazco</a>/eslint-config-vazco
</h1>

<p align="center">
    <a href="https://travis-ci.org/vazco/eslint-config-vazco">
        <img src="https://travis-ci.org/vazco/eslint-config-vazco.svg?branch=master" alt="Build Status">
    </a>
    <img src="https://img.shields.io/david/peer/vazco/eslint-config-vazco.svg" alt="peerDependencies">
    <img src="https://img.shields.io/david/dev/vazco/eslint-config-vazco.svg" alt="devDependencies">
    <a href="https://vazco.eu">
        <img src="https://img.shields.io/badge/vazco-package-blue.svg?logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAYAAAAfSC3RAAAABmJLR0QA%2FwD%2FAP%2BgvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH4QMfFAIRHb8WQgAAAY1JREFUKM%2BNkLFrGgEUxr87FMnpnXdIqxi1Q3VxachgSbcOgRBCTMbgH9CCW%2BjSUminSpEmBEIpHW7rkCmQSSjEKVOGEAK5bOFyk4c5TMRTyZ1fl5aK9ai%2F8b334%2Ft4QBBmLQmz9jpoLSKYPQCfYdaezi6atTKAMoAYgK1pJ8LkQPr5JspHsbO%2BFilAEADQArCA3Ftn%2FC40KebPO4Ln37peNNxrFxPSXTaW9cPiewDbgYkkXwBYB3B5dHES3W8cpM254ctOJhr3wsKqs7Zj%2FdOZZITkMf9yT%2FKq3e18eHf47fmTT5XE1H%2BQ3GAwDyQ%2FkkxMSvLvhP%2FxZVLc42zYJBf%2FSPMkW57nsd%2Fv03VdDgYDjkajIPkryVDIdd1Xtm0%2Fdhznptvtmr7vu5IkRRRFySiKko%2FH45BlebzgJoBdodls%2FjAM49SyrIau69etVmsIIFStVnPFYvFZoVBY1jRtJZlMpjRNm5MkCaIofhfq9XrMMIyeruuc9u1KpRIulUqqqqpLqqqW0%2Bl0OZVKyb8ANqUwunhV3dcAAAAASUVORK5CYII%3D&style=flat-square">
    </a>
</p>


## Install

To install simply add this config (along with it's peer dependencies) to your project's dev-dependencies:

```
npm install --save-dev eslint-config-vazco
npx install-peerdeps --dev eslint-config-vazco
```

## Usage

Extend your project's ESLint rules with our config.
This can be done in few ways (for TypeScript projects replace `vazco` with `vazco/typescript`):

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
