# Prerequirement
- vscode
- node
    - by nvm: https://github.com/nvm-sh/nvm
- postman
    - See: https://www.postman.com/
- bash
    - Linux/Mac: zsh, See: https://www.zsh.org/
    - Windows: Git Bash



# Try the example
## 1. See https://expressjs.com/en/starter/hello-world.html
```javascript
const express = require('express')
const app = express()
const port = 3000

app.get('/', (req, res) => res.send('Hello World!'))

app.listen(port, () => console.log(`Example app listening on port ${port}!`))
```
## 2. Write test file

Add a scirpt in the `package.json`:
```
  "scripts": {
    "start": "nodemon ./src/app.js",
    "tdd": "mocha ./test/app-spec.js",
    "test": "echo \"Error: no test specified\" && exit 1"
  }
```
Then run the following command in shell:
```shell
npm run tdd
```
This is TDD.
```shell
npm run start
```
This is app.



## 3. Task

# What do we want to do


- Create
    - **POST** /todo
- Read
    - **GET** /todo/:id/
    - **GET** /todo
- Delete
    - **DELETE** /todo/:id

# TDD
- Tasking
- Create Tests and run them
- Implement the source code
- Refactor the code.
