# 1PAW - NPM Starter

This project is an npm package starter used by @calummoore for @1productaweek.

It has the following additional features:

 * ✅ Typescript
 * ✅ Opinionated ESLint
 * ✅ Jest
 * ✅ React (optional)


### Storybook

Storybook is not included by default, but this can be easily installed with:

```sh
cd my-project-directory
npx -p @storybook/cli sb init
```

Then add these dependencies:
```sh
yarn add --dev @storybook/preset-typescript ts-loader fork-ts-checker-webpack-plugin
```

Finally, add this in the `.storybook/main.js` file that was created in the step above:

```js
module.exports = {
  addons: ['@storybook/preset-typescript'],
};
```
