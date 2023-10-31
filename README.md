# How to have aliases with nodejs import

## example usage

`import { add } from '#libs/math';`

## setup

package.json:

```
  "imports": {
    "#libs/*": "./src/libs/*.mjs"
  },
```

## test

Run `node src/bin/run.mjs `

## docs

https://stackoverflow.com/a/70161021