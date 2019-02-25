<template>
  <div style="partners">
    <img src="../assets/partners/CMU.png" alt="Carnegie Mellon Logo" class="partners__img">
    <img src="../assets/partners/Robotics_Institute.png" alt="Carnegie Mellon Logo" class="partners__img">
    <img src="../assets/partners/Astrobotic.png" alt="Carnegie Mellon Logo" class="partners__img">
    <img src="../assets/partners/NASA.png" alt="Carnegie Mellon Logo" class="partners__img">
    <img src="../assets/partners/Space_Nation.png" alt="Carnegie Mellon Logo" class="partners__img">
  </div>
</template>

<style lang="scss" scoped>
.partners {
  display: flex;
  justify-content: space-between;
  padding: 3rem 0;
  &__img {
    height: 5rem;
  }
}
@media only screen and (max-width: 750px) {
  .partners__img {
    height: 3rem;
  }
}

@media only screen and (max-width: 400px) {
  .partners__img {
    height: 2.5rem;
  }
}
</style>
