<template>
    <div class="splash-large">
        <img src="../assets/home/splash-lg.png" alt="Image of the CubeRover" class="splash-large__img">
        <h1 class="title">
            <span class="title__white">More than a rover.</span>
            <span class="title__purple">It's a platform.</span>
        </h1>
    </div>
</template>

<script>
export default {
  name: 'SplashLarge'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.splash-large {
    display: grid;
    grid-template-rows: 1fr 25rem;

    &__img {
        height: 60rem;
        grid-row-start: 1;
        grid-row-end: 3;
        grid-column-start: 1;
        justify-self: center;
    }
}
.title {
    grid-row-start: 2;
    grid-row-end: 3;
    grid-column-start: 1;
    position: relative;
    font-size: 8.5rem;

    &__purple {
        position: absolute;
        background-color: #50465E;
        color: white;
        right: 0;
        bottom: 0;
        padding: 0 8rem;
    }

    &__white {
        position: absolute;
        background-color: white;
        box-shadow: 0px .3rem .6rem rgba(0, 0, 0, .23);
        left: 0;
        top: 0;
        padding: 0 8rem;
    }
}
</style>
