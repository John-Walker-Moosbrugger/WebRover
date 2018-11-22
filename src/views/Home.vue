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
    <cube-design-rover class="content designRover"/>
    <div id="team__line"></div>
    <cube-meet-team class="content meetTeam"/>
    <cube-contact class="content contact"/>
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
import DesignRover from '@/components/DesignRover.vue'
import MeetTeam from '@/components/MeetTeam.vue'
import Contact from '@/components/Contact.vue'

export default {
  name: 'home',
  components: {
    'cube-header': Header,
    'cube-splash-large': SplashLarge,
    'cube-cards-intro': CardsIntro,
    'cube-case-for-small': CaseForSmall,
    'cube-video': Video,
    'cube-news-preview': NewsPreview,
    'cube-design-rover': DesignRover,
    'cube-meet-team': MeetTeam,
    'cube-contact': Contact

  }
}
</script>

<style lang="scss">
  #home {
    display: grid;
    grid-template-columns: 1fr minmax(60rem, 114rem) 1fr;
    grid-template-rows: auto 75vh 15rem auto 10rem repeat(2, 30rem) 20rem auto 25rem 13rem 11rem min-content 20rem min-content 30rem min-content 25rem 60rem 10rem;
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

  .designRover {
    grid-row-start: 15;
    grid-row-end: 16;
  }

    #team__line {
    background-color: #50465E;
    grid-area: 17 / 1 / 18 /4;
  }

  .meetTeam {
    grid-row: 17 / 18;
  }

  .contact {
    grid-area: 19 / 2 / 20 / 3;
  }
</style>
