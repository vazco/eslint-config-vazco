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
