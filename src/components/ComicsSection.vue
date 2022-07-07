<template>

    <section class="cards-section">
        <div class="container">

            <!-- Element between jumbotron and the comics section -->
            <span class="current-btn btn">CURRENT SERIES</span>

            <!-- Container of all the cards -->
            <div class="cards-container">

                <ComicCard v-for="(singleCard, index) in cards" :key="index" :cardDetails="singleCard"/>

            </div>

            <!-- Element at the end of the section - load more -->
             <div class="load-btn btn">LOAD MORE</div>

        </div>
    </section>

</template>

<script>

    import ComicCard from '../components/ComicCard.vue';
    import ComicsJson from '../data/dc-comics.json';

    export default {
        name: "ComicsSection",
        components: {
            ComicCard
        },
        data() {
            return {
                cards: ComicsJson
            }
        },
    }

</script>

<style lang="scss" scoped>

    @import "../style/brand-colors.scss";
    
    .cards-section {
        position: relative;
        padding-top: 30px;
        padding-bottom: 15px;
        background-color: #1c1c1c;
        color: $secondary-color;
        .container {
            display: flex;
            flex-direction: column;
           .btn {
            cursor: pointer;
            background-color: $primary-color;
                &.load-btn {
                    margin-top: 50px;
                    align-self: center;
                    padding: 10px 40px;
                }
                &.current-btn {
                    padding: 15px 30px;
                    align-self: flex-start;
                    font-size: 24px;
                    font-weight: 700;
                    position: absolute;
                    left: 330px;
                    top: -30px;
                }
            }
            .cards-container {
                display: flex;
                flex-wrap: wrap;
                justify-content: space-around;
            }
        }
        
    }
    
</style>