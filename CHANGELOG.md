### 7.1.0
- Updated dependencies:
  - Update ESLint to 8.25.0 by @kestarumper in ([#81](https://github.com/vazco/eslint-config-vazco/pull/81))
- New rule at error level has been added:
  - Added [no-constant-binary-expression](http://eslint.org/docs/rules/no-constant-binary-expression) ([#83](https://github.com/vazco/eslint-config-vazco/pull/83))

### 7.0.0
- Updated dependencies:
  - @typescript-eslint/eslint-plugin@5.27.0 (#80)
  - @typescript-eslint/parser@5.27.0 (#80)
  - eslint@8.16.0 (#80)
  - eslint-config-prettier@8.5.0 (#80)
  - eslint-plugin-import@2.26.0 (#80)
  - eslint-plugin-jsx-a11y@6.5.1 (#80)
  - eslint-plugin-prettier@4.0.0 (#80)
  - eslint-plugin-react@7.30.0 (#80)
  - eslint-plugin-react-hooks@4.5.0 (#80)
  - prettier@2.6.2 (#80)
  - typescript@4.7.2 (#80)
- Due to dependency updates, new rules at error level have been added:
  - [no-loss-of-precision](https://eslint.org/docs/rules/no-loss-of-precision)
  - [no-nonoctal-decimal-escape](https://eslint.org/docs/rules/no-nonoctal-decimal-escape)
  - [no-unsafe-optional-chaining](https://eslint.org/docs/rules/no-unsafe-optional-chaining)
  - [no-useless-backreference](https://eslint.org/docs/rules/no-useless-backreference)
- New rule at error level has been added: (#80)
  - [@typescript-eslint/prefer-ts-expect-error](https://github.com/typescript-eslint/typescript-eslint/blob/main/packages/eslint-plugin/docs/rules/prefer-ts-expect-error.md)

### 6.2.0
- Updated dependencies:
    - prettier@2.3.0 (#75)

- Replaced deprecated `babel-eslint` and `eslint-plugin-babel` packages with maintained ones from `@babel` monorepo. (#79)
- Fixed [@typescript-ełslint/no-unused-vars](https://github.com/typescript-eslint/typescript-eslint/blob/master/packages/eslint-plugin/docs/rules/no-unused-vars.md) rule in `typescript` configuration. (#78)
- Enabled [quotes](https://github.com/eslint/eslint/blob/master/docs/rules/quotes.md) rule to enhance prettier formatting. (#78)
- Added new plugin `eslint-plugin-eslint-comments`. New rules at error level have been added. (#77)
    - [eslint-comments/no-unused-disable](https://github.com/mysticatea/eslint-plugin-eslint-comments/blob/master/docs/rules/no-unused-disable.md)
    - [eslint-comments/disable-enable-pair](https://github.com/mysticatea/eslint-plugin-eslint-comments/blob/master/docs/rules/disable-enable-pair.md)
    - [eslint-comments/no-aggregating-enable](https://github.com/mysticatea/eslint-plugin-eslint-comments/blob/master/docs/rules/no-aggregating-enable.md)
    - [eslint-comments/no-duplicate-disable](https://github.com/mysticatea/eslint-plugin-eslint-comments/blob/master/docs/rules/no-duplicate-disable.md)
    - [eslint-comments/no-unlimited-disable](https://github.com/mysticatea/eslint-plugin-eslint-comments/blob/master/docs/rules/no-unlimited-disable.md)
    - [eslint-comments/no-unused-enable](https://github.com/mysticatea/eslint-plugin-eslint-comments/blob/master/docs/rules/no-unused-enable.md)

### 6.1.1
- Disabled rules:
    - jsx-a11y/no-onchange

- Added code example for `jsx-a11y/no-onchange` rule in the test file.

### 6.1.0
- Updated dependencies:
    - @typescript-eslint/eslint-plugin@4.12.0 (#72)
    - @typescript-eslint/parser@4.12.0 (#72)
    - babel-eslint@10.1.0 (#72)
    - eslint@7.17.0 (#72)
    - eslint-config-prettier@7.1.0 (#72)
    - eslint-plugin-babel@5.3.1 (#72)
    - eslint-plugin-import@2.22.1 (#72)
    - eslint-plugin-prettier@3.3.1 (#72)
    - eslint-plugin-react@7.22.0 (#72)
    - eslint-plugin-react-hooks@4.2.0 (#72)
    - prettier@2.2.1 (#72)
    - typescript@4.1.3 (#72)
    
- Due to dependency updates, new rules at error level have been added:
    - [typescript-eslint/restrict-template-expressions](https://github.com/typescript-eslint/typescript-eslint/blob/master/packages/eslint-plugin/docs/rules/restrict-template-expressions.md) (#72)
    - [typescript-eslint/restrict-plus-operands](https://github.com/typescript-eslint/typescript-eslint/blob/master/packages/eslint-plugin/docs/rules/restrict-plus-operands.md) (#72)
    - [typescript-eslint/no-floating-promises](https://github.com/typescript-eslint/typescript-eslint/blob/master/packages/eslint-plugin/docs/rules/no-floating-promises.md) (#72)
    - [typescript-eslint/no-implied-eval](https://github.com/typescript-eslint/typescript-eslint/blob/master/packages/eslint-plugin/docs/rules/no-implied-eval.md) (#72)
    - [typescript-eslint/no-unsafe-assignment](https://github.com/typescript-eslint/typescript-eslint/blob/master/packages/eslint-plugin/docs/rules/no-unsafe-assignment.md) (#72)
    - [typescript-eslint/no-unsafe-call](https://github.com/typescript-eslint/typescript-eslint/blob/master/packages/eslint-plugin/docs/rules/no-unsafe-call.md) (#72)
    - [typescript-eslint/no-unsafe-member-access](https://github.com/typescript-eslint/typescript-eslint/blob/master/packages/eslint-plugin/docs/rules/no-unsafe-member-access.md) (#72)
    - [typescript-eslint/no-unsafe-return](https://github.com/typescript-eslint/typescript-eslint/blob/master/packages/eslint-plugin/docs/rules/no-unsafe-return.md) (#72)
    
- Removed unnecessary peer dependencies:
    - eslint-plugin-vazco (#72)

### 6.0.0

- Extended rules with `react/jsx-curly-brace-presence` (#70)

- Updated dependencies:
    - eslint@7.15.0 (#71)

### 5.4.0

- Extended rules with `plugin:jsx-a11y/recommended` (#69)

- Added new dependencies:
    - eslint-plugin-jsx-a11y@6.4.1 (#69)

### 5.3.1

- Removed `vazco/no-console` rule (#68)

### 5.3.0

- Made TypeScript config extend the default one (#64)
- Changed `prettier.trailingComma` from `none` to `all` (#66)
- Added new rules:
    - `import/order` rule (#65)
    - `react-hooks/rules-of-hooks` rule (#67)
    - `react-hooks/rules-of-hooks` rule (#67)

### 5.2.0

- Added new rules:
    - `curly` rule (#62)

- Updated dependencies:
    - prettier@2.0.2

### 5.1.0

- Added new TypeScript config
- Reverted dependencies type change made in 5.0.0
- Bump dependencies

### 5.0.0

- Changed dependencies type from `peerDependencies` to `dependencies` to simplify the installation and configuration process.

### 4.3.0

- Added new rules:
    - `no-duplicate-imports` rule (#47)
    - `react/no-access-state-in-setstate` rule (#48)
    - `sort-comp` rule (#49)
    - `no-this-in-sfc` rule (#50)


### 4.2.0

- Added new rules:
    - Enforce `eqeqeq` rule (#42)

- Updated dependencies:
    - eslint-config-prettier@4.1.0

### 4.1.0

- Changed indentation to 2 spaces (#39)
    - Affected `indent`, `max-len` and `prettier/prettier`

### 4.0.0

Major version bump due to ESLint major update.

- Updated dependencies:
    - babel-eslint@8.2.6
    - eslint@5.3.0
    - eslint-config-prettier@3.0.1
    - eslint-plugin-babel@5.1.0
    - eslint-plugin-prettier@2.6.2
    - eslint-plugin-react@7.11.0
    - prettier@1.14.2

### 3.1.1

- Updated dependencies:
    - babel-eslint@8.2.1
    - eslint@4.15.0
    - eslint-config-prettier@2.9.0
    - eslint-plugin-prettier@2.4.0
    - eslint-plugin-react@7.5.1
    - prettier@1.10.1

### 3.1.0

- Updated dependencies:
    - eslint@4.7.2
    - babel-eslint@8.0.0
    - eslint-plugin-babel@4.1.2
    - eslint-plugin-react@7.4.0

- New config: `vazco/prettier`

- New optional dependencies (for `prettier`):
    - eslint-config-prettier@2.6.0
    - eslint-plugin-prettier@2.3.1

### 3.0.0

- Updated dependencies:
    - eslint@4.1.1
    - babel-eslint@7.2.3
    - eslint-plugin-react@7.1.0
    - yamljs@0.3.0

- Rules adjusted to new ESLint release

### 2.5.0

- Removed dependency:
    - eslint-plugin-brackets

- Removed rules:
    - brackets/* (#30)

- Updated dependencies:
    - eslint@3.19.0
    - babel-eslint@7.2.2
    - yamljs@0.2.9

### 2.4.1

- Relaxed rules:
    - use brackets/object-curly-newline instead of object-curly-newline (#29)

- Updated dependencies:
    - eslint@3.18.0
    - babel-eslint@7.2.1
    - eslint-plugin-react@6.10.3

### 2.4.0

- Added new errors:
    - array-bracket-newline (#24)
    - object-curly-newline (#25)
    - conditional-parens-newline (#26)
    - call-parens-newline (#27)
    - func-parens-newline (#28)

- Added new dependency:
    - eslint-plugin-brackets@0.0.1

- Updated dependencies:
    - eslint@3.17.1
    - eslint-plugin-babel@4.1.1

- Other:
    - Docs update
    - Update contributing rules
    - New PR template

### 2.3.0

- Added new errors:
    - comma-dangle (#21)
    - space-infix-ops (#22)
    - space-unary-ops (#23)

- Updated dependencies:
    - eslint@3.16.1
    - eslint-plugin-babel@4.0.1
    - eslint-plugin-react@6.10.0

### 2.2.1

- Updated dependencies:
    - babel-eslint@7.1.1
    - eslint@3.13.0
    - eslint-plugin-babel@4.0.0
    - eslint-plugin-react@6.9.0

### 2.2.0

- Added new errors:
    - no-var (#13)
    - prefer-const (#14)
    - object-shorthand (#15)
    - arrow-parens (#16)
    - no-unneeded-ternary (#17)

- Added new warnings:
    - consistent-return (#18)

- Updated dependencies:
    - eslint@3.9.1
    - eslint-plugin-react@6.5.0
    - babel-eslint@7.1.0

### 2.1.0

- Added new required peer dependency: [eslint-plugin-vazco](https://www.npmjs.com/package/eslint-plugin-vazco).

    You can install it in your project with `npm i -D eslint-plugin-vazco`

- Changes to `no-console` rule, `info`, `time` and `timeEnd` will now be a warning.

### 2.0.1

- Relax `no-console` rule, allow `info` (#9), `time` and `timeEnd` (#10)

### 2.0.0

- Switch to ESLint 3.x

### 1.3.0

- Added `no-console` rule (#7)

### 1.2.0

- Stricter jsx related rules (#6)
    - jsx-closing-bracket-location
    - jsx-curly-spacing
    - jsx-equals-spacing
    - jsx-first-prop-new-line
    - jsx-indent-props
    - jsx-key
    - jsx-no-comment-textnodes
    - jsx-no-duplicate-props
    - jsx-space-before-closing

### 1.1.2

- Move configs to `configs` directory
- Integration with Travis CI

### 1.1.1

- Fix for `eol-last` rule
- Added empty file test to verify if config is correct

### 1.1.0

- Added `eol-last` rule
- Added `no-trailing-spaces` rule

### 1.0.0

- Initial release
