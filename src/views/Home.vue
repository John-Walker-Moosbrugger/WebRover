<template>
  <div id="home">
    <cube-header class='content header'/>
    <cube-splash-large class='content splashLarge'/>
    <cube-cards-intro class='content introCards'/>
    <div id="case__left"></div>
    <cube-case-for-small class='content caseForSmall'/>
    <div id="case__right"></div>
    <cube-video class="content video"/>
    <cube-news-preview class="content newsPreview"/>
    <div id="news__line"></div>
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
import SplashLarge from '@/components/SplashLarge.vue'
import CardsIntro from '@/components/CardsIntro.vue'
import CaseForSmall from '@/components/CaseForSmall.vue'
import Video from '@/components/Video.vue'
import NewsPreview from '@/components/NewsPreview.vue'

export default {
  name: 'home',
  components: {
    'cube-header': Header,
    'cube-splash-large': SplashLarge,
    'cube-cards-intro': CardsIntro,
    'cube-case-for-small': CaseForSmall,
    'cube-video': Video,
    'cube-news-preview': NewsPreview
  }
}
</script>

<style lang="scss">
  #home {
    display: grid;
    grid-template-columns: 1fr minmax(60rem, 114rem) 1fr;
    grid-template-rows: auto 75vh 15rem auto 10rem repeat(2, 30rem) 20rem auto 25rem 13rem 11rem min-content 10rem;
  }

  .content {
    grid-column-start: 2;
    grid-column-end: 3;
  }

  .introCards {
    grid-row-start: 4;
  }

  .caseForSmall {
    grid-row: 6 / 8;

  }

  #case {
    &__left {
      background-color: #50465E;
      grid-row: 7 / 8;
    }

    &__right {
      background-color: #50465E;
      grid-row: 7 / 8;
    }
  }

  .video {
    grid-row-start: 9;
  }

  .newsPreview {
    grid-row-start: 11;
    grid-row-end: 14;
  }

  #news__line {
    background-color: #50465E;
    grid-area: 12 / 1 / 13 / 4;
  }
</style>
