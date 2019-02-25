<template>
  <div id="app">
    <router-view></router-view>
  </div>
</template>

<style lang="scss">
@import "scss/Variables.scss";
@import "scss/Typography.scss";
@import "scss/Buttons.scss";

// GLOBAL RESET
*,
*::before,
*::after {
  margin: 0;
  padding: 0;
  box-sizing: inherit;
}

html {
  box-sizing: border-box;
  font-size: 62.5%;
}

#app {
  line-height: 1.6;
  font-family: 'Source Sans Pro', sans-serif;
  color: var(--color-grey-dark);
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

@import "scss/Responsive.scss";
</style>
