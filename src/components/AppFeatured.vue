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
</template>

<style lang="scss" scoped>
.featured-wrapper {
    background-color: #0282f9;
    height: 250px;
    color: white;
    display: flex;
    align-items: center;
    justify-content: center;

    ul {
        display: flex;
        gap: 60px;
        justify-content: space-around;
        color: white;

        li {
            display: flex;
            gap: 20px;
            align-items: center;

            .img-wrapper {
                width: 60px;

                img {
                    width: 100%;
                }
            }
        }

    }
}
</style>