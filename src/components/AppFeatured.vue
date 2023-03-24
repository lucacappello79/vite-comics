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
    background-color: blue;
    height: 300px;
    color: white;
    display: flex;
    align-items: center;
    justify-content: center;

    ul {
        display: flex;
        gap: 20px;
        justify-content: space-around;
        color: white;

    }
}
</style>