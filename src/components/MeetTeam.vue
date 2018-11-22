<template>
    <div class="mt__container">
        <div class="mt__body">
            <div>
                <h2 class="mt__body--title subtitle subtitle__white">Meet Our Team</h2>
                <p class="mt__body--text">Here at CubeRover the thing that binds us all together is a deep seeded love for space exploration. It’s not uncommon to find a few of us discussing the future of spaceflight over a few drinks and that passion is what drives us to do the work we do here.</p>
            </div>
            <a href="#" class="button__sm mt__body--btn">Learn More  <img src="../assets/icons/icon_arrow-light.png" alt="" class="icon__arrow"></a>
        </div>
        <div class="mt__img">
            <img src="../assets/home/meetTeam.jpg" alt="Photo of two people assembling a test rig" class="mt__img--content">
        </div>
    </div>
</template>

<style lang="scss" scoped>
.mt {
    &__container {
        display: flex;
        transform: translateY(-4rem);
    }
    &__body {
        width: 50%;
        padding-right: 8rem;
        display: flex;
        flex-direction: column;
        justify-content: space-between;

        &--text {
            padding-top: 4rem;
            padding-left: 3rem;
            color: white;
        }
        &--btn {
            margin-left: 2rem;
            color: white;
            width: max-content;
        }
    }
    &__img {
        width: 50%;
        position: relative;
        &--content {
            width: 100%;
        }
    }
}
</style>
