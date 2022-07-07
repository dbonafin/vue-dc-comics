<template>

    <header>

       <div class="container">
            <!-- Logo container -->
            <div>
                <img src="../assets/img/dc-logo.png" alt="dc comics logo">
            </div>

            <!-- Header navigation area -->
            <nav>
                <ul>
                    <!-- Create a link for every object in the linksArray - different urls and texts -->
                    <li 
                    v-for="(link, index) in linksArray" 
                    :key="index" 
                    :class="{'active': link.active}"
                    >
                        <!-- If the item is active - add class 'active' to apply the css styles (li and a tags) -->
                        <a :class="{'active': link.active}" :href="link.url"> {{link.text}} </a>
                    </li>
                </ul>
            </nav>
       </div>
    </header>
    
</template>

<script>
    export default {
        name: "PageHeader", 
        data() {
            return {
                linksArray: [
                    {
                        url: "#",
                        text: "CHARACTERS",
                        active: false
                    },
                    {
                        url: "#",
                        text: "COMICS",
                        active: true
                    },
                    {
                        url: "#",
                        text: "MOVIES",
                        active: false
                    },
                    {
                        url: "#",
                        text: "TV",
                        active: false
                    },
                    {
                        url: "#",
                        text: "GAMES",
                        active: false
                    },
                    {
                        url: "#",
                        text: "COLLECTIBLES",
                        active: false
                    }, 
                    {
                        url: "#",
                        text: "VIDEOS",
                        active: false
                    },
                    {
                        url: "#",
                        text: "FANS",
                        active: false
                    }, 
                    {
                        url: "#",
                        text: "NEWS",
                        active: false
                    },
                    {
                        url: "#",
                        text: "SHOP",
                        active: false
                    }, 


                    
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
    @import "../style/common.scss";
    @import "../style/brand-colors.scss";

    header {
        background-color: white;
    }

    .container {
        height: 140px;
        line-height: 100%;
        display: flex;
        justify-content: space-between;
        align-items: center;
        ul {
            display: flex;
            li {
                line-height: calc(140px - 5px);
                margin: 0 10px;
                &.active {
                    color: $primary-color;
                    border-bottom: 5px solid $primary-color;
                } 
                a {
                    color: $tertiary-color;  
                    font-weight: 700;
                    &.active {
                    color: $primary-color;
                } 
                }
            }
        }
    }

</style>