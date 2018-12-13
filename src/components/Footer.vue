<template>
  <div class="footer">
    <div class="footer__nav">
      <div class="footer__nav--container">
        <h3 class="footer__nav--header title__xs "><a href="#" class="footer__nav--link">Mission Profiles</a></h3>
        <p class=""><a href="#" class="footer__nav--link">Lunar Science Missions</a></p>
        <p class=""><a href="#" class="footer__nav--link">STEM Education</a></p>
      </div>
      <div class="footer__nav--container">
        <h3 class="footer__nav--header title__xs "><a href="#" class="footer__nav--link">Design Your CubeRover</a></h3>
      </div>
      <div class="footer__nav--container">
        <h3 class="footer__nav--header title__xs "><a href="#" class="footer__nav--link">Our Team</a></h3>
        <p class=""><a href="#" class="footer__nav--link">Careers</a></p>
        <p class=""><a href="#" class="footer__nav--link">Contact Us</a></p>
      </div>
      <div class="footer__nav--container">
        <h3 class="footer__nav--header title__xs "><a href="#" class="footer__nav--link">News</a></h3>
      </div>
      <div class="footer__nav--container">
        <h3 class="footer__nav--header title__xs "><a href="#" class="footer__nav--link">Gallery</a></h3>
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
