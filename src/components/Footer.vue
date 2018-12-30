<template>
  <div class="footer">
    <div class="footer__nav">
      <div class="footer__nav--container">
        <h3 class="footer__nav--header title__xs "><router-link to="/mission" class="footer__nav--link">Mission Profiles</router-link></h3>
        <p class=""><router-link to="/mission/science" class="footer__nav--link">Lunar Science Missions</router-link></p>
        <p class=""><router-link to="/mission/stem" class="footer__nav--link">STEM Education</router-link></p>
      </div>
      <div class="footer__nav--container">
        <h3 class="footer__nav--header title__xs "><router-link to="/design" class="footer__nav--link">Design Your CubeRover</router-link></h3>
      </div>
      <div class="footer__nav--container">
        <h3 class="footer__nav--header title__xs "><router-link to="/team" class="footer__nav--link">Our Team</router-link></h3>
        <p class=""><router-link to="/careers" class="footer__nav--link">Careers</router-link></p>
        <p class=""><router-link to="/team/contact" class="footer__nav--link">Contact Us</router-link></p>
      </div>
      <div class="footer__nav--container">
        <h3 class="footer__nav--header title__xs "><router-link to="/news" class="footer__nav--link">News</router-link></h3>
      </div>
      <div class="footer__nav--container">
        <h3 class="footer__nav--header title__xs "><router-link to="/gallery" class="footer__nav--link">Gallery</router-link></h3>
      </div>
    </div>
    <p class="footer__copy">Copyright © 2018 CubeRover</p>
  </div>
</template>

<script>
export default {}
</script>

<style scoped lang="scss">
.footer {
  color: white;
  padding: 3rem 0;

  &__nav {
    display: flex;
    justify-content: space-between;

    &--header {
      margin-bottom: 1rem;
    }

    &--link {
      transition: .1s ease-in;
      color: white;
      text-decoration: none;
    }
  }

  &__copy {
    text-align: center;
    margin-top: 2.5rem;
  }
}
</style>
