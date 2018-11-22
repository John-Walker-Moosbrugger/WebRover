<template>
    <div class="contact__container">
        <h2 class="subtitle subtitle__purple contact__container--title">Get in Touch!</h2>
        <div class="contact__container--content">
            <div class="ct__left">
                <form action="Contact CubeRover" class="ct__form">
                    <input type="text" name="name" id="ct__name" class="ct__form--input" placeholder="NAME">
                    <input type="text" name="phone" id="ct__phone" class="ct__form--input" placeholder="PHONE">
                    <input type="text" name="email" id="ct__email" class="ct__form--input" placeholder="EMAIL">
                    <textarea name="message" id="ct__message" class="ct__form--input" placeholder="MESSAGE"></textarea>
                    <button class="button_lg">Submit</button>
                </form>
            </div>
            <div class="ct__right">
                <p class="ct__link"><img src="../assets/icons/icon_phone.png" alt="Icon of a phone" class="ct__link--icon">+1 (316) 922-2487</p>
                <p class="ct__link"><img src="../assets/icons/icon_email.png" alt="Icon of a email" class="ct__link--icon">info@cuberover.com</p>
                <p class="ct__link"><img src="../assets/icons/icon_twitter.png" alt="Icon for twitter" class="ct__link--icon">@CubeRover</p>
                <p class="ct__link"><img src="../assets/icons/icon_facebook.png" alt="Icon for facebook" class="ct__link--icon">www.facebook.com/cuberover/</p>
                <p class="ct__link"><img src="../assets/icons/icon_linkdin.png" alt="Icon for linkdin" class="ct__link--icon">www.linkedin.com/company/cuberover/</p>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.contact__container {
    background-color: white;

    &--content {
        box-shadow: 0px 3px 20px rgba(0,0,0,.2);
        margin-top: -3rem;
        margin-left: 4rem;
        padding: 8rem 7rem;
        height: 55rem;
        display: flex;
        justify-content: space-between;
    }
}

.ct {

    &__left {
        width: 40%;
    }

    &__right {
        width: 40%;
        display: flex;
        flex-direction: column;
    }

    &__link {
        display: flex;
        align-items: center;
        margin-bottom: 2rem;

        &--icon {
            margin-right: 2rem;
        }
    }

    &__form {
        display: flex;
        flex-direction: column;
        align-items: center;

        &--input {
            width: 100%;
            border: none;
            border-bottom: 2px solid #50465E;
            padding: 1.5rem;
            margin-bottom: 1rem;
            resize: vertical;
            min-height: 4rem;
            max-height: 20rem;
            transition: .15s ease-in-out;

            &:focus {
                background-color: rgb(240, 240, 240);
                outline: none;
            }
        }
    }
}
</style>
