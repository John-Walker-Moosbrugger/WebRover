<template>
    <div class="intro">
        <div class="intro__card">
            <h3 class="intro__card--title subtitle subtitle__purple">Modular</h3>
            <p class="intro__card--body">Our modular platforms are configurable to meet your mission requirements. Using our CubeRover system means there is no need to engineer your own rover without sacrificing reliability.</p>
        </div>
        <div class="intro__card">
            <h3 class="intro__card--title subtitle subtitle__purple">Lightweight</h3>
            <p class="intro__card--body">When every gram adds cost, a lightweight rover can open a whole new world of possibilities. Our rovers start at below 2kg meaning there is plenty of space for science.</p>
        </div>
        <div class="intro__card">
            <h3 class="intro__card--title subtitle subtitle__purple">Standardized</h3>
            <p class="intro__card--body">Standardized off-the-shelf components create robust systems you can trust and flexibility you will love. All without compromising your budget goals.</p>
        </div>
    </div>
</template>

<script>
export default {
  name: 'CardsIntro'
}
</script>

<style scoped lang="scss">
.intro {
    display: grid;
    grid-gap: 3rem;
    grid-template-columns: repeat(3, 1fr);

    &__card {

        &--title {
            position: relative;
            z-index: 10;
        }

        &--body {
            margin-top: -3rem;
            padding: 5rem 3rem 3rem 3rem;
            background-color: white;
            box-shadow: 0 3px 10px rgba(0,0,10px,.2);
        }
    }
}
</style>
