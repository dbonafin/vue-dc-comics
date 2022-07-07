<template>
    <!-- Single card template -->
    <div class="single-card">
        <img :src="cardDetails.thumb" :alt="cardDetails.series">
        <h4>{{cardDetails.series}}</h4>
    </div>

</template>

<script>

    export default {
        name: "ComicCard",
        props: {
            cardDetails: Object
        }
    }

</script>

<style lang="scss">

    @import "../style/brand-colors.scss";
    
    .single-card {
        margin: 30px 20px;
        width: calc((100% / 6) - 40px);
        height: 220px;
        h4 {
            text-transform: uppercase;
            color: $secondary-color;
            font-size: 14px;
            text-align: center;
            margin-top: 10px;
        }
        img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: top;
            cursor: pointer;
        }
    }

</style>
