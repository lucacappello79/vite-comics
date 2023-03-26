<script>
export default {
    data() {
        return {

        };
    },
};
</script>

<template>
    <section class="social">
        <div class="social-wrapper">
            <div class="social-left">
                <button>SIGN-UP NOW!</button>
            </div>
            <div class="social-right">
                <span>FOLLOW US</span>
                <div class="logo-wrapper">
                    <img src="/img/footer-facebook.png" alt="">
                    <img src="/img/footer-twitter.png" alt="">
                    <img src="/img/footer-youtube.png" alt="">
                    <img src="/img/footer-pinterest.png" alt="">
                    <img src="/img/footer-periscope.png" alt="">
                </div>

            </div>

        </div>
    </section>
</template>

<style lang="scss" scoped>
@use "../scss/variables" as *;

// .centered {
//     max-width: 1200px;
//     margin: auto;
// }

.social {
    background-color: #303030;
}

.social-wrapper {

    @include centered();

    display: flex;
    justify-content: space-between;
    font-weight: bold;
    height: 100px;

    .social-left {
        display: flex;
        align-items: center;
    }

    button {
        background-color: #303030;
        font-weight: bold;
        color: white;
        padding: 10px;
        border: 2px solid $main-color;
    }

    .social-right {
        display: flex;
        align-items: center;
    }

    span {
        font-size: 1.1em;
        color: $main-color;
        margin-right: 25px;
    }

    .logo-wrapper {
        display: flex;
        justify-content: space-between;
        gap: 15px;
    }
}
</style>
