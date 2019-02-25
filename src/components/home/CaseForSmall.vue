<template>
<div class="case">
    <div class="text">
        <h2 class="text__header">The Case For Small.</h2>
        <p class="text__body">
            Enables exploration of dangerous areas<br>
            Reduces cost of launch<br>
            Cross compatibility with CubeSats<br>
            Opportunities for rovers to collaborate<br>
            Narrow mission profiles on a flexible platform<br>
        </p>
    </div>
    <img src="../../assets/home/man-vs-cuberover.png" alt="" class="img">
    <div id="purple"></div>
</div>
</template>

<style scoped lang="scss">
.case {
    display: grid;
    grid-template-columns: minmax(max-content, 40%) 1fr;
    grid-template-rows: 30rem 30rem;
}

.text {
    grid-row-start: 2;
    grid-column-start: 1;

    &__header {
        padding: 1rem 3rem;
        font-size: 3.5rem;
        color: #50465E;
        background-color: white;
        width: max-content;
        box-shadow: 0 3px 10px rgba(0,0,10px,.2);
        margin-top: -4rem;
    }

    &__body {
        padding: 4rem 3rem;
        color: white;
        line-height: 2.2;
    }
}

.img {
    grid-column-start: 2;
    grid-row: 1 / 3;
    height: 60rem;
}

#purple {
    position: relative;
    z-index: -10;
    background-color: #50465E;
    grid-area: 2 / 1 / 3 / 3;
}

@media only screen and (max-width: 1000px) {
  .case {
    grid-template-columns: 1fr;
    grid-template-rows: 20rem 20rem min-content;
  }

  .text {
    width: 80%;
    justify-self: center;
    grid-row-start: 3;
    &__body {
      color: var(--color-grey-dark);
      padding: 2rem 3rem;
    }
  }

  .img {
    justify-self: center;
    height: 40rem;
    grid-column-start: 1;
  }
}

@media only screen and (max-width: 1000px) {
  .text {
    width: 100%;
  }
}
</style>
