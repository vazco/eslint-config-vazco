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
