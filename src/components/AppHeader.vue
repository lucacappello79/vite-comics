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
    }

}
</style>