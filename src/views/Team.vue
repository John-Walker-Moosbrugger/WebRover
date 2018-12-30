<template>
  <div id="team">
    <cube-header class="content"></cube-header>
    <cube-splash-team class="content"></cube-splash-team>
    <cube-team-intro class="content" id="teamIntro"></cube-team-intro>
    <cube-team-bios class="content" id="teamBios"></cube-team-bios>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import SplashTeam from '@/components/SplashTeam.vue'
import TeamIntro from '@/components/TeamIntro.vue'
import TeamBios from '@/components/TeamBios.vue'

export default {
  components: {
    'cube-header': Header,
    'cube-splash-team': SplashTeam,
    'cube-team-intro': TeamIntro,
    'cube-team-bios': TeamBios
  }
}
</script>

<style lang="scss" scoped>
#team {
  display: grid;
  grid-template-columns: 1fr minmax(60rem, 114rem) 1fr;

  &Intro {
    margin-top: 6rem;
  }
}

.content {
  grid-column-start: 2;
  grid-column-end: 3;
}
</style>
