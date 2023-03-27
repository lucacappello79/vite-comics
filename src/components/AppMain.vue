<script>
import AppComics from './AppComics.vue';

export default {
    data() {
        return {

            comics: [
                {
                    // "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                    "thumb": "/img/alita1.png",
                    "price": "$19.99",
                    "series": "Battle Angel Alita - Last Order",
                    "series2": "Action Comics",
                    "type": "comic book"
                },
                {
                    // "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                    "thumb": "/img/alita2.png",
                    "price": "$3.99",
                    "series": "Battle Angel Alita - Last Order",
                    "series2": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    // "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                    "thumb": "/img/alita3.png",
                    "price": "$16.99",
                    "series": "Battle Angel Alita - Last Order",
                    "series2": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    // "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                    "thumb": "/img/alita4.png",
                    "price": "$2.99",
                    "series": "Battle Angel Alita - Last Order",
                    "series2": "Batgirl",
                    "type": "comic book"
                },
                {
                    // "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "thumb": "/img/alita5.png",
                    "price": "$3.99",
                    "series": "Battle Angel Alita - Last Order",
                    "series2": "Batman",
                    "type": "comic book"
                },
                {
                    // "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "thumb": "/img/alita6.png",
                    "price": "$2.99",
                    "series": "Battle Angel Alita - Last Order",
                    "series2": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    // "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                    "thumb": "/img/alita7.png",
                    "price": "$3.99",
                    "series": "Battle Angel Alita - Last Order",
                    "series2": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    // "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                    "thumb": "/img/alita8.png",
                    "price": "$4.99",
                    "series": "Battle Angel Alita - Last Order",
                    "series2": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    // "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                    "thumb": "/img/alita9.png",
                    "price": "$5.99",
                    "series": "Battle Angel Alita - Last Order",
                    "series2": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    // "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                    "thumb": "/img/alita10.png",
                    "price": "$6.99",
                    "series": "Battle Angel Alita - Last Order",
                    "series2": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    // "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                    "thumb": "/img/alita11.png",
                    "price": "$4.99",
                    "series": "Battle Angel Alita - Last Order",
                    "series2": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "/img/alita12.png",
                    // "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                    "price": "$16.99",
                    "series": "Battle Angel Alita - Last Order",
                    "series2": "Catwoman",
                    "type": "graphic novel"
                }
            ],

        };
    },

    components: {
        AppComics,
    },
};
</script>

<template>
    <main>
        <div class="main-jumbo"></div>
        <div class="content centered">
            <div class="current-series">Current Series</div>
            <AppComics v-for="(item, index) in comics" :img="item.thumb" :title="item.series"></AppComics>
            <!-- --- Content Goes Here --- -->
        </div>
        <div class="load-more">Load More</div>
    </main>
</template>

<style  lang="scss" scoped>
@use "../scss/variables" as *;

main {
    background-color: black;
    padding-bottom: 30px;

    .main-jumbo {
        color: white;
        background-image: url(/img/jumbotron.jpg);
        background-size: cover;
        height: 300px;
        margin-bottom: 40px;
    }

    .content {

        @include centered();


        position: relative;
        display: flex;
        flex-flow: row wrap;
        justify-content: center;

        margin: 0 auto;
        width: 1200px;

        /* color: white;
        font-weight: bold;
        font-size: 1.5em;
        height: 150px;
    
        line-height: 150px;
        text-align: center; */

        .current-series {
            position: absolute;
            top: 0;
            left: 0;

            transform: translate(-50%, -150%);

            background-color: $main-color;
            color: white;
            font-weight: bold;
            text-transform: uppercase;
            padding: 8px 16px;
        }

    }

    .load-more {
        text-align: center;
        width: 180px;
        margin: 20px auto;

        background-color: $main-color;
        color: white;
        font-size: 0.8em;
        font-weight: bold;
        text-transform: uppercase;
        padding: 8px;
    }
}
</style>