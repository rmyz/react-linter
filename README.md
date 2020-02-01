# Linter

## Table of contents

1. [Installation](#installation)
1. [Scripts](#scripts)
1. [Usage](#usage)

## Installation

1. Install `@rmyzdev/react-linter` package:

```sh
npm i -D @rmyzdev/react-linter
```
​
2. Add these lines to `package.json`:
​
```json
"eslintConfig": {
   "extends": ["./node_modules/@rmyzdev/react-linter/.eslintrc.js"]
 },
 "stylelint": {
   "extends": "./node_modules/@rmyzdev/react-linter/stylelint.config.js"
 },
 "prettier": "./node_modules/@rmyzdev/react-linter/.prettierrc.js"
```

## Scripts

1. Add these `scripts` to the `package.json`:
​
```json
"eslint": "./node_modules/.bin/eslint ./src",
"stylelint": "./node_modules/.bin/stylelint \"**/*.{js,jsx}\"",
"format": "npm run prettier -- --write",
"prettier": "./node_modules/.bin/prettier \"**/*.{js,jsx,css,json}\"",
```

## Usage

### Lint JS files

```sh
npm run eslint [options]
```

### Fix JS files

```sh
npm run eslint -- --fix [options]
```

### Format JS files

```sh
npm run format [options]
```

### Lint Styled-Components

```sh
npm run stylelint [options]
```

### Fix Styled-Components

```sh
npm run stylelint -- --fix [options]
```
