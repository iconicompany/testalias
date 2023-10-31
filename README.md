# How to have aliases with nodejs import

## example usage

`import { add } from "#libs/math.mjs"`

## setup

package.json:

```
  "imports": {
    "#libs/*": "./src/libs/*"
  },
```

## IDE compatibility

jsconfig.json
```
{
  "compilerOptions": {
    "baseUrl": "./",
    "paths": {
      "#components/*": [ "src/components/*" ],
      "#libs/*": [ "src/libs/*" ]
    }
  }
}
```

## test

Run `node src/bin/run.mjs `

## docs

https://stackoverflow.com/a/70161021