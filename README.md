# Sample Typescript & Jest Setup

This project is a starter template for Typescript & Jest. Follow the instructions to setup in any other Typescript project

## Initial Setup

- `$ git init` (Initialize git repo. This will help with **watch** command of jest)
- Add _.gitignore_ file
- Add _node_modules_ folder to _.gitignore_
- Make sure typescript installed for project

```shell
$ yarn add --dev typescript
or
$ npm install --save-dev typescript
```

- Make sure you have a **src** folder for your code (can be any folder but using **src** as convention)

## Install Testing modules

Install the jest modules required for testing

```shell
$ yarn add jest @types/jest ts-jest --dev
or
$ npm install jest @types/jest ts-jest --save-dev
```

## Configure Jest

- Add a jest.config.js file to the root of your project
- Add the below config to the _jest.config.js_

```json
(module.exports = {
  "roots": ["<rootDir>/src"],
  "transform": {
    "^.+\\.tsx?$": "ts-jest"
  }
})
```

- Add test command to _package.json_

```json
{
  "test": "jest"
}
```

## Running Tests

- You can run tests by executing the command `yarn test` or `npm t`
- You can also run test in watch mode by `yarn test --watch` or `npm t --watch`
- Another option to run test is using `npx jest --watch`. This will run tests in **watch** mode

## Folder Structure

```text
|--- .git/
|--- .gitignore
|--- jest.config.js
|--- node_modules/
|--- package.json
|--- README.md
|--- src
|    |--- basic.test.ts
|    |--- basic.ts
|--- yarn.lock
```
