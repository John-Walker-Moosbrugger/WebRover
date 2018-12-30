<template>
  <div class="t-intro">
    <div class="t-intro__text">
      <h3 class="subtitle subtitle__white"> Who we are.</h3>
      <p class="t-intro__text--body">Our team is a passionate group of professionals, excited to change the way we interact with our Solar System. We’re dedicated to helping more people engage with planetary bodies.<br><br>Our team has many years of experience working on lunar rovers, autonomous vehicles and other disruptive technologies from submarines to the hyperloop.</p>
    </div>
    <img src="../assets/team/team_intro.png" alt="Image of the CubeRover team at NASA GLEN research center" class="t-intro__img">
  </div>
</template>

<style lang="scss" scoped>
.t-intro {
  display: flex;
  align-items: center;

  &__text {
    width: 50%;

    &--body {
      padding: 3rem 3rem;
    }
  }

  &__img {
    width: 50%;
  }
}
</style>
