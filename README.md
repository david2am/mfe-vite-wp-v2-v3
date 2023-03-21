Install dependencies

```sh
cd remote && yarn install && yarn dev
```

In another terminal run:
```sh
cd host && yarn install && yarn dev
```

How was it possible?

In the `host` repository run:

```sh
yarn add @vue/compat
```

In the `vite.config.js` add alias `vue: '@vue/compat'`
```js
    resolve: {
        alias: {
            ...
            vue: '@vue/compat'
        }
    }
```