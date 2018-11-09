<template>
  <div id="home">
    <cube-header class='content header'/>
    <cube-splash-large class='content splashLarge'/>
    <cube-cards-intro class='content introCards'/>
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
import SplashLarge from '@/components/SplashLarge.vue'
import CardsIntro from '@/components/CardsIntro.vue'

export default {
  name: 'home',
  components: {
    'cube-header': Header,
    'cube-splash-large': SplashLarge,
    'cube-cards-intro': CardsIntro
  }
}
</script>

<style lang="scss">
  #home {
    display: grid;
    grid-template-columns: 1fr minmax(60rem, 114rem) 1fr;
    grid-template-rows: auto 75vh 15rem auto 10rem auto;
  }

  .content {
    grid-column-start: 2;
    grid-column-end: 3;
  }

  .introCards {
    grid-row-start: 4;
  }
</style>
