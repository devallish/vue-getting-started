 # Vuejs getting started
A short step by step guide to getting a basic vue project up and running.

It includes the use of vuex, vue-resource, uikit and sass.

## Pre-requisites
1. Install node & npm
2. Install vue-cli *npm install vue-cli -g*

## Install Steps
1. Run *vue install webpack vue-getting-started* enter values as you wish or just accept defaults.
2. Run *cd vue-getting-started*
3. Run *npm install* wait for dependencies to be installed.
4. Run *npm install babel-preset-env --save-dev*
5. Run *npm install sass-loader node-sass --save-dev*
6. Run *npm install uikit jquery --save*
7. Run *npm run dev*. This should launch default app on http://localhost:8080.

## Steps to use uikit.
This project uses the .vue template style as *lang=sass scoped*. 
Include general style settings and pulling in of uikit sass in app.vue.
1. Change the style section of the App.vue to:
```scss
<style lang="scss">
  body {
    background-color: lightblue;
  }
</style>
```
2. Change the style tag in the Hello.vue to:
```scss
<style lang="scss" scoped>
```
3. Add below the existing import statements the following to main.js
```js
import 'jquery'
import 'uikit'
```
3. Change the App.vue file with the following:
```html
<template>
  <section class="uk-section">
    <div class="uk-container">
      <img src="./assets/logo.png">
      <router-view></router-view>
    </div>
  </section>
</template>
```
```css
<style lang="scss">
  @import '../node_modules/uikit/src/scss/variables-theme.scss';
  @import '../node_modules/uikit/src/scss/mixins-theme.scss';
  // Add overrides here...
  @import '../node_modules/uikit/src/scss/uikit-theme.scss';

  body {
    background-color: lightblue;
  }
</style>
```
4. Run the *npm run dev* and you should see the changes.
