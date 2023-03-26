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

        <div class="featured-wrapper centered">
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
.centered {
    max-width: 1200px;
    margin: auto;
}

section {
    background-color: #0282f9;
}

.featured-wrapper {
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
                width: 40px;

                img {
                    width: 100%;
                }
            }
        }

    }
}
</style>