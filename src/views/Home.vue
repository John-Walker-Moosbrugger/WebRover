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
    <!-- <cube-design-rover class="content designRover"/> -->
    <div id="team__line"></div>
    <!-- <cube-meet-team class="content meetTeam"/> -->
    <!-- <cube-contact class="content contact"/> -->
    <div id="footer__line"></div>
    <cube-footer class="content footer"/>
    <cube-partners class="content partners"/>
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
import SplashLarge from '@/components/SplashLarge.vue'
import CardsIntro from '@/components/home/CardsIntro.vue'
import CaseForSmall from '@/components/home/CaseForSmall.vue'
import Video from '@/components/home/Video.vue'
import NewsPreview from '@/components/NewsPreview.vue'
// import DesignRover from '@/components/DesignRover.vue'
// import MeetTeam from '@/components/MeetTeam.vue'
// import Contact from '@/components/Contact.vue'
import Footer from '@/components/Footer.vue'
import Partners from '@/components/Partners.vue'

export default {
  name: 'home',
  components: {
    'cube-header': Header,
    'cube-splash-large': SplashLarge,
    'cube-cards-intro': CardsIntro,
    'cube-case-for-small': CaseForSmall,
    'cube-video': Video,
    'cube-news-preview': NewsPreview,
    // 'cube-design-rover': DesignRover,
    // 'cube-meet-team': MeetTeam,
    // 'cube-contact': Contact,
    'cube-footer': Footer,
    'cube-partners': Partners

  }
}
</script>

<style lang="scss">
  #home {
    display: grid;
    grid-template-columns: minmax(10rem, 1fr) minmax(20rem, 114rem) minmax(10rem, 1fr);
    grid-template-rows: auto 65rem 15rem auto 10rem repeat(2, 30rem) 20rem auto 25rem 13rem 11rem min-content 20rem min-content min-content;
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

  .footer {
    grid-area: 21 / 2 / 22 / 3;
  }

  #footer__line {
    background-color: #50465E;
    grid-area: 21 / 1 / 22 /4;
  }

  .partners {
    grid-area: 22 / 2 / 23 / 3;
  }
@media only screen and (max-width: 1000px) {
  #home {
    grid-template-rows: auto 65rem 15rem auto 10rem repeat(2, 20rem) 27rem auto 25rem 13rem 11rem min-content 20rem min-content min-content;
  }
  #case {
    &__left {
      grid-row: 7 / 8;
      height: 20rem;
    }

    &__right {
      grid-row: 7 / 8;
      height: 20rem;
    }
  }
}
@media only screen and (max-width: 850px) {
  #home {
    grid-template-rows: auto 50rem 8rem auto 10rem repeat(2, 20rem) 27rem auto 10rem 13rem 11rem min-content 8rem min-content min-content;
  }
}
@media only screen and (max-width: 750px) {
  #home {
    grid-template-columns: minmax(5rem, 1fr) minmax(20rem, 114rem) minmax(5rem, 1fr);
    grid-template-rows: auto 55rem 8rem auto 10rem repeat(2, 20rem) 27rem auto 10rem 13rem 11rem min-content 8rem min-content min-content;
  }
}
@media only screen and (max-width: 650px) {
  #home {
    grid-template-rows: auto 41rem 8rem auto 10rem repeat(2, 20rem) 27rem auto 10rem 13rem 11rem min-content 8rem min-content min-content;
  }
}
@media only screen and (max-width: 450px) {
  #home {
    grid-template-rows: auto 32rem 8rem auto 10rem repeat(2, 20rem) 27rem auto 10rem 13rem 11rem min-content 8rem min-content min-content;
    grid-template-columns: minmax(2rem, 1fr) minmax(20rem, 114rem) minmax(2rem, 1fr);
  }
}
</style>
