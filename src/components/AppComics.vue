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
    }
};

</script>

<template>
    <div class="card">
        <img :src="img" alt="">
        <div class="title">
            {{ title }}
        </div>
    </div>
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
}
</style>