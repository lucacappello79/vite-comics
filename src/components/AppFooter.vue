<script>
export default {
    data() {
        return {

            footerLinks: [
                {
                    title: "DC COMICS",
                    lista: [
                        'Characters', 'Comics', 'Movies', 'TV', 'Games', 'Videos', 'News'
                    ],
                },
                {
                    title: "SHOP",
                    lista: [
                        'Shop DC', 'Shop DC Collectibles'
                    ],
                },
                {
                    title: "DC",
                    lista: [
                        'Terms of Use', 'Privacy Policy', 'Ad Choices', 'Advertising', 'Jobs', 'Talent Workshop', 'Subscriptions', 'CPSC Certificates', 'Ratings', 'Shop Help', 'Contact Us'
                    ],
                },
                {
                    title: "SITES",
                    lista: [
                        'DC', 'MAD Magazine', 'DC Kids', 'DC Universe', 'DC Power Visa'
                    ]
                },
            ]

        };
    },
};
</script>

<template>
    <footer>
        <div class="footer-wrapper centered">
            <div class="bottom-links">
                <div class="col-left">
                    <ul v-for="(singleList, singleListIndex) in footerLinks.slice(0, 2)">
                        <li>
                            <strong>{{ singleList.title }}</strong>
                            <ul>
                                <li v-for="(item, itemIndex) in singleList.lista">
                                    {{ item }}
                                </li>
                            </ul>
                        </li>
                    </ul>
                </div>
                <div class="col-right">
                    <ul v-for="(singleList, singleListIndex) in footerLinks.slice(2)">
                        <li>
                            <strong>{{ singleList.title }}</strong>
                            <ul>
                                <li v-for="(item, itemIndex) in singleList.lista">
                                    {{ item }}
                                </li>
                            </ul>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="img-wrapper">
                <img src="/img/dc-logo-bg.png" alt="">
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
.centered {
    max-width: 1200px;
    margin: auto;
}

footer {
    background-image: url(/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;

}

.footer-wrapper {

    font-size: 0.9em;
    display: flex;
    justify-content: space-between;

    // padding: 50px 0;

    color: rgb(255, 255, 255);
    // background-image: url(../../public/img/footer-bg.jpg);

    .bottom-links {
        display: flex;
        gap: 80px;

        .col-left {
            display: flex;
            flex-direction: column;
        }

        .col-right {
            display: flex;
            gap: 80px;
        }
    }

}

.img-wrapper {
    display: flex;
    align-items: center;
    justify-content: center;

    height: 450px;
    overflow: hidden;

    img {

        width: 100%;
        height: 130%;
        object-fit: cover;
        // object-position: center;
    }

}

li {
    color: #959595;
    padding: 2px;
}

strong {
    color: white;
    font-size: 1.2em;
    line-height: 60px;
}
</style>