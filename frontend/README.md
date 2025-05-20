When you run `git commit`, **Husky** should **auto-run** `lint-staged` which runs ESLint and Prettier on the staged files and blocks the commit if anything fails.

## Install
```bash
npm install -save-dev husky lint-staged eslint prettier
# Initialize Husky
npx husky init
```

make sure that package.json file has this:
```json
"scripts": {
  "prepare": "husky install"
}
```

then run 
```bash
npm run prepare
```


