<template>
  <div id="app">
    <router-view></router-view>
  </div>
</template>

<style lang="scss">
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
  color: #2A2A2B;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

// TYPOGRAPHY
p {
  font-family: 'lato', sans-serif;
  line-height: 1.8;
  font-size: 1.5rem;
  letter-spacing: 1px;
}

.subtitle {
  padding: 1rem 3rem;
  font-size: 3.5rem;
  width: max-content;

  &__white {
    color: #50465E;
    background-color: white;
    box-shadow: 0 3px 10px rgba(0,0,10px,.2);
  }
  &__purple {
    color: white;
    background-color: #50465E;
  }
}

.title {
  &__xs {
    font-size: 2rem;
    line-height: 1.2;
  }
}

.text {
  &__min {
    text-transform: uppercase;
    font-family: 'Source Sans Pro', sans-serif;
    color: #797979;
    font-size: 1.3rem;
  }
}

//BUTTONS
.button__sm,
.button__sm:visited  {
    color: #2A2A2B;
    text-decoration: none;
    text-transform: uppercase;
    font-size: 1.6rem;
    transition: .1s ease;
    padding: 1rem;
  }

.button__sm:hover {
    transform: translateY(-2px);
}
</style>
