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
    <div class="footer-wrapper">
        <ul v-for="(singleList, singleListIndex) in footerLinks">
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
</template>

<style lang="scss" scoped>
.footer-wrapper {
    color: rgb(255, 255, 255);
    background-image: url(../../public/img/footer-bg.jpg);
    background-repeat: no-repeat;
}
</style>