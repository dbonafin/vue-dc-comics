<template>

    <div class="shop-section">
        <div class="container">

            <!-- Shop section with all the shop-options elements -->
            <ul>
                <li>
                    <a href="#">
                        <img src="../assets/img/buy-comics-digital-comics.png" alt="digital comics">
                    </a>
                    <span>DIGITAL COMICS</span>
                </li>
                 <li>
                    <a href="#">
                        <img src="../assets/img/buy-comics-merchandise.png" alt="merchandise">
                    </a>
                    <span>DC MERCHANDISE</span>
                </li>
                 <li>
                    <a href="#">
                        <img src="../assets/img/buy-comics-subscriptions.png" alt="subscriptions">
                    </a>
                    <span>SUBSCRIPTIONS</span>
                </li>
                 <li>
                    <a href="#">
                        <img src="../assets/img/buy-comics-shop-locator.png" alt="shop locator">
                    </a>
                    <span>SHOP LOCATOR</span>
                </li>
                 <li>
                    <a href="#">
                        <img src="../assets/img/buy-dc-power-visa.svg" alt="dc power visa">
                    </a>
                    <span>DC POWER VISA</span>
                </li>
            </ul>
        </div>
    </div>
    
</template>

<script>

    export default {
    name: "ShopSection"
    }

</script>

<style lang="scss" scoped>

    @import "../style/brand-colors.scss";

    img {
        width: 60px;
        height: 60px;
        object-fit: contain;
    }
    .shop-section {
        background-color: $primary-color;
        color: white;
        height: 200px;
        ul {
            display: flex;
            justify-content: space-around;
            align-items: center;
            height: 200px;
            li {
                display: flex;
                align-items: center;
                span {
                    margin: 0 7px;
                }
            }
        }
    }

</style>