<template>
  <div class=header>
    <a href="#" class="header__link">DESIGN YOUR ROVER</a>
    <a href="#" class="header__link">MISSION PROFILES</a>
    <a href="#" class="header__link--img"><img src="../assets/home/cuberover-logo.png" alt="CubeRover Logo" class="header__icon"></a>
    <a href="#" class="header__link">OUR TEAM</a>
    <a href="#" class="header__link">CAREERS</a>
    <a href="#" class="header__link">NEWS</a>
    <a href="#" class="header__link">GALLERY</a>
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
