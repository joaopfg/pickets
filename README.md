# picklefriend

[![npm version](https://img.shields.io/npm/v/picklefriend.svg?style=flat-square)](https://www.npmjs.com/package/picklefriend)
[![build](https://img.shields.io/github/workflow/status/joaopfg/picklefriend/Node.js%20CI?style=flat-square&label=build)](https://github.com/joaopfg/picklefriend/actions)
[![github](https://flat.badgen.net/badge/icon/github?icon=github&label)](https://github.com/joaopfg/picklefriend/)
[![sponsors](https://img.shields.io/github/sponsors/joaopfg?style=flat-square&color=1da1f2)](https://github.com/sponsors/joaopfg/)

Typescript package compatible with python's pickle loads/dumps

# Installation
```bash
npm i picklefriend
```

# Usage
```typescript
import { pickle } from 'picklefriend'

let myString = "my test string";
let myStringDumped = pickle.dumps(myString);
let myStringLoaded = pickle.loads(myStringDumped);

console.log(myStringLoaded);
```

# Development
### Fork the main branch, clone it and entry in the root folder
```bash
git clone git@github.com:joaopfg/picklefriend.git
cd picklefriend
```
### Install the dependencies
```bash
npm install
```
### Generate the dist folder
```bash
tsc
```
### Unit tests
The unit tests are located in the `test` folder. If you want to create new tests, they must go inside this folder and the test script must be updated in `package.json`.
```bash
npm test
```