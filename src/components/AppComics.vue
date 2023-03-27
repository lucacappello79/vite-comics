<script>
export default {

    name: 'AppComics',

    data() {

        return {


        }
    },


    props: {
        img: String,
        title: String,
        link: String,
    }
};

</script>

<template>
    <a :href="link" target="_blank">
        <div class="card">
            <img :src="img" alt="">
            <div class="title">
                {{ title }}
            </div>
        </div>
    </a>
</template>

<style lang="scss" scoped>
.card {
    width: 200px;
    border: 1px solid black;
    padding: 10px;
    font-weight: bold;

    img {
        width: 100%;
    }

    ;

    .title {
        color: white;
    }

    &:hover {
        transform: scale(1.3);
    }
}
</style>