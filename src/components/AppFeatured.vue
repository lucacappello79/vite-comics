<script>
export default {
    data() {
        return {
            featuredLinks: [

                {
                    text: 'DIGITAL COMICS',
                    img: '/img/buy-comics-digital-comics.png',
                },
                {
                    text: 'DC MERCHANDISE',
                    img: '/img/buy-comics-merchandise.png',
                },
                {
                    text: 'SUBSCRIPTION',
                    img: '/img/buy-comics-subscriptions.png',
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    img: '/img/buy-comics-shop-locator.png',
                },
                {
                    text: 'DC POWER VISA',
                    img: '/img/buy-dc-power-visa.svg',
                },
            ],

        };
    },
};
</script>

<template>
    <section>

        <div class="featured-wrapper">
            <ul>
                <li v-for="(item, index) in featuredLinks ">
                    <div class="img-wrapper">
                        <img :src="item.img" alt="">
                    </div>
                    <span>
                        {{ item.text }}
                    </span>
                </li>
            </ul>

        </div>

    </section>
</template>

<style lang="scss" scoped>
@use "../scss/variables" as *;


section {
    background-color: $main-color;
}

.featured-wrapper {

    @include centered();


    height: 150px;
    color: white;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 0 20px;

    ul {
        display: flex;
        gap: 45px;
        // gap: 60px;
        justify-content: space-around;
        color: white;

        li {
            display: flex;
            gap: 15px;
            align-items: center;

            .img-wrapper {
                width: 45px;

                img {
                    width: 100%;
                }

                ;
            }

            ;

            &:nth-child(4) {
                .img-wrapper {

                    img {
                        width: 80% // Your styles for the 4th img element go here
                    }

                    ;
                }

                ;
            }

            ;

        }

        ;

    }

    ;
}

;
</style>