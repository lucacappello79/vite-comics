<script>
export default {
    data() {
        return {
            headerLinks: ["CHARACTERS", "COMICS", "MOVIES", "TV", "GAMES", "COLLECTIBLES", "VIDEOS", "FANS", "NEWS", "SHOP"]

        };
    },
};
</script>

<template>
    <header>
        <div class="header-wrapper centered">
            <div class="logo">
                <img src="/img/dc-logo.png" alt="">
            </div>
            <div class="links">
                <ul>
                    <li v-for="(link, index) in headerLinks">
                        <a href="">{{ headerLinks[index] }}</a>
                    </li>
                </ul>
            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>
.centered {
    max-width: 1200px;
    margin: auto;
}

.header-wrapper {

    display: flex;
    justify-content: space-between;

    padding: 30px 0;

    ul {

        display: flex;
        gap: 30px;
        align-items: center;

        height: 100%;
        font-size: 0.8em;
        font-weight: bold;

        li {
            position: relative;

            a {
                color: #575757;

                &:hover {
                    color: #0282f9;
                }
            }
        }

        li:hover::before {

            width: 100%;
            height: 3px;
            background-color: #0282f9;

            content: "";
            position: absolute;
            bottom: -30px;
            left: 50%;
            transform: translateX(-50%);
        }

        //.active {
        //     position: absolute;
        //     bottom: -50px;
        //     left: 0;
        //     display: none;
        //     height: 3px;
        //     width: 100%;
        //     background-color: #0282f9;

        // }


    }



}
</style>