<template>
    <div class="dr_container">
        <img src="../assets/home/cuberover-exploded.jpg" alt="Image of CubeRover Parts" class="dr_img">
        <div class="dr_text">
            <h2 class="dr_text-title subtitle subtitle__purple">Design Your CubeRover</h2>
            <div class="dr_text-body">
                <ul class="dr_bullet">
                    <li class="dr_bullet-item text-reg">Choose your payload.</li>
                    <li class="dr_bullet-item text-reg">Customize your mobility.</li>
                    <li class="dr_bullet-item text-reg">Explore thermal and other constraints.</li>
                    <li class="dr_bullet-item text-reg">Slect the right chasis size.</li>
                </ul>
            </div>
            <router-link to="design" class="dr_button button__lg">Configure Here</router-link>
            <p class="dr_button-warn text__min">FOR MORE DETAILED INFORMATION OR A QUOTE, JUST GIVE US A CALL!</p>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.dr {
    &_container {
        display: flex;
        align-items: flex-end;
    }

    &_img {
        width: 50%;
    }

    &_text {
        display: flex;
        flex-direction: column;
        align-items: center;

        &-body {
            background-color: white;
            width: minmax(min-content, 60%);
            padding: 2rem 2rem 2rem 4rem;
            box-shadow: 0 3px 10px rgba(0,0,10px,.2);
        }
    }
    &_bullet {
        line-height: 2.2;
    }

    &_button {
        margin-top: 4rem;
        &-warn {
            text-align: center;
            width: 55%;
            margin-top: 1rem;
        }
    }
}
</style>
