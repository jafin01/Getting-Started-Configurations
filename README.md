# Next.js | ESLint | Typescript | Tailwind CSS - Getting started

## Table of contents

- [Introduction](#introduction)
- [Run](#run)
- [Technology](#technology)


## Introduction

This is a getting started template of Next.js consisting of tailwindcss, typescript and ESlint configurations.
Get started with designing without worrying about the configurations.


## Run

To run this application:

- Clone this repository
- Open the directory in terminal
- Install node modules using `npm install`
- After installing all the packages create `.eslintrc.js` file in the root directory
- Paste the following configurations in the file

```
module.exports = {
  env: {
    browser: true,
    es6: true,
    node: true,
  },
  extends: [
    'airbnb',
    'plugin:@typescript-eslint/recommended',
    'plugin:prettier/recommended',
  ],
  parser: '@typescript-eslint/parser',
  parserOptions: {
    ecmaFeatures: {
      jsx: true,
    },
    ecmaVersion: 2020,
    sourceType: 'module',
  },
  plugins: ['@typescript-eslint', 'prettier'],
  rules: {
    'prettier/prettier': ['error', { singleQuote: true }],
    'react/jsx-filename-extension': [1, { extensions: ['.tsx'] }],
    'import/prefer-default-export': 'off',
    '@typescript-eslint/no-unused-vars': ['error', { argsIgnorePattern: '^_' }],
    'no-console': 'warn',
  },
};

```

Now you can run `npm run dev` to start the application in development server.

You can run `npx eslint .` or `npm run lint` to lint the application and find errors in the terminal.
(You may not be in a situation to run this command as the errors will be highlighted in red and warnings in yellow at real time

## Technology

- ESlint
- Next.js
- Typescript
- Tailwind



 Copyright 2022 © [Jafin Jahfar](https://github.com/jafin01)
