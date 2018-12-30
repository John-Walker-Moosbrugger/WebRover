<template>
  <div class=header>
    <router-link to="/design" class="header__link">DESIGN YOUR ROVER</router-link>
    <router-link to="/mission" class="header__link">MISSION PROFILES</router-link>
    <router-link to="/" class="header__link--img"><img src="../assets/home/cuberover-logo.png" alt="CubeRover Logo" class="header__icon"></router-link>
    <router-link to="/team" class="header__link">OUR TEAM</router-link>
    <router-link to="/careers" class="header__link">CAREERS</router-link>
    <router-link to="/news" class="header__link">NEWS</router-link>
    <router-link to="/gallery" class="header__link">GALLERY</router-link>
  </div>
</template>

<script>
export default {
  name: 'Header'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 2rem;

  &__link,
  &__link:visited  {
    color: #2A2A2B;
    text-decoration: none;
    text-transform: uppercase;
    font-size: 1.6rem;
    transition: .1s ease;
    padding: 1rem;
  }

  &__link:hover {
    transform: translateY(-2px);
  }

  &__icon {
    height: 3rem;
  }
}
</style>
