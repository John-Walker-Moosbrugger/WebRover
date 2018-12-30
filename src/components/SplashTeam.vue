<template>
    <div class="splash-large">
        <div class="splash__top">
            <div class="splash__top--container">
                <img src="../assets/team/team_header.png" alt="Image of assembling a test rig for CubeRover" class="splash__img">
            </div>
            <h1 class="title title__white splash__top--title">More than a rover.</h1>
        </div>
        <h1 class="title title__purple title__bottom">We’re a team.</h1>
    </div>
</template>

<script>
export default {
  name: 'SplashLarge'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.splash {
    &-large {
        margin-top: 4rem;
        position: relative;
        display: flex;
        flex-direction: column;
    }

    &__top {
        display: flex;
        flex-direction: column;
        align-items: center;
        position: relative;

        &--container {
            height: 60vh;
            min-height: 45rem;
            max-height: 66rem;
            width: 80%;
            overflow: hidden;

            .splash__img {
                width: 100%;
            }
        }

        &--title {
            position: absolute;
            left: 0;
            bottom: 0;
        }
    }
}
.title {
    font-size: 8.5rem;

    &__bottom {
        width: max-content;
        align-self: flex-end;
    }

    &__purple {
        background-color: #50465E;
        color: white;
        padding: 0 8rem;
        z-index: 100;
        transform: translateY(-2rem);
    }

    &__white {
        background-color: white;
        box-shadow: 0px .3rem .6rem rgba(0, 0, 0, .23);
        padding: 0 8rem;
    }
}
</style>
