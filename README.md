# `@bijink/prettier-config`

> Personal [Prettier](https://prettier.io) configuration

## Install
```bash
$ npm i -D prettier @bijink/prettier-config
# or
$ pnpm add -D prettier @bijink/prettier-config
# or
$ yarn add -D prettier @bijink/prettier-config
```

## Usage
Edit **`package.json`**:
```js
{
  // ...
  "prettier": "@bijink/prettier-config"
}
```
##### Or
Create **`.prettierrc.json`** file in the root directory and add: 
```json
"@bijink/prettier-config"
```
##### Or
To extend the configuration to overwrite the properties from **@bijink/prettier-config** configuration. Create **`.prettierrc.js`** file in the root directory. Then import the configuration and export the modifications, e.g:
```js
import prettierConfig from "@bijink/prettier-config";

export default {
  ...prettierConfig,
  semi: false,
};
```

### Optional
To add scripts for prettier commands, edit **`package.json`**:
```js
{
   "scripts": {
     // ...
    "format": "prettier . --write",
    "format:check": "prettier . --check"
  },
}
```

*To know more about Prettier **configuration sharing**, [click](https://prettier.io/docs/en/configuration#sharing-configurations).*