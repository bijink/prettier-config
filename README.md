# `@bijink/prettier-config`

> Personal [Prettier](https://prettier.io) configuration

## Install

```bash
$ npm i -D @bijink/prettier-config
# or
$ pnpm add -D @bijink/prettier-config
# or
$ yarn add -D @bijink/prettier-config
```

## Usage
**Edit `package.json`** :

```json
{
  // ...
  "prettier": "@bijink/prettier-config"

  // #optional
   "scripts": {
     // ...
    "format": "prettier . --write",
    "format:check": "prettier . --check"
  },
}
```
**Or**

Create **`.prettierrc.json`** file in root directory and add
```json
"@bijink/prettier-config"
```