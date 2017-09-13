
# vue-getting-started
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
1. Change the style section of the App.vue to.
```scss
<style lang="scss">
  body {
    background-color: lightblue;
  }
</style>
```
